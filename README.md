## Install

##[Docker Engine](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04-ru)

Steps:

1. sudo apt update
2. sudo apt install apt-transport-https ca-certificates curl software-properties-common
3. curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
4. sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
5. sudo apt update
6. apt-cache policy docker-ce
7. sudo apt install docker-ce
8. sudo systemctl status docker

## Do not forget about Git-Submodule
- git submodule init
- git submodule update

## Docker-Compose
1. sudo apt  install docker-compose

 - sudo chown $USER /var/run/docker.sock - turn off sudo
 - docker-compose build - Build 
 - docker-compose up - run container
 
### Start Postgres
docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres\
[more details](https://hub.docker.com/_/postgres)


### Create database mytest

### Useful commands
docker ps\
docker exec -it <key> bash\
psql -U postgres\
createuser --interactive --pwprompt


#### open http://localhost:3000/test to test
