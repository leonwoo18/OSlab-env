注：此setup.sh脚本为本人写的此项目所需安装环境（基于x86平台）
   由于本人最近把云服务器改为基于华为鲲鹏处理器（cpu为arm架构），所以该脚本需要更新，只能待有空的时候再更新了
   
   
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
如果想要跳过软件源更新步骤，请在./setup.sh后加上参数-s或-skip
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
