# ethsetup
Ethereum SetUp

1. Run the following image:
```
docker run -d ethereum/client-go:latest
```

The TCP PORTS exposed for RPC will be 8545:

```
➜  ~ docker ps
CONTAINER ID        IMAGE                       COMMAND             CREATED              STATUS              PORTS                                       NAMES
f7f5169b0af8        ethereum/client-go:latest   "geth"              About a minute ago   Up About a minute   8545-8546/tcp, 30303/tcp, 30303-30304/udp   ecstatic_varahamihira
```

2. Connect to the shell to interact

```
docker exec -it <container name> /bin/sh
```

3. Connect to the already started "geth" process with **geth attach**:
```
# geth attach
Welcome to the Geth JavaScript console!

instance: Geth/v1.8.0-unstable-b4e05adc/linux-amd64/go1.9.3
 modules: admin:1.0 debug:1.0 eth:1.0 miner:1.0 net:1.0 personal:1.0 rpc:1.0 txpool:1.0 web3:1.0

>
### References
* https://geth.ethereum.org/install/#run-inside-docker-container
