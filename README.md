# aws-ami-codedeploy-rails

## 概要

CodeDeploy AgentとRuby(rbenv)をインストールしたAMIをPackerで作成します｡  
OSはAmazon Linux2です｡

## スクリプト

| ファイル名 | 説明                                      |
| ---------- | ----------------------------------------- |
| common.sh  | PKG最新化とCodeDeploy Agentのインストール |
| rbenv.sh   | rbenvのインストール                       |
| ruby.sh    | 指定したバージョンのrubyをインストール    |

## クイックガイド

環境変数にAWSの認証情報をセットした状態で実行します｡

### テスト

```
packer validate template.json
```

### デプロイ

```
packer build template.json
```