# DOCKER-COMMANDS

delete all containers : 
```
docker system prune
```

create macvlan :
```
docker network create -d macvlan --subnet=10.214.0.0/16 --gateway=10.214.255.254 --ip-range=10.214.2.64/26 -oparent=eno1 net-214-4
```

run the container : 
```
docker run --network=net-214-1  -v /home/test/bind :/etc/bind --dns=10.255.255.200\--name c-214-2-64 --hostname c-214-2-64 -it registry.iutbeziers.fr/debianiut bash
```
