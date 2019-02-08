# Ready 2019 Demo

## Local machine setup

1. Visual Studio Code + Azure ML extension

2. Install required packages for local machine:
    - Automatically via conda:
        - `conda env create -n manufacturing --file env.yml`
        - `conda activate manufacturing`
    - Manually via pip:
        - azureml-sdk
        - numpy
        - Pillow
        - protobuf
        - tensorflow==1.10.0
        - jupyter
        - matplotlib

3. Data files: download from [here](https://contosomanufac0283843562.blob.core.windows.net/demo/data.tar.gz) and extract into the `data`, `images`, and `models` directories.

## Remote setup

1. Ensure you have access to the `scottgu-all-hands` resource group.

## Scenario notes

Contoso Manufacturing is committed to providing a safe workplace environment for its employees. As part of that goal, they recognize safety equipment - like hard hats and high viz jackets - helps reduce and/or mitigate the risk of injuries on the factory floor. While most of their employees wear the required equipment, adoption is less than 100%, often due to new staff and visitors, and hard to monitor.

To address these challenges, Contoso has decided to use machine learing to automatically identify safety violations in their most high risk areas. By taking an existing object detection model and using transfer learning, they're able to add their own data and quickly develop a custom model with Azure ML.