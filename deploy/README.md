# deploy

TerraformでS3バケットをwww公開する。
S3にコンテンツも流し込む。

## デプロイ

このディレクトリで

```bash
terraform init
terraform apply
```

でS3バケットを作成し、'../app1/dist-gz` の中身を流し込む。

その際
各S3オブジェクトには
- Etag
- Content-Type
- Content-Encoding

を自動で設定する。

無事完了したら
output の s3wwwurl か objecturl にWWWブラウザでアクセスしてください。


## TODO

CloudFrontを介した場合、gzipされたデータがちゃんと動くかチェックすること。
