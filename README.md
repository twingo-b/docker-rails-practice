# 参考
- [DockerでRails開発環境を作るワンライナー](http://qiita.com/masuidrive/items/7478fb9101652f2bbae1)
- [Rails(ActiveRecord)とMySQLでutf8mb4を扱う設定](http://qiita.com/xend/items/4d5c3333cbae53888f37)

# 前提条件
- Macでうごかしてます
    - [Docker Toolbox](https://www.docker.com/products/docker-toolbox)
    - [Getting Started with Docker for Mac](https://beta.docker.com/docs/mac/getting-started/)
- バージョン
```bash
% docker --version
Docker version 1.11.1, build 5604cbe

% docker-compose --version
docker-compose version 1.7.1, build 0a9ab35

# Docker for Mac
# Version 1.11.1-beta14 (build: 8670)
```

# 使い方
```bash
# clone
% git clone git@github.com:twingo-b/docker-rails-practice.git && cd docker-rails-practice

# setup & start
% docker-compose build
% docker-compose up -d
% docker-compose run rails ./bin/rake db:create
% docker-compose run rails ./bin/rake db:migrate

# see: http://localhost:3000

# stop
% docker-compose stop
```

