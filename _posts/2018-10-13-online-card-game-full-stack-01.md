---
title: Online card game full-stack 01
date: 2018-10-13 07:00:00 +07:00
tags:
- card game
- full-stack
- tutorial
layout: post
creationdate: ''
---

Viết cho có chút động lực để làm cái demo. Demo này thực hiện một game bài tiến lên online đơn giản. Ứng dụng sử dụng nodejs, mongodb và các module javascript như vue, mongoose...thiếu cái nào thì cài thêm cái đó.

### Tạo thư mục chứa dự án

Đơn giản đó là tạo một thư mục dự án với git. Tạo một kho github mình đặt tên là **vietnamese-cards** rồi clone về máy.

    git clone https://github.com/x2pi/vietnamese-cards.git

### Software sử dụng mô hình client–server

![](/uploads/client_server_architecture_model.jpg)

#### Khởi tạo mã client

Ta sử dụng vue and vuetify nên cần cài vue-cli.

    npm install --global vue-cli

Trong thư mục dự án **vietnamese-cards** khởi tạo thư mục **client** sẽ chứa mã chạy ở tất cả máy client.  
.../vietnamese-cards

    vue init vuetifyjs/webpack client

Với một số tùy chọn như sau:  
![](/uploads/vue-init.PNG)  
Chạy thử nó kết quả xem tại [localhost:8080](localhost:8080).  
.../vietnamese-cards

    cd client
    npm run dev

#### Khởi tạo mã sever

Tạo folder server và khởi tạo npm

.../vietnamese-cards

    mkdir server
    cd server
    npm init -y

Sử dụng babeljs cho mã server

.../vietnamese-cards/server

    npm install @babel/core @babel/register --save-dev
    npm install --save-dev @babel/preset-env

Tạo file .babelrc, index.js và app.js

.../vietnamese-cards/server/.babelrc

    {
      "plugins": ["@babel/plugin-transform-modules-commonjs"]
    }

.../vietnamese-cards/server/index.js

    require("@babel/register");
    require('./app')

.../vietnamese-cards/server/app.js

    console.log(1)

Có thể chạy thử sử dụng nodemon để tự động khởi động lại khi mã thay đổi.

Cài nodemon.

    npm install -g nodemon

Chạy thử  
.../vietnamese-cards/server

    nodemon index.js

### Kết quả

Ta có được khởi tạo cấu trúc software ban đầu một ứng dụng **client** chạy ở [localhost:8080](localhost:8080) hiểu thị một vuetify teamplate và **server** in ra số 1. Chỉ là khởi tạo ban đầu client và server chưa có liên kết tương tác gì với nhau. Thực hiện một commit cho khởi tạo này.

    git add .
    git commit -m 'Khởi tạo client và server'