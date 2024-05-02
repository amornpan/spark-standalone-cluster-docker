# Apache Spark Standalone Cluster on Docker
## spark-standalone-cluster-docker

<p align="center"><img src="doc/image/cluster-architecture.png"></p>


# 1. ติดตั้ง Docker
### 1. update
sudo apt update

### 2. ติดตั้งเครื่องมือสำหรับการแสดงการใช้งานของแพ็กเกจผ่าน HTTPS:
sudo apt install apt-transport-https ca-certificates curl software-properties-common

### 3.เพิ่ม GPG key ของ Docker:
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

### 4. เพิ่ม Docker repository:
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

### 5. อัปเดตรายการแพ็กเกจอีกครั้ง:
sudo apt update

### 6. ติดตั้ง Docker:
sudo apt install docker-ce

### 7. ทดสอบการติดตั้ง Docker ด้วยการรันคำสั่ง:
sudo docker --version

# 2. ติดตั้ง Docker Compose
### 2.1 ดาวน์โหลด Docker Compose ด้วยคำสั่ง curl:
sudo curl -L "https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

### 2.2 ให้ Docker Compose เป็นไฟล์ที่ใช้งานได้:
sudo chmod +x /usr/local/bin/docker-compose

### 2.3 ทดสอบการติดตั้ง Docker Compose ด้วยการรันคำสั่ง:
docker-compose --version

sudo usermod -aG docker $USER


## How to use
$ curl -LO https://raw.githubusercontent.com/amornpan/spark-standalone-cluster-docker/master/docker-compose.yml


