<h1 align="center">在 GitHub Action 上部署 OCR 服务</h1>

### 请自觉遵守[MIT License](https://github.com/LemonFan-maker/OCR-On-Action/blob/master/LICENSE)

## 一、特性

- [x] **参考chineseocr大佬的仓库，稍作修改，方便GitHub部署**

- [x] 开箱即用

- [x] 自动下载模型文件

- [x] 内网穿透，直接访问

- [x] 固定链接，可用接口，但限时[^1]

## 二、准备什么
**1.** 一个域名。
- 域名要求
  - 一、二级域名均可
  - 能添加**CNAME**解析

**2.** 亿点点修改**Action yaml**文件的能力
- 能看到这个*Branch*，应该都没啥大问题

## 三、食用方法

*fork*本仓库，填写*Action*必要字段并运行

家用(即:树莓派,等设备)**CPU**部署请参考[setup-cpu.md](./setup-cpu.md)
  
**注意1:** 准备时间长是正常现象.
   
**注意2:** 此分支已经维护完成

## 四、原理
![OCR-On-Action](./assets/OCR-On-Action.svg)

 [^1]: 具体限时请参考[GitHub帮助文档](https://docs.github.com/cn/billing/managing-billing-for-github-actions/about-billing-for-github-actions)
