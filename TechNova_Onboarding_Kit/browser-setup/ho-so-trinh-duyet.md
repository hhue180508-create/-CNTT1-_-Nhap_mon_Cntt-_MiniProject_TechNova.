# Hồ sơ Trình duyệt TechNova

## 1. Hai Browser Profile độc lập

| Profile | Mục đích | Tài khoản |
|---|---|---|
| `Personal` | Mạng xã hội, email và dịch vụ cá nhân | Tài khoản cá nhân |
| `TechNova_Work` | Gmail công ty, Drive, GitHub, LMS và công cụ nội bộ | Tài khoản công việc |

Mỗi Profile có Cookies, Session, History, Bookmark và Extension riêng. Không dùng chung một Profile cho công việc và cá nhân. Khi dùng máy chung, luôn khóa máy hoặc đăng xuất theo quy định.

## 2. Bookmark Manager

Tạo ba thư mục Bookmark:

1. `01_Work_Dev`: GitHub, tài liệu ngôn ngữ/lập trình, DevTools.
2. `02_Onboarding_Docs`: quy trình nội bộ, tài liệu nhân sự, hướng dẫn bảo mật.
3. `03_Tools`: Google Drive, Lark/Slack, Bitwarden và công cụ được công ty phê duyệt.

Chỉ lưu liên kết đã kiểm tra nguồn và tên miền. Không lưu liên kết đăng nhập giả mạo.

## 3. Extension theo nhóm

| Nhóm | Ví dụ mục đích | Cấu hình |
|---|---|---|
| Dev Suite | JSON Viewer, công cụ kiểm tra màu | Chỉ cài từ cửa hàng chính thức |
| Productivity Suite | Công cụ ghi chú, quản lý tab | Chỉ giữ tiện ích thật sự cần |
| Security Suite | Tiện ích bảo mật được công ty phê duyệt | Kiểm tra nhà phát triển và quyền truy cập |

Đặt `Site access` ở `On click` nếu Extension hỗ trợ. Không cấp quyền đọc và thay đổi dữ liệu trên mọi trang nếu không cần. Gỡ Extension không còn sử dụng.

## 4. Thực hành DevTools F12

- `Inspect`: chọn phần tử giao diện và xem HTML/CSS; tránh sửa nội dung trên website thật khi chưa được phép.
- `Network`: xem yêu cầu tải tài nguyên, mã trạng thái và thời gian phản hồi.
- `Console`: đọc thông báo lỗi JavaScript; không dán lệnh lạ từ Internet vào Console.
- `Hard Reload`: tải lại tài nguyên để kiểm tra phiên bản mới, thường dùng `Ctrl + Shift + R` trên Windows.

## 5. Cache và Cookies

| Cache | Cookies |
|---|---|
| Lưu bản sao tài nguyên như ảnh, CSS, JavaScript để tải nhanh hơn | Lưu dữ liệu nhỏ liên quan phiên đăng nhập và tùy chọn |
| Có thể làm giao diện hiển thị bản cũ | Có thể duy trì phiên đăng nhập |
| Hard Reload giúp yêu cầu tải lại tài nguyên | Xóa Cookies có thể khiến phải đăng nhập lại |

**Quy trình khi giao diện chưa cập nhật:** kiểm tra kết nối → Hard Reload → kiểm tra Console/Network → thử Profile sạch nếu cần → ghi lại kết quả trước khi báo IT.
