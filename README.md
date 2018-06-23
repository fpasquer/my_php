# my_php
docker php env

## setup the virtual machine
	1 Share with the virtual machine a folder called http with inside your website
	2 connect to your virtual machine with SSH
		3 sudo touch '/var/lib/boot2docker/bootlocal.sh'
		4 sudo chmod +x '/var/lib/boot2docker/bootlocal.sh'
		5 sudo vi '/var/lib/boot2docker/bootlocal.sh
			mkdir /var/http
			mount -t vboxsf http /var/http
			echo 'cd /var/http' >> /home/docker/.ashrc
		6 exit
	7 restart the virtual machine
	8 get your virtual machine ip

## docker-compose
	1 go to path/to/my_php
	2 docker-compose build
	3 docker-compose up
	4 open a brother tape your ip

## info
	To access at phpmyadmin your_ip:8080 in your brother
	db_table	: database_dev
	db_pass		: yonDTotHOMYkTqHA
	db_user		: fpasquer

## options
	In the file .env you can setup the config for phpmyadmin
