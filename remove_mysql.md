## steps to remove MySLQ from Ubuntu 18+


1. remove mysql-server mysql-client mysql-common   
`sudo apt remove --purge mysql-server mysql-client mysql-common -y`

2. remove automatically installed packages    
`sudo apt autoremove -y`   
`sudo apt autoclean`
3. remove MySQL configuration files   
`sudo apt-get remove dbconfig-mysql`

4. delete all MuSQL files on your machine   
`rm -rf /etc/mysql`   
`sudo find / -iname 'mysql*' -exec rm -rf {} \;`
