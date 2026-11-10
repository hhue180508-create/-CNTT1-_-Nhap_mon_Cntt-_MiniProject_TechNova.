# Mẫu Báo cáo Lỗi (Bug Report)

## 1. Thông tin chung

- **Tiêu đề lỗi:**
- **Người báo cáo:**
- **Ngày/giờ xảy ra:**
- **Thiết bị và hệ điều hành:**
- **Tên phần mềm và phiên bản:**

## 2. Context (Bối cảnh)

Mô tả bạn đang làm gì, ở màn hình nào, dùng tài khoản/môi trường nào. Không ghi mật khẩu, OTP, API key hoặc dữ liệu cá nhân nhạy cảm.

## 3. Expected Result (Kết quả mong đợi)

Mô tả điều đáng lẽ phải xảy ra.

## 4. Actual Result (Kết quả thực tế)

Mô tả điều đã xảy ra, thời điểm và tần suất. Ghi rõ có thể tái hiện lỗi hay không.

## 5. Log / Screenshot

Dán thông báo lỗi nguyên văn hoặc đính kèm ảnh đã che thông tin nhạy cảm. Không gửi toàn bộ file cấu hình chứa Secrets.

## 6. Các bước đã thử

1. 
2. 
3. 

## 7. Prompt AI 3 thành phần

```text
Ngữ cảnh: Tôi đang dùng [hệ điều hành, phần mềm và phiên bản] để [mục tiêu].
Lỗi nguyên văn: [dán thông báo lỗi đã loại bỏ thông tin bí mật].
Yêu cầu: Hãy giải thích nguyên nhân có thể xảy ra, đề xuất cách kiểm tra an toàn từng bước và nêu rõ rủi ro trước khi đưa lệnh. Không đề xuất lệnh xóa/ghi đè dữ liệu khi chưa xác nhận.
```

## 8. Cheat-sheet Google Search

| Toán tử | Công dụng | Ví dụ |
|---|---|---|
| `site:` | Giới hạn trong một website | `site:docs.python.org ModuleNotFoundError` |
| Dấu ngoặc kép | Tìm đúng cụm từ | `"Permission denied"` |
| Dấu trừ `-` | Loại kết quả không muốn | `Git push error -advertisement` |

## 9. Quy trình tự tra cứu và gỡ lỗi

1. Đọc lỗi nguyên văn, ghi lại môi trường và phiên bản.
2. Tìm tài liệu chính thức trước; sau đó tìm Stack Overflow hoặc GitHub Issues.
3. Đọc câu trả lời và bình luận, kiểm tra ngày đăng, phiên bản, hệ điều hành và trường hợp tương tự.
4. Thử từng bước trên bản sao/dữ liệu thử nếu có thể; sao lưu trước khi thay đổi.
5. Nếu chưa giải quyết được, gửi Bug Report đủ Context, Expected, Actual và Log.

**Lưu ý:** Accepted Answer và Upvote là tín hiệu tham khảo, không bảo đảm giải pháp phù hợp với máy của bạn. Luôn kiểm tra phiên bản, môi trường và nội dung lệnh trước khi áp dụng.
