


## Run

```bash
$ docker build -t nginx-basic .

$ docker run \
    --rm \
    --name nginx \
    -p 8080:80 \
    -p 8090:8090 \
    -e BASIC_AUTH_USERNAME=username \
    -e BASIC_AUTH_PASSWORD=password \
    -e PROXY_PASS=https://www.google.com \
    -e SERVER_NAME=basic_auth \
    -e PORT=80 \
    nginx-basic
```

