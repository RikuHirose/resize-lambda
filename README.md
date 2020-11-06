# resize-lambda

https://docs.aws.amazon.com/ja_jp/lambda/latest/dg/with-s3-example.html

1. こちらをgit clone 
https://github.com/RikuHirose/resize-lambda

2. 
```
zip -r function.zip .
```
を実行しzip fileにする


3. s3にて特定のkeyにuploadされたら、lambda関数がtriggerされるように設定

4. zipをlambdaのconsoleにupload
