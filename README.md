# datasync ver 0.0.1

データ同期するツール
開発向け

- mysql
- 他 DB (postgress)
- data (file)

保存先

- s3 or google storage

Command Lists

datasync push # データ送信
datasync pull # データ受信
datasync apply # データ適用

設定ファイル名
datasync.yaml or datasync.yml

ファイル内容の例

```yaml
target:
  kind: mysql
  ...
upload:
  kind: s3
  ...
```

各種フレームワークに対しては、糖衣構文的な形で、config レスみたいな形にしたい。
```yaml
target:
kind: rails
```
