## Lab no. 1
### Bitcoin node - regtest exercise

1. Download docker image:
```console 
docker pull nicolasdorier/docker-bitcoin:0.18.0
```

2. Create image instance: 
```console 
docker run -d --rm --name bitcoin nicolasdorier/docker-bitcoin:0.18.
```

3. Jump to container's bash:
```console 
docker exec -t -i bitcoin bash
```





