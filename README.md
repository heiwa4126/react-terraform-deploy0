# react-terraform-deploy0

Viteで作ったReactのアプリをAWS S3にTerraformでデプロイする。

おまけ機能として
.js, .css, .svg を gzip する。JavaScriptのgzipは体感できるくらい早くなる。

詳しい手順は 
- [app1/README.md](app1/README.md)
- [deploy/README.md](deploy/README.md)

を参照。

## いるもの

- [Node.js](https://nodejs.org/) (v18.12.1使用)
- [Terraform](https://www.terraform.io/) (v1.3.5使用)
- AWSアカウント。`aws sts get-caller-identity` などで確認。<br>設定されてない場合は [AWS CLI の設定 - AWS Command Line Interface](https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/cli-chap-configure.html) を参照。


## TODO

ディレクトリ構造をもっと考える。
deploy/をapp1/の下に置いたほうがいいかも。
