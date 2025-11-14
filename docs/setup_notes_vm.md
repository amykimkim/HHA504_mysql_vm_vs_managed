Ordered steps you executed, with command snippets
Any config files you edited (e.g., mysqld.cnf), with the exact lines
Troubles you hit and how you solved them
Start-to-finish elapsed time (minutes) measured by you

1. Provisioned a VM on Google Cloud Platform (GCP)
- Region: Iowa
- 2 vCPU and 4GB RAM

2. Opened up firewalls for port 22 and 3306 by adding firewall rules

3. Opened SSH and ran 
``` 
sudo apt-get update 
```
then
```
sudo apt install mysql-server mysql-client -y 
```
Then logged into mysql via ``` sudo mysql ```

4. Created a new user: amy, with a password, and granted privileges
``` 
GRANT ALL PRIVILEGES ON *.* TO 'dba'@'%' WITH GRANT
OPTION; 
```

5. Updated mySQL configuration settings to enable external connections
```
sudo nano /etc/mysql/mysql.conf.d/mysqld.cnf
```
and changed bind-address to 0.0.0.0 and saved. Next, I restarted SSH for the change to take effect.
```
/etc/init.d/mysql restart
``` 
6. Went into VS code to set up .py file to run and insert data. Ran into issues here when running the code given by professor Hants. 
