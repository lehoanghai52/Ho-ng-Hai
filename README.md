# HoangHai
# Hệ thống đăng nhập và quản lý ví điểm thưởng

## 1. Giới thiệu dự án
Dự án này là một hệ thống đăng nhập và quản lý tài khoản với ví điểm thưởng. Hệ thống cho phép:
- Người dùng đăng ký, đăng nhập và thay đổi thông tin cá nhân.
- Quản lý ví điểm thưởng, bao gồm chuyển điểm giữa các ví.
- Sử dụng bảo mật hai lớp (OTP) để xác thực các thay đổi quan trọng.
- Lưu trữ dữ liệu an toàn và hỗ trợ sao lưu.

## 2. Thành viên nhóm
| Họ và Tên | Công việc |
| Nguyễn Sỹ Thành Hưng | Quản lý hệ thống đăng nhập và đăng ký |
| Nguyễn Văn Hòa | Quản lý ví điểm thưởng và giao dịch |
| Trần Tăng Dương | Bảo mật OTP và xác thực |
| Lê Anh Hoàng Hai | Xử lý lưu trữ dữ liệu và sao lưu |

## 3. Đặc tả chức năng
### 3.1 Đăng ký và đăng nhập
- Người dùng có thể đăng ký tài khoản mới với tên đăng nhập và mật khẩu.
- Hệ thống hỗ trợ tạo mật khẩu tự động khi người dùng không cung cấp mật khẩu.
- Mật khẩu được mã hóa và lưu trữ an toàn.

### 3.2 Quản lý ví điểm thưởng
- Mỗi tài khoản có một ví điểm thưởng riêng.
- Người dùng có thể kiểm tra số dư, chuyển điểm sang ví khác.
- Các giao dịch được ghi nhận vào lịch sử.

### 3.3 OTP và bảo mật
- OTP được sử dụng để xác thực thay đổi thông tin quan trọng.
- Hệ thống gửi OTP qua email hoặc số điện thoại đăng ký.

### 3.4 Sao lưu và khôi phục dữ liệu
- Dữ liệu người dùng và giao dịch được lưu trữ trong file JSON hoặc database.
- Hệ thống có cơ chế sao lưu dữ liệu định kỳ.

## 4. Cách tải và cài đặt
### 4.1 Yêu cầu hệ thống
- Hệ điều hành: Windows/Linux/macOS
- Trình biên dịch: `g++`

### 4.2 Hướng dẫn cài đặt
```sh
# Clone repository
git clone <repo_url>
cd project_folder

# Biên dịch chương trình
g++ -o main src/*.cpp -std=c++17

# Chạy chương trình
./main
```

## 5. Cách sử dụng
1. Chạy chương trình và chọn chức năng trên menu.
2. Nhập thông tin đăng nhập hoặc đăng ký nếu chưa có tài khoản.
3. Nếu cần thay đổi thông tin hoặc thực hiện giao dịch, nhập mã OTP khi được yêu cầu.

## 6. Tham khảo
- [CPP_OTP](https://github.com/patzol768/cpp-otp)
- [COTP](https://github.com/tilkinsc/COTP)
- [ACID](https://200lab.io/blog/acid-la-gi/)

