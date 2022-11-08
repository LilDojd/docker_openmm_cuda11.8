# A repository containing files for building OpenMM 7.7.0 image with CUDA 11.8 support for 520.x NVIDIA drivers

Build with: 
```
DOCKER_BUILDKIT=1 docker build -t openmm7.7.0-cuda11.8 .
```
Run with:
```
docker run --gpus all --ipc=host --ulimit memlock=-1 --ulimit stack=67108864 ...
```

# This container image contains the complete source of the version of PyTorch in /opt/pytorch. It is prebuilt and installed in the Conda default environment (/opt/conda/lib/python3.8/site-packages/torch/) in the container image. 
