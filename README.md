## CordovaVueJS
Projeto base do Cordova com VueJs

# Instalar NodeJS:
  https://nodejs.org/

# Instalar Android Studio:
  https://developer.android.com/studio

# Instalar Java SDK:
  https://www.oracle.com/java/technologies/downloads/#java11-windows

# Instalar Gradle Binary (Descompactar em C:\Program Files\Gradle\{zip}):
  https://gradle.org/install/


# Variáveis de ambiente (Sistema):
  ANDROID_HOME
  C:\Users\{usuario}\AppData\Local\Android\Sdk
  ANDROID_SDK_ROOT
  C:\Users\{usuario}\AppData\Local\Android\Sdk
  JAVA_HOME
  C:\Program Files\Java\jdk-11.0.17
  Path
  C:\Program Files\Gradle\gradle-7.5.1\bin
  C:\Users\{usuario}\AppData\Local\Android\Sdk\tools
  C:\Users\{usuario}\AppData\Local\Android\Sdk\platform-tools
  C:\Program Files\Java\jdk-11.0.17\bin

---------------

# Android Studio:
  Instalar Android 10
  Instalar SDK Tools 30.0.3

---------------

# Comandos CMD:
  npm install -g cordova
  npm install -g vue-cli
  npm i -g @vue/cli-init

  cordova create MyApp
  vue init webpack MyApp

---------------

# O que fazer:
  Apagar os arquivos da pasta www

  Alterar o arquivo ./index.html (Trocar <HEAD>)
  <head> 
      <meta charset="utf-8"> 
      <meta name="format-detection" content="telephone=no"> 
      <meta name="msapplication-tap-highlight" content="no"> 
      <meta name="viewport" content="user-scalable=no, initial-scale=1, maximum-scale=1, Minimum-scale=1, width=device-width"> 
      <meta http-equiv="Content- Security-Policy" content="default-src 'self' data: gap: https://ssl.gstatic.com 'unsafe-eval'; style-src 'self' 'unsafe-inline'; media-src *; img -src 'self' data: content:; connect-src 'self' ws:;">
      <title>Nome do projeto</title> 
      <script src="cordova.js"></script> 
  </head>

# Alterar o arquivo ./config/index.js (trocar "dist" por "www")
build: {
  index: path.resolve(__dirname, ‘../www/index.html’),
  assetsRoot: path.resolve(__dirname, ‘../www’),
  ...
  
---------------

# Possíveis comandos de plataformas:
  cd MyApp
  cordova platform add windows
  cordova platform add browser
  cordova platform add android
  cordova platform add android@10.1.2
  cordova platform add android@6.xx —-save 
  cordova platform add ios --save

---------------

# Possíveis comandos de execução:
  npm run dev
  npm run build 
  cordova build android
  cordova build windows
  cordova build ios
  cordova run browser
  cordova emulate android


## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```