# 403 Forbidden Errors on Centos Server

I was getting 403 errors from apache when trying to access a zip file. The file permissions and apache configuration looked correct. The issue was with SELinux running on the server. I followed this serverfault post to fix the issue. The other option would be to change SELinux to permissive.

[more info](http://serverfault.com/questions/650402/403-forbidden-errors-on-redhat-server)
