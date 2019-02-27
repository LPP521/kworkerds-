##  重复了一点没有关系，我的服务器每一分钟会新建一个挖矿进程，所以要在一分钟之内执行完毕 
##  其中开头的主机名称更换为自己的名称即可
##  有的地方如果root权限不够，要自己添加chattr修改权限，（一般不用）

``
ps aux|grep "iZkyo9knm39v08Z"|grep -v grep|awk '{print $2}'|xargs kill -9

chattr -i /etc/cron.d/root
 echo "" > /etc/cron.d/root
 echo "" > /etc/cron.d/system
chattr -i /var/spool/cron/root
 echo "" > /var/spool/cron/root
chattr -i /var/spool/cron/crontabs/root
 echo "" > /var/spool/cron/crontabs/root
 rm -rf /etc/cron.hourly/oanacrons
 rm -rf /etc/cron.daily/oanacron
 rm -rf /etc/cron.monthly/oanacron

 rm -rf /bin/httpdns
 sed -i '$d' /etc/crontab

 sed -i '$d' /etc/ld.so.preload
 rm -rf /usr/local/lib/libntp.so

 ps aux|grep kworkerds|grep -v color|awk '{print $2}'|xargs kill -9
 rm -rf /tmp/.tmph
 rm -rf /bin/kworkerds
 rm -rf /tmp/kworkerds
 rm -rf /usr/sbin/kworkerds
 rm -rf /etc/init.d/kworker

rm -rf /tmp/kworkerds
chattr -i /tmp/thisxxs
rm -rf /tmp/thisxxs

rm /tmp.*

 chkconfig --del kworker


echo "" > /etc/ld.so.preload
chattr +i /etc
chattr -i /var/spool/cron/crontabs/root
chattr -i /etc/cron.d/apache
chattr -i /etc/cron.d/root
chattr -i /var/spool/cron/root
chattr -i /usr/local/lib/libntpd.so
rm -rf /var/spool/cron/*
rm -rf /etc/cron.d/*
chattr +i /var/spool/cron/
rm -f /usr/local/lib/*
chattr +i /usr/local/lib
killall kworkerds
rm -f /var/tmp/kworkerds*
rm -f /var/tmp/1.so
rm -f /tmp/kworkerds*
rm -f /tmp/1.so
rm -f /var/tmp/wc.conf
rm -f tmp/wc.conf
``
