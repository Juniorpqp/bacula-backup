# You can use the commands to open ports on Linux and Windows:


# change ens160 for your ethernet 
# change IP_FROM with the Bacula IP Server

# Linux
ufw allow in on ens160 from IP_FROM to any port 9102

# Windows
netsh advfirewall firewall add rule name="Bacula Rule" dir=in action=allow protocol=TCP localport=9102 remoteip=IP_FROM
