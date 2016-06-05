# supervisord
常用的监控配置存储

yum install supervisor python-pip -y
pip install supervisor==3.1
///////
下载并安装supervisor

wget http://pypi.python.org/packages/source/s/supervisor/supervisor-3.0b1.tar.gz
tar -zxvf supervisor-3.0b1.tar.gz
cd supervisor-3.0b1
python setup.py install
安装setuptools后也可以
easy_install supervisor
////
chkconfig supervisord on
wget https://raw.githubusercontent.com/wxliuxh/supervisord/master/supervisord -O /etc/init.d/supervisord
wget https://raw.githubusercontent.com/wxliuxh/supervisord/master/supervisord.conf -O /etc/supervisord.conf

chmod 755 /etc/init.d/supervisord

service supervisord start
