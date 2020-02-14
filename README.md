# hello-js-demo
It's a very simple hello.js Oauth2 client demo 

## HTTPS for localhost
Since this demo is running in https, so it's better to have certificate with localhost, you can use `mkcert` to build your own.

1. Install mkcert
```shell
brew install mkcert
```
2. Use mkcert to generate certificate for localhost
```shell
mkcert -key-file key.pem -cert-file cert.pem 127.0.0.1
```

## Install dependecies in JavaScript
```shell
npm install http-server -g
npm install 
```

## Run the https server for testing
```shell
http-server -S -p 8080
```
