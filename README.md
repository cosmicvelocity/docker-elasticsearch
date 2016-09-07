# docker-elasticsearch

[elasticsearch](https://hub.docker.com/_/elasticsearch/) のバージョン 1.7.5 をカスタマイズしたものです。

- kuromoji プラグインを追加。

## 例

    $ docker run -v $(pwd)/data:/usr/share/elasticsearch/data -p 9200:9200 --name elasticsearch --rm cosmicvelocity/elasticsearch:1.7.5

## ドキュメント

### コンテナのビルド

    git clone https://github.com/cosmicvelocity/docker-elasticsearch.git
    cd docker-elasticsearch
    git checkout 1.7.5
    cd 1.7.5
    docker build -t cosmicvelocity/elasticsearch:1.7.5 .

### 実行

    $ docker run -v $(pwd)/data:/usr/share/elasticsearch/data -p 9200:9200 --name elasticsearch --rm cosmicvelocity/elasticsearch:1.7.5
