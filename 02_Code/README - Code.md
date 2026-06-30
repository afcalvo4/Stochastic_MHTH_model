<div align="center">

# Code

 
</div>
Place all files required to recreate the published paper and key results from this project here.

## Description

What it does

## How to run

Install dependencies

```bash
# clone project
git clone https://github.com/YourGithubName/your-repo-name
cd your-repo-name

# [OPTIONAL] create conda environment
conda create -n myenv python=3.8
conda activate myenv

# install pytorch according to instructions
# https://pytorch.org/get-started/

# install requirements
pip install -r requirements.txt
```

Train model with default configuration

```bash
# train on CPU
python run.py trainer.gpus=0

# train on GPU
python run.py trainer.gpus=1
```

Train model with chosen experiment configuration from [configs/experiment/](configs/experiment/)

```bash
python run.py experiment=experiment_name.yaml
```

You can override any parameter from command line like this

```bash
python run.py trainer.max_epochs=20 datamodule.batch_size=64
```