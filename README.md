# Strapi NextJs Skelton
A simple guide for getting Docker, Strapi, Postgres, and NextJS to play nice together.


# Requisites

## Docker
Install docker.
(https://docs.docker.com/get-docker/)[https://docs.docker.com/get-docker/]

## Node/NPM
Install Node and NPM, I recommend using NVM for this.
(https://github.com/nvm-sh/nvm)[https://github.com/nvm-sh/nvm]


# Template Setup 

Run below, one at a time, on root:
```bash 
yarn create strapi-app backend --quickstart
yarn create next-app frontend
mv Dockerfile-backend backend/Dockerfile
mv Dockerfile-frontend frontend/Dockerfile
```

# Startup Prep

```bash
docker-compose pull
```


# Start Developing

Start dev server with docker-compose:
```bash
docker-compose up # updated recently? run `docker-compose build --no-cache`
```

**Frontend**: http://localhost:3000/
**Backend**: http://localhost:1337/

