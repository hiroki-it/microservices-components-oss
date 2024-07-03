# 遊び方

1. パスワードを環境変数に設定する

```bash
$ brew install pwgen

$ echo SECRET_KEY=$(pwgen 64 1) >> .env
```

2. コンテナを起動する。

```bash
$ docker-compose up -d
```

> - https://github.com/grafana/oncall/tree/dev?tab=readme-ov-file#getting-started
