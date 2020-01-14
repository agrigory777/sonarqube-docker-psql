
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

If seeing error `max virtual memory areas vm.max_map_count [65530] is too low, increase to at least [262144]`
Increase it with: `sudo sysctl -w vm.max_map_count=262144`

### Run
`git clone https://github.com/agrigory1982/sonarqube-docker-psql.git`

`cd sonarqube-docker-psql`

`sudo docker-compose up`

### Help
Links:
https://www.azuredevopslabs.com/labs/vstsextend/sonarqube/
https://msftplayground.com/2019/02/combining-sonarqube-and-azure-devops/

