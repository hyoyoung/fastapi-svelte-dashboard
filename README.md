# fastapi-svelte-dashboard
templates of fastapi with svelte admin dashboard - ([Norus](https://github.com/creativetimofficial/notus-svelte) by Creative Tim)

## Using
- fastapi
- pydantic
- sqlalchemy
- uvicorn
- pyjwt
- pymysql
- svelte
- rollup
- tailwind css
- fortawesome
- chartjs

## Quick Start
### build svelte dashboard
build files are in admin-app/public/build
```bash
cd admin-app
yarn install
yarn build
yarn build:tailwind
yarn build:fontawesome
cd ..
```

run backend api with docker
```bash
docker build -f Dockerfile.local -t fastapi-svelte .
docker run -t --rm --name fastapi-svelte -p 8080:80 -v `pwd`:/code --link mysql:fastapidb -e env="local" fastapi-svelte
```
