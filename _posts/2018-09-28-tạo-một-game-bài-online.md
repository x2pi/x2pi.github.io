---
title: Tạo một game bài online
date: 2018-09-28 00:00:00 +0000
layout: post
creationdate: ''
tags:
- demo

---
Viết lại cho có chút động lực để làm cái demo. Demo này thực hiện một game bài tiến lên online đơn giản. Ứng dụng sử dụng nodejs, mongodb và các module javascript như vue, mongoose...thiếu cái nào thì cài thêm cái đó.

Tạo folder chứa dự án.

    mkdir thirteen
    cd thirteen

## Tạo client

### Khởi tạo dự án

Cài vue-cli.

    npm install --global vue-cli

Trong folder dự án **thirteen** khởi tạo folder **client** sẽ chứa mã chạy ở client.

    vue init vuetifyjs/webpack client

Chạy thử nó rồi mở tab browser  [localhost:8080]() xem kết quả.

    cd client
    npm run dev