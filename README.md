# ufw
Firewall setup for Ubuntu24 ufw

```  
ufw allow 80/tcp
ufw allow 888/tcp
ufw allow 887/tcp
ufw allow 8888/tcp
ufw allow 400:500/tcp
ufw allow 10443/tcp
ufw allow 10443/udp
ufw allow 1000:5000/tcp
ufw allow 1812:1814/tcp
ufw allow 1812:1814/udp
ufw allow 3389/tcp
ufw allow 8443/tcp
ufw allow 35601/tcp
```  

`ufw status`  

echo "net.ipv4.ip_forward=1" >> /etc/sysctl.conf  

