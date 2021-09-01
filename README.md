# Go Playground
Go で色々書いたものを残していくレポジトリ

## Requirements
- docker

## 実行
```shell
docker-compose run --rm app <command> 
```
- テスト・フォーマット
```shell
docker-compose run --rm app go fmt ./...
docker-compose run --rm app go test ./... -v
```

- `main.go`の実行
```shell
make run
```
- すべてのテストの実行
```shell
make test_all
```
fileにパッケージの相対パスを指定することでそのパッケージのみのテストにできる。
```shell
# example
make test file=./coding/chapter1
```