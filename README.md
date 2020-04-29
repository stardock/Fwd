# rc.local
old method

```  
touch /var/lock/subsys/local
mkdir /var/run/radiusd
chown radiusd:radiusd -R /var/run/radiusd
setcap CAP_NET_BIND_SERVICE=+eip  /usr/bin/python2.7
setcap CAP_NET_BIND_SERVICE=+eip  /usr/bin/python3.6
#iptables -I INPUT 1 -p tcp -m tcp --tcp-flags RST RST -j DROP
```  


```
#Ali
iptables -I INPUT -s 140.205.201.0/28 -j DROP
iptables -I INPUT -s 140.205.201.16/29 -j DROP
iptables -I INPUT -s 140.205.201.32/28 -j DROP
iptables -I INPUT -s 140.205.225.192/29 -j DROP
iptables -I INPUT -s 140.205.225.200/30 -j DROP
iptables -I INPUT -s 140.205.225.184/29 -j DROP
iptables -I INPUT -s 140.205.225.183/32 -j DROP
iptables -I INPUT -s 140.205.225.206/32 -j DROP
iptables -I INPUT -s 140.205.225.205/32 -j DROP
iptables -I INPUT -s 140.205.225.195/32 -j DROP
iptables -I INPUT -s 140.205.225.204/32 -j DROP
#Default
iptables -I INPUT -s 27.211.176.45 -j DROP
iptables -I INPUT -s 27.211.57.207 -j DROP
iptables -I INPUT -s 27.224.136.227 -j DROP
iptables -I INPUT -s 27.224.137.1 -j DROP
iptables -I INPUT -s 36.32.3.158 -j DROP
iptables -I INPUT -s 36.32.3.166 -j DROP
iptables -I INPUT -s 36.32.3.3 -j DROP
iptables -I INPUT -s 36.32.3.5 -j DROP
iptables -I INPUT -s 36.32.3.9 -j DROP
iptables -I INPUT -s 58.248.202.171 -j DROP
iptables -I INPUT -s 58.249.103.14 -j DROP
iptables -I INPUT -s 58.249.99.82 -j DROP
iptables -I INPUT -s 59.173.152.190 -j DROP
iptables -I INPUT -s 59.173.152.248 -j DROP
iptables -I INPUT -s 60.13.7.110 -j DROP
iptables -I INPUT -s 60.13.7.67 -j DROP
iptables -I INPUT -s 60.216.137.224 -j DROP
iptables -I INPUT -s 60.216.137.34 -j DROP
iptables -I INPUT -s 60.216.140.161 -j DROP
iptables -I INPUT -s 106.45.1.222 -j DROP
iptables -I INPUT -s 106.45.1.40 -j DROP
iptables -I INPUT -s 110.177.73.131 -j DROP
iptables -I INPUT -s 110.177.73.33 -j DROP
iptables -I INPUT -s 110.177.78.108 -j DROP
iptables -I INPUT -s 110.177.80.223 -j DROP
iptables -I INPUT -s 110.177.87.118 -j DROP
iptables -I INPUT -s 110.80.154.127 -j DROP
iptables -I INPUT -s 110.80.155.137 -j DROP
iptables -I INPUT -s 110.80.155.189 -j DROP
iptables -I INPUT -s 110.80.155.19 -j DROP
iptables -I INPUT -s 111.175.58.137 -j DROP
iptables -I INPUT -s 111.224.218.113 -j DROP
iptables -I INPUT -s 111.224.235.241 -j DROP
iptables -I INPUT -s 112.112.86.34 -j DROP
iptables -I INPUT -s 112.115.139.249 -j DROP
iptables -I INPUT -s 112.230.42.150 -j DROP
iptables -I INPUT -s 112.66.97.213 -j DROP
iptables -I INPUT -s 112.66.98.28 -j DROP
iptables -I INPUT -s 112.80.137.63 -j DROP
iptables -I INPUT -s 113.128.104.141 -j DROP
iptables -I INPUT -s 113.128.104.196 -j DROP
iptables -I INPUT -s 113.128.105.135 -j DROP
iptables -I INPUT -s 113.128.105.205 -j DROP
iptables -I INPUT -s 113.128.105.43 -j DROP
iptables -I INPUT -s 113.128.105.58 -j DROP
iptables -I INPUT -s 113.24.86.42 -j DROP
iptables -I INPUT -s 113.58.224.28 -j DROP
iptables -I INPUT -s 113.58.247.230 -j DROP
iptables -I INPUT -s 114.221.127.123 -j DROP
iptables -I INPUT -s 115.200.234.35 -j DROP
iptables -I INPUT -s 116.252.0.177 -j DROP
iptables -I INPUT -s 116.252.0.188 -j DROP
iptables -I INPUT -s 118.81.226.91 -j DROP
iptables -I INPUT -s 119.118.31.188 -j DROP
iptables -I INPUT -s 119.39.46.189 -j DROP
iptables -I INPUT -s 119.39.46.236 -j DROP
iptables -I INPUT -s 119.39.47.4 -j DROP
iptables -I INPUT -s 119.96.105.178 -j DROP
iptables -I INPUT -s 121.57.225.140 -j DROP
iptables -I INPUT -s 121.57.230.234 -j DROP
iptables -I INPUT -s 122.96.128.132 -j DROP
iptables -I INPUT -s 122.96.73.23 -j DROP
iptables -I INPUT -s 123.138.72.195 -j DROP
iptables -I INPUT -s 123.138.79.110 -j DROP
iptables -I INPUT -s 123.145.5.56 -j DROP
iptables -I INPUT -s 123.157.193.199 -j DROP
iptables -I INPUT -s 123.160.232.64 -j DROP
iptables -I INPUT -s 123.160.235.79 -j DROP
iptables -I INPUT -s 123.163.114.25 -j DROP
iptables -I INPUT -s 123.191.140.143 -j DROP
iptables -I INPUT -s 124.225.41.121 -j DROP
iptables -I INPUT -s 124.235.138.154 -j DROP
iptables -I INPUT -s 124.235.138.161 -j DROP
iptables -I INPUT -s 124.89.90.52 -j DROP
iptables -I INPUT -s 124.90.48.49 -j DROP
iptables -I INPUT -s 124.90.53.95 -j DROP
iptables -I INPUT -s 125.120.60.103 -j DROP
iptables -I INPUT -s 171.12.10.249 -j DROP
iptables -I INPUT -s 171.34.177.212 -j DROP
iptables -I INPUT -s 171.36.128.101 -j DROP
iptables -I INPUT -s 175.184.166.135 -j DROP
iptables -I INPUT -s 175.184.167.108 -j DROP
iptables -I INPUT -s 175.184.167.155 -j DROP
iptables -I INPUT -s 175.42.0.10 -j DROP
iptables -I INPUT -s 175.42.1.243 -j DROP
iptables -I INPUT -s 175.42.1.71 -j DROP
iptables -I INPUT -s 175.42.2.6 -j DROP
iptables -I INPUT -s 175.42.3.183 -j DROP
iptables -I INPUT -s 182.138.158.121 -j DROP
iptables -I INPUT -s 182.138.163.194 -j DROP
iptables -I INPUT -s 182.138.215.164 -j DROP
iptables -I INPUT -s 182.245.44.9 -j DROP
iptables -I INPUT -s 211.97.20.72 -j DROP
iptables -I INPUT -s 211.97.20.97 -j DROP
iptables -I INPUT -s 219.140.117.172 -j DROP
iptables -I INPUT -s 219.140.117.188 -j DROP
iptables -I INPUT -s 219.143.174.167 -j DROP
iptables -I INPUT -s 220.200.158.44 -j DROP
iptables -I INPUT -s 220.200.159.40 -j DROP
iptables -I INPUT -s 220.200.167.52 -j DROP
iptables -I INPUT -s 220.250.10.132 -j DROP
iptables -I INPUT -s 221.213.75.120 -j DROP
iptables -I INPUT -s 221.213.75.208 -j DROP
iptables -I INPUT -s 221.213.75.73 -j DROP
iptables -I INPUT -s 221.213.75.80 -j DROP
iptables -I INPUT -s 222.79.48.159 -j DROP
iptables -I INPUT -s 222.79.48.47 -j DROP
iptables -I INPUT -s 222.82.49.23 -j DROP
iptables -I INPUT -s 222.82.58.233 -j DROP
iptables -I INPUT -s 222.94.140.196 -j DROP
iptables -I INPUT -s 222.94.163.207 -j DROP
iptables -I INPUT -s 222.94.163.45 -j DROP
iptables -I INPUT -s 222.94.212.154 -j DROP
iptables -I INPUT -s 222.94.212.231 -j DROP
iptables -I INPUT -s 223.166.75.85 -j DROP
```  
