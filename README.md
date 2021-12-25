# scaleway-auto-start
首先下载星尘cil并初始化
``` bash
wget https://github.com/scaleway/scaleway-cli/releases/download/v2.4.0/scw-2.4.0-linux-x86_64
mv scw-2.4.0-linux-x86_64 /bin/scw
scw init
```
然后
``` bash
wget https://github.com/ours1505/scaleway-auto-start/blob/main/scw.sh
chmod 777 scw.sh
scw instance server list
vi scw.sh
```
使用vi 将***your-server-id***换为你的server-id <br> 
像这样 <br> 
![](https://aichatnew.oss-cn-shanghai.aliyuncs.com/chat/202112/1ae77958-ec5f-4b33-8356-a4203e3c9129.png)  <br> 
红色的复制到***your-server-id***，并删除***your-server-id*** <br> 
像这样 <br> 
![](https://aichatnew.oss-cn-shanghai.aliyuncs.com/chat/202112/c884704a-29d5-4645-b7b1-407ed7d811e5.png)  <br> 
然后运行
``` bash
screen scw.sh
```
让他自动刷一会即可，静止1天，就可开机当呈现running就OK啦
