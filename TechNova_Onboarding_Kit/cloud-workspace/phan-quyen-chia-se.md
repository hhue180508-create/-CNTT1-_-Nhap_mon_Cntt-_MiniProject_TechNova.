# Quy trình Không gian cộng tác Cloud

## 1. Hybrid Workflow

| Thành phần | Vai trò | Cách sử dụng |
|---|---|---|
| Local | Làm việc trực tiếp trên máy | Lưu bản đang chỉnh sửa trong thư mục dự án đã thống nhất |
| Cloud | Đồng bộ và cộng tác | Dùng tài khoản công ty, kiểm tra trạng thái đồng bộ |
| Version history | Khôi phục phiên bản | Dùng khi cần xem hoặc phục hồi thay đổi trước đó |

**Lưu ý:** Đồng bộ không thay thế hoàn toàn backup. Xóa nhầm ở Local có thể được đồng bộ lên Cloud. Tệp quan trọng cần có lịch sử phiên bản hoặc bản sao lưu riêng theo quy định công ty.

## 2. Bảng phân quyền mẫu

| Vai trò | Quyền Google Drive | Kênh Lark/Slack | Ghi chú |
|---|---|---|---|
| Nhân viên mới | Editor trên thư mục cá nhân do mình sở hữu | `#onboarding`, hỏi Mentor | Không tự ý chia sẻ dữ liệu nội bộ |
| Đồng đội cùng dự án | Editor trên thư mục dự án chung theo nhiệm vụ | `#dev-ten-du-an` | Dùng Thread cho từng vấn đề |
| Thực tập sinh phòng ban khác | Commenter khi cần góp ý | `#thong-bao` chỉ đọc; kênh được mời | Không cấp quyền sửa nếu không cần |
| Đối tác/khách mời | Viewer, Restricted theo email | Kênh khách mời riêng nếu được duyệt | Không cấp quyền vào Workspace nội bộ |

## 3. Nguyên tắc chia sẻ an toàn

- `Viewer`: chỉ xem.
- `Commenter`: xem và nhận xét.
- `Editor`: chỉnh sửa nội dung.
- Ưu tiên `Restricted` và cấp quyền theo email cụ thể.
- Tuyệt đối không kết hợp `Anyone with the link` với quyền Editor.
- Kiểm tra người nhận, phạm vi thư mục và quyền trước khi bấm Share.
- Khi nhân viên chuyển nhóm/nghỉ việc, rà soát và thu hồi quyền không còn cần thiết.

## 4. Văn hóa giao tiếp Channel/Thread

- `#onboarding`: câu hỏi của nhân viên mới và trao đổi với Mentor.
- `#dev-ten-du-an`: thảo luận kỹ thuật theo dự án.
- `#thong-bao`: thông báo chính thức, hạn chế chat tự do.
- Mỗi chủ đề mới tạo một Thread; trả lời tiếp trong Thread để không trôi nội dung.
- Tag đúng người liên quan, nêu rõ việc cần hỗ trợ và thời hạn.
- Tránh gửi “No-Hello” kéo dài; nêu thẳng bối cảnh và câu hỏi trong một tin nhắn.
- Không spam `@all`, đặc biệt ngoài giờ làm việc.
