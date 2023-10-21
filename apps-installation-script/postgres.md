## Postgresql in Linux mint   

> Uninstall Postgres
 
**`sudo apt remove postgresql postgresql-contrib`**  

If, you wana purge remove postgres  
**`sudo apt-get -purge remove postgresql postgresql-14 postgresql-client-common postgresql-common postgresql-contrib`**  
then autoremove that are no longer needed ...   
```
sudo apt autoremove
```
<hr>     

> List all postgres packages    
```
dpkg -l |grep postgres
```   

### Installation    

```
sudo apt install postgresql postgresql-contrib
```
<hr>  

Enable Postgres:  
`sudo systemctl enable postgresql`    
Disable Postgres:  
`sudo systemctl disable postgresql`   
Check Status:  
`sudo systemctl status postgresql`     

-> **to get the pid info**    
```
ps -ef |grep postgres
```
if you don't get any pid info, that means the postgres is not running ...   

> Connect to postgres
```
sudo su - postgres
```
then type `psql` to run the cli.    


## Postgresql Cli Commands   


