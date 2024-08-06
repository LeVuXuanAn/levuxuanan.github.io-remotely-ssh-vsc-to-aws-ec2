## HƯỚNG DẪN KẾT NỐI VSCODE VỚI AWS EC2 BẰNG KẾT NỐI SSH
![](https://jimmydqv.com/assets/img/post-vscode-on-aws/vscode-on-aws-thumb.png)
Bài viết này sẽ giới thiệu cho bạn cách sử dụng 

## MỤC LỤC
1. [Giới thiệu kết nối SSH](##1.-giới-thiệu-kết-nối-ssh)
2. [Mục đích sử dụng SSH](##2.-mục-đích-sử-dụng-ssh)
3. [Giới thiệu Remote-SSH Extension trên VSCode]()
4. [Hướng dẫn khởi tạo Ubuntu EC2]()
5. [Hướng dẫn cấu hình kết nối VSCode với EC2]()

## 1. Giới thiệu kết nối SSH
- **SSH** (**Secure Shell**) là một giao thức mạng dùng để thiết lập kết nối mạng một cách bảo mật. SSH hoạt động ở lớp trên trong mô hình phân lớp TCP/IP. Các công cụ SSH (như OpenSSH) cung cấp cho người dùng cách thức để thiết lập kết nối mạng được mã hoá để tạo một kênh kết nối riêng tư.
- **SSH** tạo ra cơ chế xác thực qua mật khẩu mạnh, hình thành mối liên kết giao tiếp dữ liệu mã hóa ra giữa hai máy qua môi trường internet.
- Chức năng:
    - Hỗ trợ truy cập từ xa vào những hệ thống, thiết bị ứng dụng giao thức SSH.
    - Cho phép dịch chuyển file an toàn.
    - Thực thi lệnh bảo mật, an toàn trên hệ thống điều khiển từ xa.
    - Quản lý an toàn và hiệu quả thành phần hạ tầng mạng.

## 2. Mục đích sử dụng SSH
![](https://fptcloud.com/wp-content/uploads/2022/02/Mo-ta-co-che-hoat-dong-cua-SSH.jpg)
Mục đích SSH được tạo ra là để thay thế cho trình giả lập Terminal, cơ chế đăng nhập không an toàn (Telnet, Rlogin). Giao thức SSH hỗ trợ tính năng đăng nhập, khởi chạy Terminal Session thông qua hệ thống điều khiển từ xa.

Chức năng cơ bản nhất của giao thức SSH là liên kết với một host từ xa, ứng với một phiên Terminal bằng dòng lệnh "ssh server.example.org". Dòng lệnh này có thể liên kết Client với một máy chủ server.example.com thông qua ID người dùng UserName.

Trường hợp đó là lần kết nối đầu tiên giữa của Server và Host, người dùng phải được thông báo mã khóa của Host.



