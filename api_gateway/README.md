# 遊び方

1. コンテナを起動する。

```bash
$ docker-compose up -d
```

2. JWTを`Authorization`ヘッダーに割り当てて、Nginx (API Gateway) にリクエストを送信する。

```bash
$ curl https://localhost/tea -H "Authorization: CSlkjdfj3423lkj234jj==" -k
> Your Coffee has been served by - 64ab8788dfbb
```

```bash
$ curl https://localhost/tea -H "Authorization: CSlkjdfj3423lkj234jj==" -k
> Your Coffee has been served by - 64ab8788dfbb
```

```bash
$ curl https://localhost/tea -H "Authorization: CSlkjdfj3423lkj234jj==" -k
> Your Coffee has been served by - 64ab8788dfbb
```

以下の機能を持つAPI Gatewayである。

- 通信の暗号化
- 認証
- `L7`ロードバランシング

> - https://github.com/Pungyeon/docker-nginx-example

