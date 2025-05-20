```bash
conda create -n kg python=3.10
conda activate kg
conda install cudatoolkit cuda-cudart cuda-nvtx cuda -c nvidia -c conda-forge
conda install pytorch pytorch-cuda torchvision torchaudio -c pytorch

# conda remove --name kg --all
conda clean --all -y

# conda install datasets -c HuggingFace
# conda install huggingface_hub transformers tokenizers datasets -c conda-forge
# conda install azure-identity openai wandb rich accelerate evaluate nltk -c conda-forge
```
