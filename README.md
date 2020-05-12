# httpd-basic-auth

Apache server to demonstrate basic authentication.

Example usage:

```
docker run -d \
    --name basic-auth \
    --env AUTH_USER=myusername \
    --env AUTH_PASS=mypassword \
    -v ${PWD}/index:/var/www \
    -p 8080:80 \
    sathed/httpd-basic-auth:latest
```

Build with:

```docker build -t <image>:<tag> .```
