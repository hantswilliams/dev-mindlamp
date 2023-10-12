# dev-mindlamp
a simple test environment file for docker mindlamp 

## instructions
- have modified the docker-compose to include traefik in it 
- have modified to remove swarm, this is just for testing purposes

## deployment
- when it first runs, it will generate a admin password that you will be able to see in the terminal, it will look something like:
```
server_1         |       ┌────────────────────────┬────────────────────────────────────────────────────────────────────┐
server_1         |       │        (index)         │                               Values                               │
server_1         |       ├────────────────────────┼────────────────────────────────────────────────────────────────────┤
server_1         |       │ Administrator Password │ '34b8b1................f6cd' │
server_1         |       └────────────────────────┴────────────────────────────────────────────────────────────────────┘

```
