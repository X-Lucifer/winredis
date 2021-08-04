---
title: Windows Redis Server
created: '2021-08-04 19:00:00'
modified: '2021-08-05 02:33:00'
version: '6.2.5'
---

## Windows Redis Server
#### 说明:
> 从`Redis`官方源码中编译的`Windows`平台可用的`Redis Server`程序, 分别编译的版本为`cygwin`和`msys2`, 功能上无差别, 可任意选择. 可选择`exe`安装程序自动安装为Windows系统服务,或可配合nssm手动安装为Windows服务开机自启动. 方便Windows环境下Redis的调试和日常开发使用.

#### Windows平台其他版本Redis
1. `tporadowski / redis`
  > `地址`: [https://github.com/tporadowski/redis](https://github.com/tporadowski/redis)<br/>
  > `版本`: 5.0.10<br/>
  > `说明`:
  >> Native port of Redis for Windows. Redis is an in-memory database that persists on disk. The data model is key-value, but many different kind of values are supported: Strings, Lists, Sets, Sorted Sets, Hashes, Streams, HyperLogLogs. This repository contains unofficial port of Redis to Windows.

2. `microsoftarchive / redis`
  > `地址`: [https://github.com/microsoftarchive/redis](https://github.com/microsoftarchive/redis)<br/>
  > `版本`: 3.0.504<br/>
  > `说明`:
  >> Redis is an in-memory database that persists on disk. The data model is key-value, but many different kind of values are supported: Strings, Lists, Sets, Sorted Sets, Hashes.

### 安装为系统服务:
#### 第一种 (自动安装) , 推荐:+1::+1::+1::
<details open>
<summary>自动安装为系统服务</summary>
  
  >从[此处](https://github.com/X-Lucifer/winredis/releases)任意选择`.exe`后缀的可执行程序下载即可. `msys2`或`cygwin`版本功能无差别.
  
</details>

#### 第二种 (手动安装), 不推荐:-1::-1::-1::
<details>
  <summary>使用nssm手动安装redis为系统服务</summary>
  
  1. 从[此处](https://github.com/X-Lucifer/winredis/releases)任意选择`.tar`后缀的压缩包文件下载解压. `msys2`或`cygwin`版本功能无差别.<br/>
  2. 以`管理员身份`运行`cmd`或`powershell`, 并在当前目录执行以下命令:<br/>
  ```shell
  .\nssm install
  ```
  3. 打开服务安装窗体, 按图示设置好对应的参数, 点击`install service`按钮即可<br/>

  参考以下步骤:
  1. 第一步 ![第一步](./step/step_1.png)<br/>
  2. 第二步 ![第二步](./step/step_2.png)<br/>
  3. 第三步 ![第三步](./step/step_3.png)<br/>
  4. 第四步 ![第四步](./step/step_4.png)<br/>
  
</details>

#### 相关源码和其他软件
1. `Redis`源码: [https://github.com/redis/redis](https://github.com/redis/redis)
2. `Redis`官网: [https://redis.io](https://redis.io/)
3. `MSYS2`: [https://www.msys2.org/](https://www.msys2.org/)
4. `Cygwin`: [https://www.cygwin.com/](https://www.cygwin.com/)
5. `NSSM`: [https://www.nssm.cc/](https://www.nssm.cc/)



