# Upgrading curl on Centos 6.x

```
yum install epel-release -y
rpm -Uvh http://www.city-fan.org/ftp/contrib/yum-repo/rhel6/x86_64/city-fan.org-release-1-13.rhel6.noarch.rpm
yum --disablerepo="base" --enablerepo="city-fan.org" upgrade curl
```

This command did on not work: ``` yum update curl ```. I needed to disable the base repo otherwise it always returned nothing to update.
