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