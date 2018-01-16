# vtalks documentation

Welcome to vtalks documentation!

* [Developer environment](development.md)
* [Production environment](production.md)

## Common recipes

### System cleanup

Docker cleanup, stop and remove containers and images:

```bash 
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
docker rmi $(docker images -q)
```

Remove all images with no associated container:

```bash
docker image prune -a
```
