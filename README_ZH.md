<p align="center">
  <h1 align="center">jenkins持续集成工具</h1>
  <p align="center">
    <a href="README.md"><strong>English</strong></a> | <strong>简体中文</strong>
  </p>

## 目录

- [仓库简介](#项目介绍)
- [前置条件](#前置条件)
- [镜像说明](#镜像说明)
- [获取帮助](#获取帮助)
- [如何贡献](#如何贡献)

## 项目介绍
[jenkins](https://github.com/jenkinsci/jenkins) 是基于Java开发的一种持续集成工具，用于监控持续重复的工作，旨在提供一个开放易用的软件平台，使软件项目可以进行持续集成。

**核心功能：**
- **‌持续集成/持续交付（CI/CD）‌：** 自动化构建、测试和部署流程，支持多语言和工具链（如 Maven 、 Gradle 、 JUnit 等）。‌
- **插件生态系统‌：** 拥有超过1,500个插件，可扩展性极强，支持与 Docker 、 Kubernetes 等工具集成。‌
- **分布式构建‌：** 支持主从架构和多节点并行执行任务，有效利用计算资源。‌
- **可视化流程管理‌：** 通过 Groovy DSL定义的流水线（Pipeline）支持声明式和脚本式语法，可监控构建阶段并生成报告。‌

本项目提供的开源镜像商品 [**Jenkins**](https://marketplace.huaweicloud.com/contents/fc8e0589-9356-4a10-bc1a-1c4bd970a8bf#productid=OFFI1154255482317213696) ，已预先安装jenkins及其相关运行环境，并提供部署模板。快来参照使用指南，轻松开启“开箱即用”的高效体验吧。

> **系统要求如下：**
> - CPU: 2GHz 或更高
> - RAM: 4GB 或更大
> - Disk: 至少 40GB

## 前置条件
[注册华为账号并开通华为云](https://support.huaweicloud.com/usermanual-account/account_id_001.html)

## 镜像说明

| 镜像规格                                                                                                      | 特性说明                                           | 备注 |
|-----------------------------------------------------------------------------------------------------------|------------------------------------------------| --- |
| [jenkins-2.492.3-kunpeng](https://github.com/HuaweiCloudDeveloper/jenkins-image/tree/jenkins-2.492.3-kunpeng) | 基于 鲲鹏服务器 + Huawei Cloud EulerOS 2.0 64bit 安装部署 |  |

## 获取帮助
- 更多问题可通过 [issue](https://github.com/HuaweiCloudDeveloper/jenkins-image/issues) 或 华为云云商店指定商品的服务支持 与我们取得联系
- 其他开源镜像可看 [open-source-image-repos](https://github.com/HuaweiCloudDeveloper/open-source-image-repos)

## 如何贡献
- Fork 此存储库并提交合并请求
- 基于您的开源镜像信息同步更新 README.md
