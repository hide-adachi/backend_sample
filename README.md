# backend_sample

cloneしてからdevcontainerで開発して下さい


# devcontainer
https://code.visualstudio.com/docs/devcontainers/containers

※↑読まなくても、
1. VS Codeの拡張機能より、【.devcontainer】を追加
2. 左下の><みたいなアイコンから【Reopen in Container】
3. 立ち上がったらAPIも実行できます

# (yarn) command
コマンド周りは【package.json】を見て下さい

# API
```
http://localhost:3000/api/v1/samples
```

# あえて省いた事
(弄ってみると良いと思う事)
* CI/CD
  * GitHub Actionsがオススメ
* 環境差分の吸収
  * .envだとセキュリティリスクの観点からソースコード管理しづらいですよね？どうしたらいいと思いますか？
* 認証周り
* DB構築
  * MYSQLのコンテナ積み込んだり、
    * https://hub.docker.com/_/mysql
  * docker-entrypoint-initdb.dで色々初期化したり
  * マイグレーションしたり、
  * APIと疎通したり、
  * APIから利用したり、
  * テストコードに利用したり
* キャッシュ構築
  * Valkeyのコンテナ積み込んだり、
  * APIと疎通したり、
  * APIから利用したり、
  
