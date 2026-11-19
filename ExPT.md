# [Phân tích] So sánh Trade-off các giải pháp ra lệnh cho Ứng dụng AI trong Học tập & Nghiên cứu

**Chủ đề:** Ứng dụng AI trong Học tập & Nghiên cứu (Feynman gia sư + Rubric chấm bài)

## Bước 1: Hai prompt mẫu

**Giải pháp 1 (Đơn giản):**
```
Giải thích "Khóa ngoại trong CSDL" cho tôi như dạy học sinh lớp 6.
Sau đó đặt 1 câu hỏi kiểm tra và chấm câu trả lời của tôi trên thang 10.
```

**Giải pháp 2 (Chi tiết):**
```
Vai trò: Gia sư Feynman kiêm giám khảo.
Nhiệm vụ: Dạy "Khóa ngoại trong CSDL" cho sinh viên năm nhất.

Quy trình:
1. Giải thích đơn giản + 1 ví dụ đời thường (tối đa 120 từ).
2. Yêu cầu tôi tự giải thích lại bằng lời của mình.
3. Chấm theo Rubric 10 điểm: Đúng khái niệm (4), Có ví dụ (3), Dễ hiểu (3).
4. Chỉ ra chỗ còn hổng và cách sửa.

Ràng buộc:
- Trả lời lạc đề hoặc để trống: không chấm, yêu cầu làm lại.
- Không chắc thì nói "tôi không chắc", không bịa.
- Không đưa đáp án trước khi tôi trả lời.
- Chỉ dùng tiếng Việt.

Định dạng: Bảng điểm từng tiêu chí + nhận xét tối đa 3 dòng.
```

## Bước 2: Bảng so sánh Trade-off

| Tiêu chí | Giải pháp 1 (Đơn giản) | Giải pháp 2 (Chi tiết) |
|---|---|---|
| Độ dễ hiểu | Cao | Trung bình |
| Tốn token | Ít | Nhiều hơn |
| Thời gian viết | Nhanh | Lâu hơn |
| Độ ổn định kết quả | Thấp | Cao |
| Rubric chấm điểm | AI tự đặt, không nhất quán | Cố định, nhất quán |
| Chặn lỗi biên | Trung bình | Cực tốt |
| Phù hợp | Hỏi nhanh | Học nghiêm túc, chấm lặp lại |

## Bước 3: Lựa chọn và chạy thử

**Chọn: Giải pháp 2.**

**Lý do:**
1. Cần Rubric cố định để chấm công bằng, so sánh được giữa các lần.
2. Có ràng buộc chặn lỗi biên (lạc đề, bịa thông tin).
3. Đúng tinh thần Feynman: bắt người học tự giải thích, không đưa đáp án sẵn.
4. Tốn thêm token nhưng đổi lại độ chính xác cao hơn.

**Kết quả chạy thử** (mô phỏng, khi nộp bạn nên tự chạy lại và dán kết quả thật):

- **AI giải thích:** Khóa ngoại giống *số thẻ sinh viên ghi trên phiếu mượn sách*: phiếu chỉ ghi số thẻ để tra ngược về danh sách sinh viên. Trong CSDL, khóa ngoại là cột ở bảng này trỏ tới khóa chính của bảng khác. Bạn hãy tự giải thích lại nhé.
- **Người học:** "Khóa ngoại là cột để nối hai bảng với nhau."
- **AI chấm:**

| Tiêu chí | Điểm | Nhận xét |
|---|---|---|
| Đúng khái niệm | 3/4 | Thiếu "trỏ tới khóa chính" |
| Có ví dụ | 0/3 | Chưa có ví dụ |
| Dễ hiểu | 3/3 | Ngắn gọn, rõ |
| **Tổng** | **6/10** | |

- **Gợi ý:** Thêm ví dụ "bảng Đơn hàng có cột MaKH trỏ tới bảng Khách hàng".
- **Thử ca biên:** Nếu người học viết "Hôm nay trời đẹp", AI trả lời: *"Câu trả lời chưa liên quan nên mình chưa chấm điểm, bạn thử lại nhé."*

## Kết luận

Giải pháp 2 vượt trội về độ ổn định, Rubric nhất quán và chặn lỗi biên; đánh đổi là tốn token và công viết prompt. Với học tập và nghiên cứu, đây là sự đánh đổi hợp lý.
