# Learn Terraform with AWS

詳しい説明は以下の記事を参照．

https://blog.chellwo.com/about-terraform

## 前提

Terraform（v1.3.5） と AWS CLI（v2.9.1） はインストール済みとする．

## 構成図

以下を構成する．

![AWS Structure](images/aws-640wri.png)

## AWSの環境変数の設定

aws-credentialsファイルを自分のAWSアカウントもしくはIAMに基づいて設定する．

```
export AWS_ACCESS_KEY_ID=YOUR_IAM_ACCESS_KEY_ID
export AWS_SECRET_ACCESS_KEY=YOUR_IAM_SECRET_KEY
```

### 環境変数の設定

```
source aws-credentials
```

## リソース作成

以下のコマンドを実行すればリソースが作成される．

```
terraform init
terraform apply
```
