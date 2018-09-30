# dns-config
This is my DNS configuration for my test cluster on Fedora/CentOS

named-checkconf /etc/named.conf

named-checkzone majid.org /var/named/majid.org.zone
named-checkzone majid.org  /var/lib/named/
named-checkzone 50.168.192.in-addr.arpa /var/named/reverse.majid.org
