#this is a sample docker for testapp front end
from centos:7
maintainer rprajyoth@gmail.com
run yum -y update
run yum -y install httpd
#copy code/* /var/www/html
add code /var/www/html
env BACKENDLB=test
expose 80
copy config/httpd-foreground /usr/bin
run chmod 755 /usr/bin/httpd-foreground
cmd ["httpd-foreground"]