
<p align="center">
<h1 align="center">新讯 WR800 随身wifi固件</h1>
</p>
<p align="center">
    <img alt="Gitea Stars" src="https://img.shields.io/github/stars/x7780/MF32T_MB_V01?style=flat-square&logo=GitHub">
    <img alt="GitHub forks" src="https://img.shields.io/github/forks/x7780/MF32T_MB_V01?style=flat-square&logo=GitHub">
    <img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/t/x7780/MF32T_MB_V01?style=flat-square&logo=GitHub">
    <img alt="GitHub Issues or Pull Requests" src="https://img.shields.io/github/issues-closed-raw/x7780/MF32T_MB_V01?style=flat-square&logo=GitHub">
    <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/x7780/MF32T_MB_V01?style=flat-square&logo=GitHub">
    <img alt="GitHub License" src="https://img.shields.io/github/license/x7780/MF32T_MB_V01?style=flat-square">
</p>

<!-- Start of Selection -->
## 设备信息
- **品牌**：新讯 WR800 （黑色）
- **板子型号**：MF32T_MB_V01
- **芯片**：高通 410 （msm8916）
- **WiFi 密码**：12345678
- **Web 管理密码**：admin
- **切卡密码**：admin
- **Root 状态**：已获取
- **ADB 状态**：已开启

## 目录详情
- **APP**：存放常用刷机后用的应用程序。
- **驱动工具**：请先安装 `9008drive.exe`，其他工具可自行选择安装。
- **完整固件**：存放完整固件，方便下载。
## MiKo和boot.img，system.img固件在网盘里面
因为固件太大，无法上传，请自行下载。
https://www.123865.com/s/dgXbjv-9Sgfd?  提取码:6666

## 刷机原因
新买的随身wifi，存在限速、切卡、掉线等问题，且由于 boot 中存在强空，设备价格仅为 15 元，使用高通 410 芯片，性价比高。

## 刷机前注意事项
1. 使用螺丝刀打开随身WiFi，确认板子上信号是否为 MF32T_MB_V01。如果不是该型号，请勿刷机。
2. 刷机前请务必备份，以避免刷错。

## 备份设备
1. 安装 `9008drive.exe`，一路点击“下一步”即可。
2. 进入 9008 模式：
   - 先断开 USB，取下电池，找到板子上的 fb 位置（仔细查看，在板子边缘），共有 4 个金点。用镊子按住中间 2 个金点，然后插入 USB，数到3，即可进入 9008 模式。右键点击“我的电脑” - “管理” - “设备管理器” - “端口（COM 和 LPT）”查看是否成功。

3. 备份设备固件，保存为 bin 格式：
   - 打开 Miko，（文件太大，我放在网盘里面了）按照图示流程备份您的随身WiFi。备份默认bin格式就可以。
    <p align="center">
   <img src="img/image-1.jpg" style="max-width: 80%;" alt="设备备份示意图">
   </p>

## 刷机步骤
1. 在网盘下载固件，并将下载的固件放在一个英文目录中。
2. 进入 9008 模式。
3. 打开 Qualcomm Premium Tool，记住一定要注册，查看流程：注册机-注册机使用教程.txt
4. 先读取设备分区，选择boot分区点写入，在选择system分区，在点写入。
5. 记住选择还原分区不要选错，不然会变砖。
   <p align="center">
   <img src="img/image-6.png" style="max-width: 80%;" alt="设备备份示意图">
   </p>

## 常见问题
- **（Miko Service Tool）和（Qualcomm Premium Tool）提示：fail**
  1. 主要原因是 9008 被占用，需要重新插拔数据库或更换 USB 接口。
  2. 如果更换数据线、插拔 USB 口后仍然不行，可能是系统问题。我的笔记本因系统不兼容，折腾了很久，最后重装系统。如果无法解决，可以去网吧或借用朋友的电脑。我使用的是 Windows 10 64 位专业版。
  3. 如果更换后仍然不行，可能是电脑硬件问题。大部分情况下更换硬件后会成功。
  **9008怎么都进不去**
  1. 先检查驱动，是否正确安装。
  2. 换数据线或者镊子，或者换电脑。
  3. 用镊子按住主板上的两个小圆点，然后插上USB，数到3，即可进入9008。

## OpenWRT 和 Debian
使用了多个版本的 OpenWRT，调试解调器时提示失败，尝试更换各种文件仍然无效。待有新固件时，我会上传，目前没有支持的好用版本，只能耐心等待，时间有限，无法继续折腾。