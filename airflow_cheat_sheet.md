#whenever you are not able to find any application. In this case when i type airflow, I got a command not found.
#So i ran the following locate command and found the exact location where airflow was installed and then updated the path.

locate airflow | grep airflow$

airflow

echo $PATH

export PATH=$PATH:/home/bharati/.local/bin/

airflow

#Also i noticed that while installing some apps, they were unable to connect to some site.
#The reason is because i'm on ipv4 and the apps use ipv6. 
#To run the command successfully, i did the following

sudo apt-get -o Acquire::ForceIPv4=true install libmysqlclient-dev
