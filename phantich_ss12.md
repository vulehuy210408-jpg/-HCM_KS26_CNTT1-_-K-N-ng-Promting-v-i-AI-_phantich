# [Phân tích] So sánh Trade-off các giải pháp ra lệnh cho Cấu trúc Prompt Tiêu chuẩn & Định dạng
## I. Mục tiêu bài tập

- Rèn luyện tư duy phản biện trong việc thiết kế câu lệnh (Prompt Engineering).
- Đề xuất và so sánh 2 giải pháp viết prompt khác nhau cho cùng một bài toán thực tế:
  - Giải pháp 1: Đơn giản, ngắn gọn.
  - Giải pháp 2: Chi tiết, nhiều ràng buộc.
- Đánh giá ưu, nhược điểm (trade-off) để lựa chọn phương án tối ưu nhất.

## II. Đề xuất 2 giải pháp prompt mẫu

### 1. Giải pháp 1: Prompt đơn giản, ngắn gọn

- **Đặc điểm:** Tinh gọn, tập trung thẳng vào yêu cầu chính mà không đi sâu vào các ràng buộc biên dữ liệu hay định dạng cấu trúc phức tạp.
- **Nội dung prompt:**

```text
Hãy viết một email gửi bộ phận Nhân sự (HR) để xin nghỉ phép 2 ngày vì lý do cá nhân. Trình bày ngắn gọn, lịch sự và xuất bản dưới dạng mẫu email hoàn chỉnh.
```
## 2. Giải pháp 2: Prompt chi tiết, chuẩn khung CREATE và ràng buộc biên
[C] Context: Bạn là trợ lý AI hỗ trợ nhân viên văn phòng soạn thảo văn bản hành chính và giao tiếp nội bộ chuyên nghiệp tại doanh nghiệp.
[R] Request: Hãy tạo một mẫu email gửi bộ phận Nhân sự (HR) để xin nghỉ phép 2 ngày.
[E] Explanation & Edge Cases: Nếu thông tin thời gian hoặc lý do bị thiếu, hãy tự động chèn các khoảng trống [Cần cập nhật]. Đảm bảo ngôn ngữ lịch sự, chuyên nghiệp, đi thẳng vào vấn đề và không dùng từ ngữ khiếu nại gay gắt.
[A] Action:
1. Đặt tiêu đề (Subject) rõ ràng.
2. Nêu rõ lý do chính đáng và thời gian nghỉ cụ thể.
3. Đề xuất phương án bàn giao công việc ổn định cho đồng nghiệp.
[T] Tone: Chuyên nghiệp, lịch sự, chân thành và hợp tác.
[E] Extras: Xuất bản dưới dạng văn bản hoàn chỉnh, định dạng Markdown để copy sử dụng ngay.
