# Easy install shadowsock client on Ubuntu 14.04 and above
# Shadowsocks-libev

---> Base

  1. First we need to add repository:

         apt-get install software-properties-common -y
         add-apt-repository ppa:max-c-lv/shadowsocks-libev -y
         apt-get update
         apt install shadowsocks-libev -y
    
  2. Proxy SwitchyOmega extension to integrate proxy
  3. We must have working "config.json" file

---> Working

  To run shadowsock client you have to choose which best for you to run it:
  1. Type command on terminal every time like this
  
          ss-local -c /*PATHTOCONFIG*/.json
          
  2. Or just use ss command in terminal and its simpflified command as i personally like it. Let me breakdown step by step;
        - we must copy file ss to /usr/local/bin and dont forget chmod +x that file
        - we must have symlink /usr/local/bin to /home
        - we must have folder that contain "config.json" file
        
---> Integrate

  1. Be sure Proxy SwitchyOmega in extension installed
  2. Use this configuration
        scheme       (default)
        protocol     SOCKS5
        server       127.0.0.1
        port         1080

