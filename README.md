Wordpress Application using Docker
⦁	Create an EC2 instance in public subnet
⦁	Open custom ports 8080 for wordpress and 8181 for phpmyadmin in security grp.
⦁	Launch the instance
⦁	Sudo yum update
⦁	Install docker using:
sudo amazon-linux-extras install docker
⦁	Start docker:
systemctl start docker
⦁	Install python-pip
yum install python-pip
⦁	Install docker-compose:
pip3 install docker-compose
⦁	Create wordpress directory
⦁	Cd to wordpress
⦁	Create docker-compose.yml file and paste below content:
⦁	Start multiple containers
docker-compose up –d
⦁	Open <public-ip>:8080 in browser
⦁	Php can be opnened from 8181 port.

Issues:
The 4.4.1 version of wordpress has a bug hence it gives error while connecting to database. Hence explicitly specify the version of wordpress as 4.4 in docker-compose.yml file.
Extra docker commands:
To list running containers:
⦁	docker ps 
To stop container
⦁	docker stop <container-name>
To stop multiple containers:
⦁	docker-compose stop

 

 
