# supervisord
常用的监控配置存储

----------SS监控
````
wget https://raw.githubusercontent.com/wxliuxh/supervisord/master/jk -O /root/jk
chmod 755 /root/jk
nohup /root/jk >/dev/null 2>&1 &
````
加入开机启动
````
echo 'nohup /root/jk >/dev/null 2>&1 &' >> /etc/rc.local
````
查看内容
````
cat /etc/rc.local
````
----------SS监控end

----------kms
````
wget https://raw.githubusercontent.com/wxliuxh/supervisord/master/kms-server-x86 -O /usr/bin/kms-server --no-check-certificate
#wget https://raw.githubusercontent.com/wxliuxh/supervisord/master/kms-server-x64 -O /usr/bin/kms-server --no-check-certificate
chmod 755 /usr/bin/kms-server
/usr/bin/kms-server
````
加入开机启动
````
echo '/usr/bin/kms-server' >> /etc/rc.local
````
查看内容
````
cat /etc/rc.local
````
----------kms--end
https://forums.mydigitallife.info/threads/50234-Emulated-KMS-Servers-on-non-Windows-platforms
````
wget https://raw.githubusercontent.com/wxliuxh/supervisord/master/time.sh -O /root/time.sh
chmod 755 /root/time.sh
./time.sh
````
