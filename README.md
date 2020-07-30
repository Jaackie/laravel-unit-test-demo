## Docker开发环境
需要先将127.0.0.1 taobaoke.jq-docker.com加入本机Host

[详细文档](Docker.md)

## Demo
```$xslt
$ cp .env.example .env //修改配置

$ composer install --ignore-platform-reqs

$ docker-composer up -d 

$ docker exec -it unit.test bash

$ cd /www/unit.test

$ vendor/bin/phpunit --configuration phpunit.xml --colors  tests
```