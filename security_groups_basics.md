security groups basics 

secruity group is a virtual firewall

1 instance can have multiple security groups 
first line of defense 

lock down ssh to ip address


ssh and security up dates 
hello cloud gurus 

play with security groups 
wait for ec2 instance to provision 

copy and paste public ip address 

ssh -i <public pem file> ec2-user@<public ip address>

elevate priviledges of current user 
sudo su 

apply all updates 
sudo yum update 

updating all security patches 

install apache web server  
yum install httpd -y

start the apache server 
service httpd start 

start automatically when booting ec2 

chkconfig httpd on 

cd /var/www/html

<html>
    <h1>
        Hello Cloud Gurus!
    </h1>
</html>

create an index.html file 

go to security groups click on the webdmz security group 

description 

inbound rules 

outbound rules 

no tags 

deleting the inbound rules 

deleting is effective immediately 

inbound rule does not need an outbound rule 

anything added in will be allowed out 

access control lists need inbound and outbound 
 
you can't deny traffic 
you can only allow 

associate multiple security groups with an ec2 instance 

rdp 
mysql and aurora

allow them in for all traffic 

go back to instances 

add new security group 

remove webdmz 
add default 

you can chanve security groups 

cant deny anything in a security groups 
    there will not be any conflicts 

just adds up all the rules 
