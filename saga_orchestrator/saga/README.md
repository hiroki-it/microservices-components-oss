1. リポジトリをクローンする。

```bash
$ git clone https://github.com/temporalio/samples-go
```

2. temporalサーバーを起動する

```bash
$ docker-compose up -d
```

3. 別のターミナルで、temporalワーカーを実行する。

```bash
go run saga/worker/main.go
```

4. 別のターミナルで、temporalクライアントを実行する。

```bash
go run saga/start/main.go
```

> - https://github.com/temporalio/samples-go
