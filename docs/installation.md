# jenkins部署指南

## ‌一、环境准备

### 一、更新系统

```bash
yum -y update  
yum -y upgrade
```

## ‌二、安装docker

参考：[安装Docker](https://support.huaweicloud.com/bestpractice-hce/hce_bp_0002.html)

## ‌三、安装jdk

#### 下载解压

```bash
# 下载
wget https://mirrors.tuna.tsinghua.edu.cn/Adoptium/17/jdk/aarch64/linux/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.11_9.tar.gz
# 创建安装目录
sudo mkdir -p /usr/lib/jvm
# 解压至目标目录
sudo tar -xzf OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.11_9.tar.gz -C /usr/lib/jvm/
# 重命名便于管理
sudo mv /usr/lib/jvm/jdk-17.0.11+9 /usr/lib/jvm/jdk-17
```

### 配置环境变量
```bash
vim /etc/profile
```

```xml
# 在文末加入
export JAVA_HOME=/usr/lib/jvm/jdk-17
export JRE_HOME=${JAVA_HOME}/jre
export CLASSPATH=.:${JAVA_HOME}/lib:${JRE_HOME}/lib
export PATH=${JAVA_HOME}/bin:$PATH
```

### 使环境变量生效
```bash
source /etc/profile
```

## 四、拉取镜像和创建容器

### 1.拉取镜像
```bash
docker pull jenkins/jenkins:2.492.3-lts-jdk17
```

### 2.宿主机创建jenkins用户和目录
```bash
sudo groupadd -g 1000 jenkins
sudo useradd -u 1000 -g jenkins -d /var/jenkins_home jenkins
sudo mkdir -p /var/jenkins_home
sudo chown -R jenkins:jenkins /var/jenkins_home

```

### 3.创建容器
```bash
docker run -d \
   --name jenkins \
   -p 8080:8080 -p 50000:50000 \
   -v /var/jenkins_home:/var/jenkins_home \
   -v /var/run/docker.sock:/var/run/docker.sock \
   -u jenkins:jenkins \
   --restart always \
   jenkins/jenkins:2.492.3-lts-jdk17
```