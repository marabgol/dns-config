# dns-config
This is my DNS configuration for my test cluster on Fedora/CentOS

named-checkconf /etc/named.conf

named-checkzone majid.org /var/named/majid.org.zone
named-checkzone majid.org  /var/lib/named/
named-checkzone 50.168.192.in-addr.arpa /var/named/reverse.majid.org


sudo firewall-cmd --permanent --add-port=53/tcp --zone=public
sudo firewall-cmd --permanent --add-port=53/tcp --zone=internal


# some firewall command

firewall-cmd  --add-service=dns-server –-permanent
firewall-cmd  –-permanent --add-service=dns-server
firewall-cmd  --add-service=dns-server
firewall-cmd  --list-all
firewall-cmd --permanent --zone=internal --add-service=dns
firewall-cmd --reload
