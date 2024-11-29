# Backend Supporting Service - Software
- backend-docker-compose.yml contains redis, mongo, and nats
    - need to be sure to assign normal DNS names to the services in Dokploy so tath the API service can find them (e.g., mindlamp.redis, mindlamp.mongo, mindlamp.nats)

# Backend Supporting Service - API 
- backend-api-docker-compose.yml contains the backend API
    - might need to update this to ensure the naming convention is correct for the services in Dokploy that are reference in the other backend file

# Frontend Supporting - Dashboard
- Dockerfile from https://github.com/hantswilliams/LAMP-dashboard 

