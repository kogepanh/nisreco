# NISLAB 議事録作成アプリ

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

## Use JSON-Server for Develop

```bash
# install global
yarn global add json-server

# check version
json-server -v

# run json-server
# json-server --watch [name].json --port [port]
json-server --watch db.json

# get http request
# curl -X GET http://localhost:[port]
curl -X GET http://localhost:3000/members

# post http request
# curl -X POST http://localhost:[port] -d '[param]'
curl -X POST http://localhost:3000/meetings/ -d 'id&team=N&writer=1'
```
