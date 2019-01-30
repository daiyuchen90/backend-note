
####  一、查看端口
-   netstat -anp           //查询已开放的端口
-   firewall-cmd --query-port=3306/tcp         //查询指定端口是否已开 
-   firewall-cmd --zone=public --list-ports

####  二、简单介绍systemctl命令的使用
-   systemctl list-unit-files --type service   //查看全部服务命令
-   systemctl status name.service       //查看服务命令
-   systemctl start name.service        //启动服务
-   systemctl stop name.service         //停止服务
-   systemctl restart name.service      //重启服务
-   systemctl enable name.service       //增加开机启动
-   systemctl disable name.service      //删除开机启动

-  添加端口进防火墙： firewall-cmd --zone=public --add-port=3306/tcp --permanent
-  启动/重启/停止服务： systemctl start/restart/stop name.service
-  查看服务状态：  systemctl status name.service




    