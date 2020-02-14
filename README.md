# hello-js-demo
It's a very simple hello.js Oauth2 client demo 

## Preparation for Oauth2 in Facebook, Google
Go to facebook and google developer page, create a oauth2 application and get the client ID, replace `FACEBOOK_CLIENT_ID` and `GOOGLE_CLIENT_ID` in `index.html` 

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

After that, `cert.pem` and `key.pem` will be in your current folder

## Install dependecies in JavaScript
```shell
npm install http-server -g
npm install 
```

## Run the https server for testing
```shell
http-server -S -p 8080
```
It will get `cert.pem` and `key.pem` in your current folder to run https server.

And then you can see the page in `https://127.0.0.1:8080` 
