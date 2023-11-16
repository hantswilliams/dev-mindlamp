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