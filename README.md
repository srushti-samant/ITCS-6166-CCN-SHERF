# ITCS-6166-CCN
# SHERF: Generalizable Human NeRF from a Single Image
This is a repository for the final project of Group 7 for the course ITCS 6166/8166 (Computer Communication and Networks) under the guidance of Dr. Pu Wang. It has detailed instructions on how to run the project using Google Colab. We recreated the results of the project SHERF: Generalizable Human NeRF from a Single Image.

                               SHERF learns a Generalizable Human NeRF to animate 3D humans from a single image.
1) NVIDIA GPUs are required for this project. We recommand Using 4 gpus for running this project.
2) We used Google Colab and anaconda to manage the python environment.
3) Grp7-SHERF.ipynb is our colab file. Open it and follow the steps.

# Setting up Environment
1)  conda create --name sherf python=3.8
2)   conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 cudatoolkit=11.3 -c pytorch
3)    conda install -c fvcore -c iopath -c conda-forge fvcore iopath
4)   conda install pytorch3d -c pytorch3d (or pip install --no-index --no-cache-dir pytorch3d -f https://dl.fbaipublicfiles.com/pytorch3d/packaging/wheels/py38_cu113_pyt1110/download.html)
5)   pip install -r requirements.txt
6)   conda activate sherf

# Set up Dataset
Due to Large and Complex datasets, which are diffcult to Unzip we used only one dataset.

# 🖥️RenderPeople Dataset

Please download the rendered multi-view images of RenderPeople dataset from this link [Onedrive](https://mycuhk-my.sharepoint.com/personal/1155098117_link_cuhk_edu_hk/_layouts/15/onedrive.aspx?id=%2Fpersonal%2F1155098117%5Flink%5Fcuhk%5Fedu%5Fhk%2FDocuments%2FICCV2023%5FSHERF%2FRenderPeople%5Frecon&ga=1).

# 🏃‍♀️Inference

# Download Models

The pretrained models and SMPL model are needed for inference.

The pretrained models are put in [OneDrive](https://mycuhk-my.sharepoint.com/personal/1155098117_link_cuhk_edu_hk/_layouts/15/onedrive.aspx?id=%2Fpersonal%2F1155098117%5Flink%5Fcuhk%5Fedu%5Fhk%2FDocuments%2FICCV2023%5FSHERF%2FSHERF%5Fcheckpoint%2Ezip&parent=%2Fpersonal%2F1155098117%5Flink%5Fcuhk%5Fedu%5Fhk%2FDocuments%2FICCV2023%5FSHERF&ga=1).

Register and download SMPL models [here](https://smpl.is.tue.mpg.de/). Put the downloaded models in the folder smpl_models. Only the neutral one is needed. The folder structure should look like
