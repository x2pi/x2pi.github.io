---
title: Tạo một game bài online
date: 2018-09-28 00:00:00 +0000
layout: post
creationdate: ''
tags:
- demo

---
Viết lại cho có chút động lực để làm cái demo. Demo này thực hiện một game bài tiến lên online đơn giản. Ứng dụng sử dụng nodejs, mongodb và các module javascript như vue, mongoose...thiếu cái nào thì cài thêm cái đó.

### Tạo folder cho demo

Tạo folder đặt tên là thirteen chứa dự án bằng cách tạo new repository githu rồi clone về máy.

    git clone https://github.com/x2pi/thirteen.git

### Tạo nơi chứa mã client

Cài vue-cli.

```sh
npm install --global vue-cli
```

Trong folder dự án **thirteen** khởi tạo folder **client** sẽ chứa mã chạy ở client.

_.../thirteen_

    vue init vuetifyjs/webpack client

Với một số tùy chọn như sau:  
![](/uploads/vue-init.PNG)

Chạy thử nó kết quả xem tại [localhost:8080]().

.../thirteen

    cd client
    npm run dev

### Tạo nơi chữa mã server

Tạo folder server và khởi tạo npm

.../thirteen

    mkdir server
    cd server
    npm init -y

Sử dụng babeljs cho mã server

.../thirteen/server

    npm install @babel/core @babel/register --save-dev
    npm install --save-dev @babel/preset-env

Khởi tạo .babelrc, index.js và app.js

.../thirteen/server/.babelrc

    {
      "plugins": ["@babel/plugin-transform-modules-commonjs"]
    }

.../thirteen/server/index.js

    require("@babel/register");
    require('./app')

.../thirteen/server/app.js

    console.log(1)