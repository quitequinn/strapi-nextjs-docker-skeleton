# Strapi NextJs Docker Skelton
A simple guide for getting Docker, Strapi (with Postgres), and NextJS to play nice together.


## Requisites

### Docker
Install **Docker**.
(docs.docker.com/get-docker)[https://docs.docker.com/get-docker/]

### Node/NPM
Install **Node** and **NPM**, I recommend using **NVM** for this.
(github.com/nvm-sh/nvm)[https://github.com/nvm-sh/nvm]

### Yarn
Ya, install **Yarn**.
(classic.yarnpkg.com/en/docs/install)[https://classic.yarnpkg.com/en/docs/install]


## Template Setup 

Run each, one at a time, on root:
```bash 
yarn create strapi-app backend --quickstart
```
```bash 
yarn create next-app frontend
```
```bash 
mv Dockerfile-backend backend/Dockerfile
```
```bash 
mv Dockerfile-frontend frontend/Dockerfile
```


## Startup Prep

```bash
docker-compose pull
```


## Start Developing

Start dev server with docker-compose:
```bash
docker-compose up # updated recently? run `docker-compose build --no-cache`
```

**Frontend**: http://localhost:3000/

**Backend**: http://localhost:1337/

