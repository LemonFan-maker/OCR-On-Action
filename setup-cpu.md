## **提示：** 由于某些省份[清华镜像源](https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple)访问较慢，替换[北京外国语大学镜像站](https://mirrors.bfsu.edu.cn/pypi/web/simple)。

## 使用方法

**1.** 安装[Anaconda](https://mirrors.bfsu.edu.cn/anaconda/archive/Anaconda3-2019.10-Linux-x86_64.sh),可直接单击进行下载

**2.** 创建虚拟环境

```sh
conda create -n OCR python=3.6 pip scipy
source activate OCR
```

**3.** 编译darknet

```sh
cd OCR-On-Action
rm -rf darknet
git clone https://github.com/LemonFan-maker/Only-for-Action.git && mv Only-for-Action darknet
```

**修改``darknet/python/darknet.py``的``lib = CDLL("/home/runner/ocr/darknet/libdarknet.so", RTLD_GLOBAL)``为自己的*darknet*地址**

```sh
make && cd ..
```

**4.** 安装依赖

```sh
pip install easydict opencv-contrib-python==4.0.0.21 Cython h5py==2.10.0 lmdb numpy==1.16 mahotas pandas requests bs4 matplotlib lxml -i https://mirrors.bfsu.edu.cn/pypi/web/simple
pip install -U pillow -i https://mirrors.bfsu.edu.cn/pypi/web/simple
pip install web.py==0.40.dev0 redis
pip install keras==2.1.5 tensorflow==1.8
```

**5.** 安装pytorch

```sh
#linux
conda install pytorch-cpu torchvision-cpu -c pytorch
```

**6.** 运行OCR服务
```sh
cd OCR-On-Acion
python web.py 8081
```

**7.** 访问OCR

- 本机OCR
  - 浏览器直接访问 *0.0.0.0:8081/ocr*或*127.0.0.1:8081/ocr*

- 局域网OCR
  - 浏览器直接访问 *本机IP:8081/ocr*
