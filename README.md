### 1.把此库克隆到linux主机上（以ubuntu18.04为例）
```shell
git clone https://github.com/leonwoo18/OSlab-env.git ~/oslab-env  
```
再把hit-oslab-linux-20110823.tar.gz（包含linux-0.11源码、bochs虚拟机等）移到用户目录下  </br>
cd ~/oslab-env  </br>
mv hit-oslab-linux-20110823.tar.gz ~/   </br>


### 2.解压hit-oslab-linux-20110823.tar.gz
tar -zxvf hit-oslab-linux-20110823.tar.gz  </br>
解压后会放在 /home/用户/ 目录下的 oslab/   </br>

### 3.执行脚本，一步完成安装实验环境所需的东西
cd ~/oslab-env/   </br>
chmod +x setup.sh   </br>
./setup.sh    </br>

### 4.编译linux-0.11
cd ~/oslab/linux-0.11/  </br>
make all                 </br>

### 5.运行boch模拟器
cd ~/oslab/        </br>
./run               </br>
