# AWS Lambda for Python3

> Serverless(ApiGateway + Lambda)

## 説明

AWS Lambdaをはじめれる環境だけを用意します

## 必須環境

* [Docker](https://www.docker.com/) をインストール済み

## セットアップ

1. クレデンシャル情報を設置

    ```bash
    cp -a .env.example .env
    vim .env

    以下を書き換えます
    AWS_ACCESS_KEY_ID=XXXXXXXXXXXXXXXXXXXX
    AWS_SECRET_ACCESS_KEY=YYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYY
    ```

2. Dockerイメージの作成

    ```bash
    docker-compose build
    ```

3. Dockerコンテナの起動と接続

    ```bash
    docker-compose up -d
    docker-compose exec app bash
    ```

## Author

* acronhub(https://github.com/acronhub)

## ライセンス

[MIT license](https://en.wikipedia.org/wiki/MIT_License).