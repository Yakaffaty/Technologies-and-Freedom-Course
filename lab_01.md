## Lab no. 1
### Bitcoin node - regtest exercise


1. Download docker image:
```console 
docker pull nicolasdorier/docker-bitcoin:0.16.0
```

2. Create image instance: 
```console 
docker run -d --rm --name bitcoin nicolasdorier/docker-bitcoin:0.16.0
```

3. Jump to container's bash:
```console 
docker exec -t -i bitcoin bash
```

4. Check everything's ok:
```console 
which bitcoind
```

```console 
which bitcoin-cli
```

5. Go to Bitcoin application directory:
```console 
cd home/bitcoin/.bitcoin
```

6. Edit bitcoin.conf:
```console 
nano bitcoin.conf
```

Basic .conf file:
```
daemon=1
txindex=1
rpcuser=yourusername
rpcpassword=astrongpassword
rpchost=http://127.0.0.1
rpcport=18443

# Run on the test network instead of the real bitcoin network.
#testnet=1
#regtest=1

debug=0
```


Resources:

* Official documentation [here](https://bitcoin.org/en/developer-examples).  
* Config file generator [here](https://jlopp.github.io/bitcoin-core-config-generator).