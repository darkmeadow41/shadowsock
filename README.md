# Easy install shadowsock client on Ubuntu 14.04 and above
# Shadowsocks-libev

---> Base

First we need to add repository:

    apt-get install software-properties-common -y
    add-apt-repository ppa:max-c-lv/shadowsocks-libev -y
    apt-get update
    apt install shadowsocks-libev -y

---> Working


# 
ss-server -s 0.0.0.0 -p 1133 -k password -m aes-256-cfb
