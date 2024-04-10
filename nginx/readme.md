# What is it

This part of the project holds the Nginx server config, and some additional files related to this (see the 502 error page?). 
Nginx acts as our reverse proxy server.

# How to server

login to our AWS server (you will need the ssh cert):

`ssh -i "chat-dungeon.pem" ubuntu@ec2-18-130-49-105.eu-west-2.compute.amazonaws.com`

Then there is `chat-dungeon` directory which holds this repo.

If you want to update Nginx:

`cd ~/chat-dungeon/nginx`

`git pull`

`sudo sh deploy_nginx_config.sh`