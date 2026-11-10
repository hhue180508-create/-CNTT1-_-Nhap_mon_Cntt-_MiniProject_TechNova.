# TechNova Onboarding Kit

**Bộ hồ sơ nhập môn số dành cho nhân viên mới của Startup TechNova.**

## 1. Mục tiêu

Bộ hồ sơ hướng dẫn nhân viên mới tổ chức dữ liệu Local/Cloud, chia sẻ tài liệu đúng quyền, sử dụng trình duyệt nhiều Profile, bảo vệ tài khoản và tự tra cứu lỗi trước khi gửi yêu cầu hỗ trợ IT.

## 2. Mô hình Hybrid Workflow và Data Isolation

- **Local:** nơi nhân viên trực tiếp mở, chỉnh sửa và xử lý tệp.
- **Cloud:** nơi đồng bộ, sao lưu và cộng tác với đồng đội.
- **Data Isolation:** tách riêng dữ liệu cá nhân và công việc bằng thư mục, tài khoản và Browser Profile độc lập.

Không xem đồng bộ là bản sao lưu duy nhất. Với tài liệu quan trọng, cần có lịch sử phiên bản hoặc bản sao lưu riêng. Không lưu dữ liệu công ty trong tài khoản cá nhân nếu chưa được cho phép.

## 3. Cấu trúc thư mục 5 trụ cột

```text
technova-onboarding-kit/
├── docs/
│   ├── README.md
│   └── srs-onboarding-kit.docx
├── cloud-workspace/
│   └── phan-quyen-chia-se.md
├── browser-setup/
│   └── ho-so-trinh-duyet.md
├── security/
│   ├── checklist-bao-mat.md
│   ├── .env
│   ├── .env.example
│   └── .gitignore
└── troubleshooting/
    └── mau-bao-cao-loi.md
```

Tên thư mục và tệp dùng chữ thường, không dấu, không khoảng trắng; dùng dấu gạch nối `-` để phân tách từ.

## 4. Hướng dẫn bắt đầu

### Bước 1: Tạo không gian làm việc

Tạo thư mục gốc và các thư mục con bằng CMD tại thư mục muốn lưu dự án:

```bat
mkdir technova-onboarding-kit\docs technova-onboarding-kit\cloud-workspace technova-onboarding-kitrowser-setup technova-onboarding-kit\security technova-onboarding-kit	roubleshooting
```

### Bước 2: Thiết lập Cloud

Cài Google Drive for Desktop theo hướng dẫn chính thức của công ty, đăng nhập bằng tài khoản công việc và chọn thư mục cần đồng bộ. Kiểm tra trạng thái đồng bộ trước khi tắt máy.

### Bước 3: Thiết lập trình duyệt

Tạo hai Profile độc lập: `Personal` và `TechNova_Work`. Không đăng nhập tài khoản công ty trong Profile cá nhân.

### Bước 4: Bảo mật tài khoản

Dùng Password Manager, tạo mật khẩu riêng cho từng tài khoản và bật 2FA bằng ứng dụng Authenticator khi dịch vụ hỗ trợ. Lưu Backup Codes trong kho mật khẩu an toàn.

### Bước 5: Khi gặp lỗi

Làm theo thứ tự: đọc thông báo lỗi nguyên văn → kiểm tra phiên bản và môi trường → tìm tài liệu chính thức → tìm Stack Overflow/GitHub Issues → thử giải pháp an toàn → gửi Bug Report đủ thông tin nếu chưa xử lý được.

## 5. Checklist Onboarding

- [ ] Đã đăng nhập Cloud bằng tài khoản công việc.
- [ ] Đã tạo thư mục dự án theo cấu trúc thống nhất.
- [ ] Đã kiểm tra quyền Viewer/Commenter/Editor trước khi chia sẻ.
- [ ] Đã tạo Browser Profile Personal và TechNova_Work.
- [ ] Đã sắp xếp Bookmark theo nhóm công việc.
- [ ] Đã kiểm tra Extension và quyền Site Access.
- [ ] Đã thiết lập Password Manager và bật 2FA.
- [ ] Đã kiểm tra `.env` nằm trong `.gitignore`.
- [ ] Đã biết cách gửi Bug Report có Context, Expected, Actual và Log.

## 6. Bảng tài khoản và công cụ

| Công cụ | Mục đích | Nguyên tắc |
|---|---|---|
| Google Drive | Lưu trữ và cộng tác | Dùng tài khoản công ty, chia sẻ đúng quyền |
| Lark/Slack | Giao tiếp nhóm | Dùng Channel và Thread đúng chủ đề |
| Browser Profile | Tách phiên đăng nhập | Personal tách khỏi TechNova_Work |
| Bitwarden | Quản lý mật khẩu | Một tài khoản, một mật khẩu riêng |
| Authenticator | Tạo mã 2FA/TOTP | Bảo vệ thiết bị và Backup Codes |
| Git/GitHub | Quản lý mã nguồn | Không commit `.env` hoặc Secrets |

## 7. Quy tắc khi chia sẻ

Không cấp `Anyone with the link` kèm quyền Editor. Với đối tác bên ngoài, ưu tiên `Restricted` theo email và quyền Viewer; chỉ mở rộng quyền khi chủ sở hữu dữ liệu phê duyệt.

## 8. Quy tắc khi xử lý sự cố

Không gửi mật khẩu, API key, token hoặc dữ liệu cá nhân vào nhóm chat, diễn đàn hay Prompt AI. Che thông tin nhạy cảm trước khi chia sẻ ảnh chụp màn hình hoặc log.
