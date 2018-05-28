# Install_TF

## 安装NVIDIA显卡驱动

## 安装CUDA

## 安装CuDNNv6
    # 复制
      cd cuda/include
      sudo cp cudnn.h /usr/local/cuda/include/
    # 复制
      cd ../lib64
      sudo cp lib* /usr/local/cuda/lib64/
      cd /usr/local/cuda/lib64/
    # 更改权限
      sudo chmod a+x /usr/local/cuda/include/cudnn.h  /usr/local/cuda/lib64/libcudnn*

## 安装Tensorflow（清华镜像）
    # cp27-1.4
        pip install -i https://pypi.tuna.tsinghua.edu.cn/simple/ https://mirrors.tuna.tsinghua.edu.cn/tensorflow/linux/gpu/tensorflow_gpu-1.4.0-cp27-none-linux_x86_64.whl

    # cp27-1.3
        pip install -i https://pypi.tuna.tsinghua.edu.cn/simple/ https://mirrors.tuna.tsinghua.edu.cn/tensorflow/linux/gpu/tensorflow_gpu-1.3.0-cp27-none-linux_x86_64.whl

    # cp27-1.2.1
        pip install -i https://pypi.tuna.tsinghua.edu.cn/simple/ https://mirrors.tuna.tsinghua.edu.cn/tensorflow/linux/gpu/tensorflow_gpu-1.2.0-cp27-none-linux_x86_64.whl

##  导入tensorflow时报警告
      >>> import tensorflow
      /usr/local/lib/python2.7/dist-packages/h5py/__init__.py:36: FutureWarning: Conversion of the second argument of issubdtype from `float` to `np.floating` is deprecated. In future, it will be treated as `np.float64 == np.dtype(float).type`.
      from ._conv import register_converters as _register_converters

      解决方案：
      sudo pip install h5py==2.8.0rc1






#
