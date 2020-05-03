wget https://raw.githubusercontent.com/iyqfz/ssr/master/shadowsocksR.sh && bash shadowsocksR.sh && wget --no-check-certificate -O change_kernel.sh https://raw.githubusercontent.com/iyqfz/ssr/master/change_kernel.sh && bash change_kernel.sh
--------------------------------------------------------------重启后-----------------------------------------------------------------------
yum install net-tools -y && wget -N --no-check-certificate https://raw.githubusercontent.com/iyqfz/ssr/master/serverspeeder.sh && bash serverspeeder.sh


service serverSpeeder start #启动
service serverSpeeder stop #停止
service serverSpeeder reload #重新加载配置
service serverSpeeder restart #重启
service serverSpeeder status #状态
service serverSpeeder stats #统计
service serverSpeeder renewLic #更新许可文件
service serverSpeeder update #更新
chattr -i /serverspeeder/etc/apx* && /serverspeeder/bin/serverSpeeder.sh uninstall -f #卸载
