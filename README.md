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
### References
* https://geth.ethereum.org/install/#run-inside-docker-container
