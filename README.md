# Generador PDF

REST webservice to convert the data coming from graph into PDF

## dependencies

* libreoffice
* coreutils (for the use of `timeout` changable by the configuration file when it will work)
* time (changable by the configuration file when it will work)
* [iron](https://github.com/iron/iron) / [params](https://github.com/iron/params) / [router](https://github.com/iron/router) / [staticfile](https://github.com/iron/static) / [mount](https://github.com/iron/mount)
* [fern](https://github.com/daboross/fern-rs) / log
* config

To generate the sample html form:

* node/iojs
* bower

## build the static form

From the project directory

``` shell
nvm use # if you use nvm to switch between different node/iojs versions
npm run setup
npm run jadec
```

## run the service

```shell
cargo run
```

`POST` the document to <http://localhost:3000/generator-pdf> by using a multipart/formdata request.

For an sample form `GET` <http://localhost:3000/generador-pdf/docNumber>
