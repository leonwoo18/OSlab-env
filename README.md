### 1.把此库克隆到linux主机上（以ubuntu18.04为例）
```shell
git clone https://github.com/leonwoo18/OSlab-env.git ~/oslab-env  
```
再把hit-oslab-linux-20110823.tar.gz（包含linux-0.11源码、bochs虚拟机等）移到用户目录下  </br>
```shell
cd ~/oslab-env 
mv hit-oslab-linux-20110823.tar.gz ~/  
```

### 2.解压hit-oslab-linux-20110823.tar.gz
```shell
tar -zxvf hit-oslab-linux-20110823.tar.gz  
```
解压后会放在~/oslab/目录下 
### 3.执行脚本，一步完成安装实验环境所需的东西
```shell
cd ~/oslab-env/   
chmod +x setup.sh   
./setup.sh   
```
### 4.编译linux-0.11
```shell
cd ~/oslab/linux-0.11/  
make all                
```
### 5.运行boch模拟器
```shell
cd ~/oslab/        
./run               
```
