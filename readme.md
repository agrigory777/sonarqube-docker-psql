
## Ubuntu server

### Install docker

Help: https://phoenixnap.com/kb/how-to-install-docker-on-ubuntu-18-04

`sudo apt-get update`

`sudo apt-get remove docker docker-engine docker.io`

`sudo apt install docker.io`

check installation with `docker --version`

`sudo systemctl start docker`

`sudo systemctl enable docker`

### Install docker-compose

Help: https://phoenixnap.com/kb/install-docker-compose-ubuntu

Check the current release and if necessary, update it in the command below:
`sudo curl -L "https://github.com/docker/compose/releases/download/1.24.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose`

`sudo chmod +x /usr/local/bin/docker-compose`

`docker–compose –version`

