# 参考
- [DockerでRails開発環境を作るワンライナー](http://qiita.com/masuidrive/items/7478fb9101652f2bbae1)
- [Rails(ActiveRecord)とMySQLでutf8mb4を扱う設定](http://qiita.com/xend/items/4d5c3333cbae53888f37)

# 使い方
```bash
# clone
git clone git@github.com:twingo-b/docker-rails-practice.git && cd docker-rails-practice

# setup & start
docker-compose build
docker-compose up -d
docker-compose run rails ./bin/rake db:create
docker-compose run rails ./bin/rake db:create RAILS_ENV=test

# see: http://localhost:3000

# stop
docker-compose stop
```

