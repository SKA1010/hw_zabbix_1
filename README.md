# hw_zabbix_1

**Задание 1**

![image](https://user-images.githubusercontent.com/125235217/236620837-2245b7e6-0ceb-4804-abaf-9d67a59ab22b.png)


Текст команд:
sudo apt update
    5  su -
    
    6  sudo apt update
    
    7  sudo apt install postgresql postgresql-contrib
    
    8  sudo systemctl status postgresql
    
    9  wget https://repo.zabbix.com/zabbix/6.4/debian/pool/main/z/zabbix-release/zabbix-release_6.4-1+debian11_all.deb
   
   10  dpkg -i zabbix-release_6.4-1+debian11_all.deb
   
   11  sudo dpkg -i zabbix-release_6.4-1+debian11_all.deb
   
   12  sudo apt update
   
   13  sudo apt install zabbix-server-pgsql zabbix-frontend-php php7.4-pgsql zabbix-apache-conf zabbix-sql-scripts zabbix-agent
   
   14  sudo -u postgres createuser --pwprompt zabbix
   
   15  sudo -u postgres createdb -O zabbix zabbix
   
   16  zcat /usr/share/zabbix-sql-scripts/postgresql/server.sql.gz | sudo -u zabbix psql zabbix
   
   17  sudo nano /etc/zabbix/zabbix_server.conf
   
   18  sudo systemctl restart zabbix-server zabbix-agent apache2
   
   19  sudo systemctl enable zabbix-server zabbix-agent apache2
   
   
   **Задание 2**

![image](https://user-images.githubusercontent.com/125235217/236622509-214e72c7-dbab-4717-9357-2602da9a2a80.png)


![image](https://user-images.githubusercontent.com/125235217/236622733-4883dab9-3d31-40ba-9c55-2cdfa3936dcf.png)

![image](https://user-images.githubusercontent.com/125235217/236623459-7d370d63-d7f5-4c4b-8436-a4ba0ce9d40b.png)


Команды: 

       wget https://repo.zabbix.com/zabbix/6.4/debian/pool/main/z/zabbix-release/zabbix-release_6.4-1+debian10_all.deb
       
       dpkg -i zabbix-release_6.4-1+debian10_all.deb
       
       sudo dpkg -i zabbix-release_6.4-1+debian10_all.deb
       
       apt update
       
       sudo apt install zabbix-agent
       
       systemctl restart zabbix-agent
       
       systemctl enable zabbix-agent
