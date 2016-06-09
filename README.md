# supervisord
常用的监控配置存储

----------SS监控
wget https://raw.githubusercontent.com/wxliuxh/supervisord/master/jk -O /root/jk

chmod 755 /root/jk

nohup /root/jk >/dev/null 2>&1 &

加入开机启动
echo 'nohup /root/jk >/dev/null 2>&1 &' >> /etc/rc.local

查看内容
cat /etc/rc.local
----------SS监控end
