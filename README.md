# caddy-docker
create a docker file for caddy php and mariadb
start command:
`sudo docker run -d -v /var/www/html:/srv -p 2015:2015 abiosoft/caddy:php`
DOC : 
```
https://hub.docker.com/r/itzg/minecraft-server/
```
little command for install my server :

sudo add-apt-repository -y ppa:webupd8team/java && sudo apt-get update && sudo apt-get install -y oracle-java8-installer && sudo apt install git && wget -q http://deb.opera.com/archive.key -O- | sudo apt-key add - && sudo apt-get update && sudo apt-get install opera && sudo apt-get install     apt-transport-https     ca-certificates     curl     software-properties-common && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository    "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable" && sudo apt-get update && sudo apt-get install docker-ce && git clone https://github.com/sorlinV/caddy-docker.git
