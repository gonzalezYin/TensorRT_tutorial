# TensorRT_tutorial

## PyCUDA Installation
```
pip install pycuda==2021.1
```
To test you've installed successfully, run the commands as follows.
```
import pycuda.autoinit
import pycuda.driver
free_bytes, total_bytes = pycuda.mem_get_info()
print(free_bytes, total_bytes)
```

## 半自动安装
半自动安装通过拉取官方镜像，然后创建容器，在容器内部安装.[完整的镜像列表](https://gitlab.com/nvidia/container-images/cuda/blob/master/doc/supported-tags.md)
```
sudo snap install docker
sudo docker pull nvidia/cuda:11.3.0-cuddnn8-devel-ubuntu20.04
```
