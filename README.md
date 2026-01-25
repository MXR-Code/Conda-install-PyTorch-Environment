```bash
conda create -n mxr_kgllm python=3.10 -y
conda activate mxr_kgllm 

# Cuda Version
nvcc --version
nvidia-smi

# GPU Pytorch
conda install pytorch pytorch-cuda=11.8 torchvision torchaudio torchdata -c pytorch -c nvidia

# Huggingface Packages
conda install huggingface_hub=0.34 transformers=4.56 tokenizers=0.22.0 datasets=4.0 sentence-transformers=5.1.0 -c conda-forge

# GPU Pytorch Geometric 
conda install pyg=*=*cu* pytorch-scatter pytorch-sparse pytorch-cluster pytorch-spline-conv -c pyg

# kg 
conda install pykeen -c mfratello -c conda-forge

# Other
conda install nvidia wandb rich accelerate evaluate nltk rouge-score absl-py bert_score openpyxl selenium fire peft ninja torchdata opencv pillow numpy scipy pandas matplotlib scikit-learn grpcio optuna alembic colorlog imbalanced-learn llvmlite littleutils mako markdown numba ogb outdated protobuf tensorboard tensorboard-data-server werkzeug pydantic igraph cmake -c pytorch -c pyg -c conda-forge

# for Linux
conda triton -c conda-forge

conda activate base
conda remove --name mxr_kgllm --all -y
conda clean --all -y
```


