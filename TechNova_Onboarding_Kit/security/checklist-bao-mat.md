# Checklist An toàn thông tin TechNova

## 1. Password Manager

- Dùng Bitwarden làm kho quản lý mật khẩu theo chính sách công ty.
- Tạo mật khẩu riêng cho từng tài khoản, ưu tiên độ dài 16–32 ký tự theo yêu cầu bài tập và khả năng hỗ trợ của dịch vụ.
- Dùng Password Generator; không tái sử dụng mật khẩu.
- Bảo vệ Master Password, bật khóa kho và không chia sẻ tài khoản vault.
- Không lưu Master Password trong file `.env`, ghi chú công khai hoặc chat nhóm.

## 2. 2FA/TOTP

- Bật 2FA cho GitHub và email công ty.
- Ưu tiên ứng dụng Authenticator/TOTP khi dịch vụ hỗ trợ; SMS không nên là phương thức chính nếu có lựa chọn mạnh hơn.
- Lưu Backup Codes trong Bitwarden hoặc nơi lưu trữ được công ty phê duyệt.
- Không gửi mã OTP hoặc Backup Codes cho bất kỳ ai, kể cả người tự nhận là IT.
- Nếu mất thiết bị Authenticator, dùng quy trình khôi phục chính thức của dịch vụ và báo IT.

## 3. Nhận diện rủi ro

| Rủi ro | Dấu hiệu | Cách xử lý |
|---|---|---|
| Phishing | Email/tin nhắn thúc giục đăng nhập, đính kèm lạ | Không bấm link; tự mở website bằng Bookmark chính thức |
| Typosquatting | Tên miền gần giống tên thật, sai một ký tự | Kiểm tra kỹ tên miền trước khi nhập thông tin |
| Crack/Malware | Phần mềm bẻ khóa, yêu cầu tắt antivirus | Không cài; báo IT và dùng nguồn phần mềm hợp pháp |
| Social engineering | Người lạ xin mật khẩu/OTP/API key | Không cung cấp; xác minh qua kênh chính thức |

## 4. Quy tắc 5 KHÔNG

1. Không dùng chung một mật khẩu cho nhiều tài khoản.
2. Không chia sẻ mật khẩu, OTP, Backup Codes hoặc Master Password.
3. Không bấm link/đính kèm đáng ngờ.
4. Không cài phần mềm crack hoặc tiện ích không rõ nguồn.
5. Không đưa Secrets hoặc dữ liệu nội bộ lên nơi công khai hay Prompt AI.

## 5. Bảo vệ Secrets bằng .env và .gitignore

- `.env`: chứa cấu hình riêng của máy/môi trường; không commit lên Git.
- `.env.example`: chỉ chứa tên biến và giá trị mẫu không bí mật để đồng đội biết cần cấu hình gì.
- `.gitignore`: phải có `.env` trước commit đầu tiên.
- Không hardcode API Key, Password hoặc Token trong mã nguồn.

Ví dụ `.env.example`:

```dotenv
APP_ENV=development
API_BASE_URL=https://api.example.test
API_KEY=REPLACE_WITH_LOCAL_VALUE
```

Ví dụ `.gitignore`:

```gitignore
.env
.env.*
!.env.example
```

Giá trị trong ví dụ chỉ là placeholder. Không điền khóa thật vào tệp mẫu. Nếu Secrets đã bị commit, xóa khỏi file hiện tại chưa đủ; cần thu hồi/đổi khóa và làm theo quy trình xử lý sự cố của công ty.
