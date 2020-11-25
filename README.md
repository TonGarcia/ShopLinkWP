# ShopLinkWP
ShopLinkWP-Docker

# Credenciais
WordPress Clean Installation:
admin:
    user: user
    password: bitnami
    
# Docker Container access
```shell script
    $ docker exec -it --user root  container_id /bin/bash
```

# Backup container to dockerhub
```shell script
  $ docker commit container_id  iltongarcia/swp:latest && docker push iltongarcia/swp:latest 
  $ docker commit container_id  iltongarcia/swpdb:latest && docker push iltongarcia/swpdb:latest
```

# Install Docker on Ubuntu Server GCP
```shell script
    $ sudo apt install apt-transport-https ca-certificates curl software-properties-common
    $ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
    $ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic test"
    $ sudo apt update
    $ sudo apt install docker-ce
    $ sudo apt install docker-compose
```
