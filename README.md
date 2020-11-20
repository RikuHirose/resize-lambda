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
lambdaの環境変数を設定

```

DST_BUCKET sample-webapp
RESIZED_KEY files/streaming/
RESIZED_WIDTH  600
UPLOADED_KEY  files/original/


```

4. zipをlambdaのconsoleにupload