# Nginx docker image builder.

## 1. build image
``` shell
docker build -t some-content-nginx:v1.0.0 .
```

## 2. run container
``` shell
# start a new container
docker run --name some-nginx -d some-content-nginx

# refer to a outer html folder.
docker run --name some-nginx -v /some/content:/usr/share/nginx/html:ro -d nginx

# exposing external port.
docker run --name some-nginx -d -p 8080:80 some-content-nginx

# complex config
docker run --name my-custom-nginx-container -v /host/path/nginx.conf:/etc/nginx/nginx.conf:ro -d nginx
``` 