
# Compose Test Swarm


```bash
docker swarm init --advertise-addr master.node.ip-addr

# run on master node, so it does not run containers
docker node update --availability drain manager-node

# run on worker node to register it on master
docker swarm join --token token.given.by.swarm.init.on.master.node


```

