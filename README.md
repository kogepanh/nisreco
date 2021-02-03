# NISLAB 議事録作成アプリ

## Issue の立て方

1. 「New Issue」から Issue を立てる

## 開発までの準備

1. Issue の Assignees から自分を選択する
2. Develop ブランチにいるかを確認する
3. `git pull origin develop`で pull する
4. `git checkout -b feature/#(チケット番号)`でブランチを切り，開発開始

## 開発中の手順

### コミットに関して

`git commit -m "#(チケット番号) XXXX"`でコミットする

### Issue の引継ぎ

1. 他の人に引き継ぐ場合は，Push した上で，その上で Issue にコメントを残す
2. 引き継いで作業する場合は，Issue の Assignees に自分を選択する
3. Develop ブランチにいるかを確認する
4. `git fetch origin feature/#(チケット番号)`で fetch する
5. `git checkout feature/#(チケット番号)`でブランチを移動し，作業開始

## 開発後の手順

1. GitHub で pull_request する
2. メッセージは「Close #(チケット番号)」
3. 1 人のレビューが必要で、レビュワーがマージ・ブランチの削除・Issue の Close を行う

---

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
