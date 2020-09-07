# Минификация файлов сайта NetCat с использованием компилятора Webpack

Предполагается, что .css, .js файлы находятся в папке макетов дизайна, установлен менеджер пакетов npm.

Переходим в папку с макетом:
```
$ cd /netcat_template/template/<ID макета>
```

Генерируем и заполняем package.json:
```
$ npm init
```

Установка пакетов:
```
$ npm install -D webpack webpack-cli
$ npm install -D babel-loader @babel/core @babel/preset-env webpack
$ npm install -D clean-webpack-plugin
$ npm install -D css-loader
$ npm install -D file-loader
$ npm install -D html-webpack-plugin
$ npm install -D mini-css-extract-plugin
$ npm install -D optimize-css-assets-webpack-plugin
$ npm i -S jquery
```

Конфигурационый файл Webpack:
```
$ touch webpack.config.js
```

Файл с ресурсами:
```
$ touch index.js
```

Копируем родительский файл макета:
```
$ scp Template.html Template.copy.html
```

Запуск минификации на development или на production:
```
$ npm run dev
$ npm run prod
```