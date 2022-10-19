##CPU 环境配置，支持linux\macOs
conda create -n chineseocr python=3.6 pip scipy jupyter ipython ##运用conda 创建python环境
source activate chineseocr
cd darknet/ && make && cd ..
pip install easydict opencv-contrib-python==4.0.0.21 Cython h5py==2.10.0 lmdb numpy==1.16 mahotas pandas requests bs4 matplotlib lxml -i https://mirrors.bfsu.edu.cn/pypi/web/simple
pip install -U pillow -i https://mirrors.bfsu.edu.cn/pypi/web/simple
pip install web.py==0.40.dev0 redis
pip install keras==2.1.5 tensorflow==1.8
## mac
conda install pytorch torchvision -c pytorch
## linux
## conda install pytorch-cpu torchvision-cpu -c pytorch

