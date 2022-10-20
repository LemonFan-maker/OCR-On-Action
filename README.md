<h1 align="center">在 GitHub Action 上部署 OCR 服务</h1>

## 一、特性

- [x] **参考chineseocr大佬的仓库，稍作修改[^1]，方便GitHub部署**

- [x] 开箱即用

- [x] 自动下载模型文件

- [x] 内网穿透，直接访问

- [x] 随机链接，防止接口盗用

## 二、食用方法

*fork*本仓库，直接*Action*运行

**提示:** 如果要采用固定接口，请切换*branch*到**API**

家用(即:树莓派,等设备)**CPU**部署请参考[setup-cpu.md](./setup-cpu.md)
  
**注意1:** 准备时间长是正常现象.
   
~~**注意2:** *API*分支正在维护中.~~[^2]

## 三、原理
![OCR-On-Action](./assets/OCR-On-Action.svg)

[^1]: 测试的时候发现chineseocr大佬*setup-cpu.md*有亿点问题[^3]，影响开心地使用.本仓库友好修改了*setup-cpu.md*文件，老少皆可放心食用.有问题直接开Issue.[^4]
[^2]: 应该维护好了？有问题开Issue.
[^3]: ``numpy``和``h5py``版本有问题，导致运行报错，本仓库已修复.
[^4]: **不要问我什么模型怎么转换，什么pytorch怎么了:rofl:.有模型训练上的任何问题请自觉点击这个[chineseocr踢馆](https://github.com/chineseocr/chineseocr/issues).[^5]**
[^5]: 对不起，chineseocr大佬，我是故意的:yum:.
