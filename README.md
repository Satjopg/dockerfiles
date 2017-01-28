# dockerfiles
dockerイメージを作成するためのファイル群(バックアップ兼任)

# Requirements
* Docker version 1.13.0
* Docker compose version 1.10.0
* Docker machine version 0.9.0

# Usage
* Dockerhubを使わない例
* testディレクトリのDokerfileのコンテナを作る.
* image_nameとtag_nameは任意.  
(image_name:{username}/{imageの用途}, が分かりやすいかも)

以下コマンドを実施。(buildは時間かかる)
```
$ git clone https://github.com/Satjopg/dockerfiles/tree/master/test
$ cd ./test
$ docker build -t [image_name]:[tag_name]
```

コンテナの起動&ログイン(中に入る)
```
docker run -it [image_name]
```

# Future
* nodeの環境構築用イメージ(開発用は一応完成,外部公開等は未完)
* railsの環境構築用イメージ
