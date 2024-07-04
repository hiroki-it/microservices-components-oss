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

3. Grafanaダッシュボード (`localhost:3000`) にアクセスする。

4. GrafanaダッシュボードでOnCallプラグインをインストールする。

5. Grafanaダッシュボードで、OnCall APIのURLに`http://engine:8080`を入力し、GrafanaダッシュボードとOnCallを連携する。ポートが空いていないとエラーになる。

6. 画面をリロードし、初期化する。

7. OnCall > Settings > `GRAFANA_CLOUD_NOTIFICATIONS_ENABLED` を無効化する。

8. Grafana OnCallは、電話のコール機能にTwilioを使っているため、Twilioでアカウントの作成が必要である。これにより、自分の電話番号に対応する番号をTwilioが発行する。

9. Grafana OnCallで、ユーザーに自分の電話番号を設定し、ワンタイムパスワードで認証する。

10. Twilioの番号を介して、自分の電話番号にオンコールが届く。

> - https://github.com/grafana/oncall/tree/dev?tab=readme-ov-file#getting-started
> - https://qiita.com/yteraoka/items/7e6db7111a061f5e22e4
