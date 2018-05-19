# vtalks documentation

Welcome to vtalks documentation!

* [Developer environment](development.md)
* [Production environment](production.md)

## Common recipes

### System cleanup

Stop and remove all docker containers and images:

```bash 
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
docker rmi $(docker images -q)
```

Remove all docker volumes:

```bash
docker volume prune
```

Remove all docker images with no associated container:

```bash
docker image prune -a
```

### Create a new docker machine

```bash
docker-machine create \
    --driver generic \
    --generic-ip-address machine_ip \
    --generic-ssh-key ~/.ssh/id_rsa.pub \
    machine_name
```
