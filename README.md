

Dockerfile build .

docker-compose run zerotest
docker-compose build

# To run test:

```bash
alias dc="docker-compose"

dc up # 1:1 client-server

dc up --scale client=3
```
