# Firewall change to allow a docker container to connect to MySQL running on the host(centos machine).

Command to run on Centos to allow connectiosn to mysql from a docker container.

```
sudo firewall-cmd --zone=public --add-service=mysql --permanent
sudo firewall-cmd --reload
```

You also need to set the dockerhost IP as an environment variable for the docker container.

```
ifconfig | grep -E "([0-9]{1,3}\.){3}[0-9]{1,3}" | grep -v 127.0.0.1 | awk '{ print $2 }' | cut -f2 -d: | head -n1
```
