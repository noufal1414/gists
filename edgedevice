#!/bin/sh
#below line checks if crontab job for dnsmasq is available, if not adds it. 
if [cat /etc/crontabs/root | grep dnsmasq | wc -l == 0] ; then
    echo "*/2 * * * * /etc/init.d/dnsmasq restart" >> /etc/crontabs/root
fi
