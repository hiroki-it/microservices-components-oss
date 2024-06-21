# 遊び方

1. コンテナを起動する

```bash
$ docker-compose up -d
```

2. Keycloakにログインする。

3. クライアントを作成する。クライアントIDは`oauth2-proxy`とする。

4. 作成したクライアントから、クライアントシークレットを取得する。

5. oauth2-proxyコンテナのクライアントシークレット変数を設定する。

> - https://github.com/oauth2-proxy/oauth2-proxy/tree/master/contrib/local-environment
