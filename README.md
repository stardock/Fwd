# fwd
Firewall setup for Centos7


firewall-cmd --zone=public --permanent --add-port=80/tcp  
firewall-cmd --zone=public --permanent --add-port=888/tcp  
firewall-cmd --zone=public --permanent --add-port=8888/tcp  
firewall-cmd --zone=public --permanent --add-port=400-500/tcp  
firewall-cmd --zone=public --permanent --add-port=400-500/udp  
firewall-cmd --zone=public --permanent --add-port=10443/tcp  
firewall-cmd --zone=public --permanent --add-port=10443/udp  
firewall-cmd --zone=public --permanent --add-port=1000-5000/tcp  
firewall-cmd --permanent --add-masquerade  
firewall-cmd --reload  
firewall-cmd --zone=public --list-all  

echo "net.ipv4.ip_forward=1" >> /etc/sysctl.conf  

