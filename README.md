# CẨM NANG SỬ DỤNG AI HIỆU QUẢ CHO TÂN SINH VIÊN


## PHẦN 1: CÁCH AI ĐOÁN TỪ (LLM HOẠT ĐỘNG THẾ NÀO?)

**1. LLM là gì?**

LLM (Large Language Model) là mô hình ngôn ngữ lớn được huấn luyện trên lượng dữ liệu văn bản lớn để nhận diện quy luật ngôn ngữ và dự đoán nội dung tiếp theo.

**2. AI tạo câu trả lời như thế nào?**

AI không suy nghĩ giống con người mà dự đoán Token tiếp theo dựa trên ngữ cảnh và xác suất.

Ví dụ:

Khi nhập câu: "Ngôn ngữ lập trình phổ biến để học lập trình là..."

AI có thể dự đoán các từ tiếp theo như "Python", "C++" hoặc "Java" dựa trên ngữ cảnh.

**3. Token và Context Window**

- Token: Đơn vị dữ liệu AI sử dụng để xử lý văn bản.
- Context Window: Giới hạn lượng Token AI có thể tiếp nhận và xử lý trong một ngữ cảnh.
- Khi hội thoại quá dài, thông tin cũ có thể bị cắt bỏ (Truncation).

## PHẦN 2: BA CÁCH NHẬN DIỆN ẢO GIÁC CỦA AI

Ảo giác AI (AI Hallucination) là hiện tượng AI tạo ra thông tin sai lệch nhưng trình bày như thể đó là sự thật.

**Cách 1: Kiểm tra nguồn thông tin**

- Yêu cầu AI cung cấp tài liệu hoặc đường dẫn tham khảo.
- Ưu tiên tài liệu chính thức, giáo trình và trang chủ của nhà phát triển.
- Kiểm tra xem nguồn có thực sự tồn tại và hỗ trợ nội dung AI đưa ra hay không.

**Cách 2: Kiểm tra và chạy thử kết quả**

- Với code lập trình, cần chạy thử trên VS Code hoặc OnlineGDB.
- Kiểm tra lỗi cú pháp, kết quả đầu ra và các trường hợp đặc biệt.
- Không sao chép code của AI mà chưa hiểu cách hoạt động.

**Cách 3: Đối chiếu và kiểm tra chéo**

- So sánh câu trả lời với giáo trình hoặc tài liệu đáng tin cậy.
- Có thể hỏi thêm một mô hình AI khác để tìm ra điểm bất đồng.
- Tự đánh giá và xác minh lại trước khi sử dụng thông tin.

**Nguyên tắc:** Không tin tưởng tuyệt đối vào câu trả lời của AI, kể cả khi câu trả lời được trình bày rất tự tin.

## PHẦN 3: CẤU TRÚC PROMPT MẪU TỐI ƯU BẰNG KHUNG CREATE

CREATE gồm 6 thành phần:

| Thành phần | Ý nghĩa |
|---|---|
| C – Context | Xác định bối cảnh và vai trò của AI |
| R – Request | Nêu nhiệm vụ cần AI thực hiện |
| E – Explanation | Giải thích mục đích và yêu cầu |
| A – Action | Chỉ định các bước AI cần thực hiện |
| T – Tone | Quy định giọng điệu và cách trình bày |
| E – Extras | Bổ sung giới hạn và ràng buộc |

**Prompt mẫu hỗ trợ học lập trình:**

**C – Context:**
Bạn là giảng viên lập trình C++ đang hướng dẫn sinh viên năm nhất chưa có nhiều kiến thức lập trình.

**R – Request:**
Hãy giải thích vòng lặp for trong C++ và đưa ra một ví dụ minh họa.

**E – Explanation:**
Tôi muốn hiểu bản chất vòng lặp for để có thể tự viết chương trình, không chỉ học thuộc cú pháp.

**A – Action:**
1. Giải thích vòng lặp for là gì.
2. Phân tích từng thành phần trong cú pháp.
3. Đưa ra một ví dụ tính tổng từ 1 đến 10.
4. Giải thích từng dòng code.
5. Đưa ra một bài tập nhỏ để tự thực hành.

**T – Tone:**
Sử dụng tiếng Việt đơn giản, dễ hiểu, phù hợp với sinh viên năm nhất.

**E – Extras:**
- Không sử dụng kiến thức nâng cao.
- Không bỏ qua bước giải thích code.
- Nếu có nhiều cách giải, hãy chọn cách đơn giản nhất.
- Không khẳng định thông tin chưa được kiểm chứng.
