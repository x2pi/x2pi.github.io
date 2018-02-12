---
layout: post
creationdate:  2018-02-05 00:00:00 +0700
title: Lỗi bảo mật web phổ biến
permalink: /book/tutorial/security/basic-model
author: PI
date: 2018-02-05 00:00:00 +0700
---

Bài viết này mục đích đưa ra các ý tưởng cơ bản về một số lỗi bảo mật web phổ biến. Nó sẽ giúp hiểu được một phần nào đó về các vấn đề an ninh phải đối mặt.

#### 1. Injection

Lỗi gây ra bởi việc xử lý một chuỗi đầu vào không hợp lệ khiến hệ thống thực hiện các hành vi mà kẻ tấn công có thể lợi dụng và khai thác nó.

Các lỗi thường tìm thấy trong các truy vẫn SQL, LDAP hoặc NoSQL, phân tích cú pháp XML... Nó rất dễ phát hiện có thể sử dụng các cộng cụ quét tự động hay fuzzers như SQLMap chẳng hạn để tìm ra lỗi.


Một số điều có thể giúp phòng tránh là xử lý chuỗi đầu vào cẩn thận. Có thể xử lý dữ liệu ở khách hàng bằng javascript nhưng làm việc đó ở máy chủ sẽ an toàn hơn. Sử dụng các API có sẵn vì nó thường tích hợp các tính năng để hạn chế lỗi injection.

#### 2. Xác thực bị hỏng

Lỗi gây ra bởi hệ thống xác thực và phiên bị hỏng. Và kẻ tấn công có thể giả mạo hoặc có được quyền truy cập của người khác.

Lỗi này khác phổ biến hầu hến các ứng dụng đều cần tính năng xác thực. Kẻ tấn công có thể phát hiện bằng phương pháp thủ công, hoặc sử dụng các công cụ tự động với danh sách mật khẩu hay các cuộc tấn công từ điển ([dictionary attack](https://en.wikipedia.org/wiki/Dictionary_attack)).

Cách hạn chế và ngăn chặn là: Nếu có thể hãy xác thực đa yếu tố, không sử dụ các tính năng xác thực mặc định đặc biệt là tài khoản người quản trị, không sử dụng các mật khẩu dễ đoán, giới hạn và trì hoãn khi nhiều lần đăng nhập không thành công.

#### 
