<p align="center">
  <h1 align="center">Jenkins Continuous Integration Tool</h1>
  <p align="center">
    <strong>English</strong> | <a href="README_ZH.md">Simplified Chinese</a>
  </p>

## Table of Contents

- [Repository Introduction](#repository-introduction)
- [Prerequisites](#prerequisites)
- [Image Description](#image-description)
- [Getting Help](#getting-help)
- [How to Contribute](#how-to-contribute)

## Repository Introduction
[Jenkins](https://github.com/jenkinsci/jenkins) is a continuous integration tool developed in Java. It is used to monitor continuously repeated tasks and aims to provide an open and user - friendly software platform for software projects to implement continuous integration.

**Core Features:**
- **Continuous Integration/Continuous Delivery (CI/CD):** Automates the build, test, and deployment processes, supporting multiple languages and toolchains (such as Maven, Gradle, JUnit, etc.).
- **Plugin Ecosystem:** It has over 1,500 plugins, offering strong extensibility and supporting integration with tools like Docker and Kubernetes.
- **Distributed Build:** Supports the master - slave architecture and parallel task execution on multiple nodes, effectively utilizing computing resources.
- **Visual Process Management:** Supports both declarative and scripted syntax through Groovy DSL - defined pipelines (Pipeline), enabling monitoring of build stages and report generation.

The open - source image product [**Jenkins**]() provided by this project has Jenkins and its related runtime environment pre - installed, and deployment templates are also provided. Refer to the usage guide and easily start an "out - of - the - box" efficient experience!

> **System requirements are as follows:**
> - CPU: 2GHz or higher
> - RAM: 4GB or more
> - Disk: At least 40GB

## Prerequisites
[Register a Huawei account and activate Huawei Cloud](https://support.huaweicloud.com/usermanual-account/account_id_001.html)

## Image Description

| Image Specification                                                                                                      | Feature Description                                           | Remarks |
|-----------------------------------------------------------------------------------------------------------|------------------------------------------------| --- |
| [jenkins-2.492.3-kunpeng](https://github.com/HuaweiCloudDeveloper/jenkins-image/tree/jenkins-2.492.3-kunpeng) | Installed and deployed based on Kunpeng servers + Huawei Cloud EulerOS 2.0 64bit |  |

## Getting Help
- For more questions, you can contact us via [issue](https://github.com/HuaweiCloudDeveloper/jenkins-image/issues) or the service support of the specified product in the Huawei Cloud Marketplace.
- For other open - source images, refer to [open-source-image-repos](https://github.com/HuaweiCloudDeveloper/open-source-image-repos)

## How to Contribute
- Fork this repository and submit a merge request.
- Synchronously update README.md based on your open source image information.