# Bài: So sánh Markdown và HTML trong hệ thống AI

## Phần 1. Phân tích bài toán

AI không đọc từng chữ cái mà chia văn bản thành các Token (mảnh nhỏ). Số Token càng nhiều thì chi phí càng cao và xử lý càng chậm.

HTML dùng thẻ mở và thẻ đóng, nên mỗi định dạng tốn nhiều ký tự và bị chia thành nhiều Token. Markdown chỉ dùng vài ký hiệu nên ít ký tự, ít Token hơn.

Ví dụ in đậm chữ "Rau sạch":

- HTML: `<strong>Rau sạch</strong>` (25 ký tự)
- Markdown: `**Rau sạch**` (12 ký tự)

Cùng nội dung nhưng Markdown ngắn hơn khoảng một nửa, nên AI đọc nhanh hơn và tiết kiệm Token.

## Phần 2. So sánh & Đánh giá

| Tiêu chí | Markdown | HTML |
|----------|----------|------|
| Số ký tự cho cùng định dạng | Ít (`**chữ**`) | Nhiều (`<strong>chữ</strong>`) |
| Số Token | Ít | Nhiều |
| Chi phí | Thấp | Cao hơn |
| Tốc độ xử lý của AI | Nhanh | Chậm hơn |
| Human-readable (người đọc được) | Cao, đọc thẳng được | Thấp, rối vì nhiều thẻ |
| Tùy biến giao diện | Cơ bản | Rất mạnh |

**Giải pháp tối ưu cho GreenTech:** dùng Markdown.

**Lý do:**

- Tiết kiệm Token nên giảm chi phí và trả lời nhanh hơn cho nông dân.
- Dễ đọc, dễ viết, dễ kiểm tra lỗi, người không rành kỹ thuật cũng hiểu.
- Câu trả lời của chuyên gia nông nghiệp chỉ cần tiêu đề, danh sách, in đậm, bảng nên Markdown là đủ.
- Nếu cần giao diện đẹp hơn thì chuyển Markdown sang HTML ở bước hiển thị, không cần gửi HTML cho AI.