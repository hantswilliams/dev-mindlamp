# dev-mindlamp
a simple test environment file for docker mindlamp 

## instructions
- have modified the docker-compose to include traefik in it 
- have modified to remove swarm, this is just for testing purposes

## deployment
- Create a new network called public to connect all externally accessible services.
```bash
sudo docker network create --driver overlay --attachable public
```

Using your DNS provider of choice, provision a domain name (here we use example.com to represent your domain name and 1.1.1.1 to represent your node's IP address).

Replace administrator@example.com with your configuration variable.

Create a /data folder in the node that will be hosting the database.

```bash
mkdir -p /data/db
```

```bash
openssl rand -hex 8 # DB_PASSWORD_HERE
openssl rand -hex 32 # ROOT_ENCRYPTION_KEY_HERE
```


- when it first runs, it will generate a admin password that you will be able to see in the terminal, it will look something like:
```
server_1         |       ┌────────────────────────┬────────────────────────────────────────────────────────────────────┐
server_1         |       │        (index)         │                               Values                               │
server_1         |       ├────────────────────────┼────────────────────────────────────────────────────────────────────┤
server_1         |       │ Administrator Password │ '34b8b1................f6cd' │
server_1         |       └────────────────────────┴────────────────────────────────────────────────────────────────────┘

```

## api documentation issues 

- INSERT DOCUMENTATION HERE FOR ISSUES THAT YOU PREVIOUSLY FOUND 


## api notes for connecting 

- Example endpoint of how to connect: 
```python
import requests 

test_url = 'http://localhost:3000/api/v1/users/login'

test_data = {
    "username": "admin",
    "password": "34b8b1................f6cd"
}

```

## api notes for creating dummy data 


## api notes for pulling down dummy data 