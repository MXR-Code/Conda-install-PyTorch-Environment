```bash
conda create -n kg python=3.10
conda activate kg

nvcc --version
# Cuda compilation tools, release 12.4, V12.4.131
conda install cudatoolkit cuda-cudart cuda-nvtx cuda cuda-compiler -c nvidia -c conda-forge
conda install cudatoolkit cuda-cudart cuda-nvtx cuda cuda-compiler=12.4 -c nvidia -c conda-forge

conda install pytorch pytorch-cuda torchvision torchaudio -c pytorch
conda install pytorch pytorch-cuda=12.4 torchvision torchaudio -c pytorch

conda install sentence-transformers -c conda-forge

conda install datasets -c HuggingFace
conda install huggingface_hub transformers tokenizers datasets -c conda-forge
conda install azure-identity openai wandb rich accelerate evaluate nltk rouge-score absl-py bert_score openpyxl -c conda-forge

conda remove --name kg --all
conda clean --all -y
```
```bash
conda create -n mxr_kgllm python=3.10 -y
conda activate mxr_kgllm
nvcc --version

conda install cuda-toolkit=11.8 cuda-cupti=11.8 cuda-cudart=11.8 cuda-nvtx=11.8 cuda=11.8 cuda-compiler=11.8 cuda-runtime=11.8 cuda-nvprune=11.8 cuda-nvprune=11.8 cuda-libraries=11.8 -c nvidia
conda install pytorch pytorch-cuda=11.8 torchvision torchaudio torchdata -c pytorch

conda install huggingface_hub transformers tokenizers datasets sentence-transformers -c conda-forge
conda install azure-identity openai wandb rich accelerate evaluate nltk rouge-score absl-py bert_score openpyxl -c conda-forge

conda install pyg=*=*cu* pytorch-scatter pytorch-sparse pytorch-cluster pytorch-spline-conv -c pyg

torchdata opencv pillow numpy scipy openpyxl pandas matplotlib scikit-learn grpcio optuna absl-py alembic colorlog imbalanced-learn llvmlite littleutils mako markdown numba ogb outdated protobuf tensorboard tensorboard-data-server werkzeug pydantic igraph cmake -c pytorch -c pyg -c conda-forge  -c nvidia


conda activate base
conda remove --name mxr_kgllm --all -y
conda clean --all -y
```

```bash
conda create -n uni python=3.10
conda activate uni

nvcc --version
# Cuda compilation tools, release 12.4, V12.4.131
conda install cudatoolkit cuda-cudart cuda-nvtx cuda cuda-compiler -c nvidia -c conda-forge
conda install cudatoolkit cuda-cudart cuda-nvtx cuda cuda-compiler=12.4 -c nvidia -c conda-forge

conda install pytorch pytorch-cuda torchvision torchaudio -c pytorch
conda install pytorch pytorch-cuda=12.4 torchvision torchaudio -c pytorch

conda install huggingface_hub transformers tokenizers datasets timm -c conda-forge

conda remove --name uni --all
conda clean --all -y
```
