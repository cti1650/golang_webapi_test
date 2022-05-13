# A Golang CLI template on Gitpod

This is a [Golang CLI](https://golang.org) template configured for ephemeral development environments on [Gitpod](https://www.gitpod.io/).

## Next Steps

Click the button below to start a new development environment:

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/gitpod-io/template-golang-cli)

## Get Started With Your Own Project

### A new project

Click the above "Open in Gitpod" button to start a new workspace. Once you're ready to push your first code changes, Gitpod will guide you to fork this project so you own it.

### An existing project

To get started with Golang CLI on Gitpod, add a [`.gitpod.yml`](./.gitpod.yml) file which contains the configuration to improve the developer experience on Gitpod. To learn more, please see the [Getting Started](https://www.gitpod.io/docs/getting-started) documentation.



## 参考にしたサイト

- [Tutorial: Developing a RESTful API with Go and Gin - The Go Programming Language](https://go.dev/doc/tutorial/web-service-gin)  

### エンドポイント

- 一覧取得
```
curl http://localhost:8080/albums
```

- 要素追加
```
curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
```

- 抽出
```
curl http://localhost:8080/albums/2
```