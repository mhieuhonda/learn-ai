# Hướng dẫn sử dụng lộ trình

Tài liệu này giúp từng nhóm người dùng khác nhau tìm đúng điểm xuất phát và đi đúng nhịp trên lộ trình 170 giai đoạn. Trước khi đọc tiếp, hãy mở [ROADMAP.md](../ROADMAP.md) một lượt để có bức tranh tổng thể về 8 phần của hành trình.

## 1. Xác định con đường học tập của bạn

Lộ trình thiết kế cho **một con đường duy nhất chia 170 chặng**, nhưng ba nhóm người dùng sẽ bước lên con đường đó với ba nhịp độ khác nhau:

| Con đường | Dành cho | Điểm bắt đầu | Nhịp gợi ý |
|-----------|----------|--------------|-------------|
| **Học đường chuẩn** | Học sinh tiểu học → THCS → THPT | Giai đoạn 01 | 1 giai đoạn / 1–2 tuần |
| **Tăng tốc** | Người lớn tự học, sinh viên, người chuyển ngành | Phần D (77) nếu đã biết Python; Phần C (53) nếu mới biết lập trình | 2–3 giai đoạn / tuần |
| **Theo nhu cầu** | Giáo viên, phụ huynh, người làm nghề khác | Tùy mục tiêu (xem bảng bên dưới) | Tùy chọn giai đoạn |

### Gợi ý chọn giai đoạn theo nhu cầu thực tế

| Bạn là... | Nên học | Bỏ qua | Lý do |
|-----------|---------|--------|-------|
| Giáo viên tiểu học | GĐ 01–24, 53–56 | B, D–H | Cần biết dạy tư duy máy tính và nhận biết AI cho trẻ |
| Giáo viên THCS/THPT (Tin học) | GĐ 25–100 | A | Nền Python + dữ liệu phục vụ giảng dạy |
| Phụ huynh đồng hành cùng con | GĐ 01–24 kèm con; tự học GĐ 61–76 | B, D+ | Hiểu AI để dẫn dắt con an toàn |
| Nhân viên văn phòng | GĐ 53–56, 77–92, 146–149 | A, B, E–H | Bảng tính, phân tích dữ liệu, dùng LLM hiệu quả |
| Sinh viên ngành khác muốn chuyển sang AI | GĐ 53–170 | A, B (kiểm tra trước) | Nền dữ liệu + ML + DL + triển khai |
| Học sinh THPT mê AI | Toàn bộ theo số thứ tự | Không bỏ giai đoạn nào | Mỗi giai đoạn là viên gạch cho giai đoạn sau |

**Quy tắc vàng:** trước khi bỏ qua một phần nào đó, hãy tự làm bài tập cuối giai đoạn tiêu biểu của phần đó. Làm được trọn vẹn thì mới có quyền bỏ qua — đây là cách tránh "tự tin ảo" mà không cần ai phán xét.

## 2. Cách dùng một thư mục giai đoạn

Mỗi giai đoạn đã phát hành gồm 3 tệp, dùng theo trình tự sau:

1. **Đọc `README.md`** — xem "Thông tin chung" để chuẩn bị nguyên liệu; đọc mục tiêu học tập để biết đích đến; học theo từng bài trong "Nội dung bài học"; đối chiếu "Rubric đánh giá" trước khi làm sản phẩm.
2. **Làm `bai-tap-thuc-hanh.md`** — bài tập được xếp từ dễ đến khó; bắt buộc làm bài tập lõi (đánh dấu sao), bài nâng cao là tùy chọn dành cho học sinh muốn đi nhanh hơn.
3. **Tra `tu-dien-va-tai-nguyen.md`** khi gặp thuật ngữ lạ; dùng phần "Câu hỏi gợi mở" để trò chuyện với gia đình hoặc nhóm học tập.

Sau khi hoàn thành sản phẩm cuối giai đoạn: chụp ảnh hoặc sao lưu số hóa sản phẩm vào thư mục portfolio cá nhân, tự chấm theo rubric, xin chữ ký/xác nhận của phụ huynh hoặc giáo viên (với học sinh dưới 18 tuổi), rồi mới chuyển giai đoạn kế tiếp.

## 3. Thiết bị và tài khoản cần chuẩn bị

| Phần | Thiết bị tối thiểu | Tài khoản / phần mềm |
|------|--------------------|----------------------|
| A | Máy tính hoặc chỉ giấy bút (nhiều hoạt động unplugged) | Scratch (scratch.mit.edu) cho GĐ 09–16, có người lớn đồng hành |
| B | Máy tính 4GB RAM | Python 3.10+ hoặc Google Colab; trình duyệt web |
| C | Máy tính | Google Sheets; SQLite/DB Browser; tài khoản do phụ huynh tạo |
| D | Máy tính 8GB RAM | Anaconda hoặc Colab; Git; tài khoản GitHub |
| E | Máy tính 8GB RAM | scikit-learn; tài khoản Kaggle (có phụ huynh xác nhận nếu dưới 13 tuổi) |
| F | Máy tính + GPU (Colab miễn phí) | PyTorch; Hugging Face |
| G | Máy tính 16GB RAM | Docker; GitHub; dịch vụ LLM API (chỉ người 18+ hoặc có sự cho phép) |
| H | Tùy dự án | Công cụ nghiên cứu, Kaggle, Hugging Face |

Lưu ý an toàn: học sinh **dưới 13 tuổi** không tự tạo tài khoản trực tuyến — phụ huynh tạo và giám sát. Mọi hoạt động chụp ảnh, ghi âm cần xin phép người được ghi nhận.

## 4. Lên lịch học mẫu

### Học sinh tiểu học (Phần A)

- **Tuần học thông thường:** 2 buổi x 35 phút — buổi 1 học khái niệm mới, buổi 2 thực hành và hoàn thành sản phẩm.
- **Cuối tuần gia đình:** 15 phút cùng phụ huynh làm bài tập thực hành và trò chuyện theo câu hỏi gợi mở.

### Học sinh THCS – THPT (Phần B–F)

- **Học kỳ:** 1 giai đoạn / tuần = 2–3 buổi x 45–90 phút + 1 giờ tự làm bài tập.
- **Hè:** tăng lên 2–3 giai đoạn / tuần; đây là lúc đẩy nhanh một phần lớn hành trình mà không ảnh hưởng việc học chính khóa.

### Người tự học (Phần D–H)

- **Nhịp 90 phút/ngày:** mỗi giai đoạn 2–3 ngày, mỗi phần 3–6 tuần, toàn lộ trình phần còn lại 6–12 tháng.
- **Nhịp cuối tuần:** mỗi tuần 1 buổi x 4 giờ = 1 giai đoạn; phù hợp người đi làm.

## 5. Theo dõi tiến độ

- In hoặc sao chép bảng 170 giai đoạn trong ROADMAP.md, dán ở bàn học; tô màu mỗi giai đoạn hoàn thành.
- Giữ "Hồ sơ hành trình" (thư mục Google Drive/USB) với cấu trúc: `GD01-Nhat-ky-AI/`, `GD02-Sach-thuat-toan/`... Mỗi giai đoạn một thư mục chứa sản phẩm + ảnh chụp + phiếu tự đánh giá.
- Mỗi khi qua một cột mốc (GĐ 24, 52, 76, 100, 120, 140, 158, 170), hãy "lên cấp" — tổ chức một buổi trình bày nhỏ cho gia đình hoặc lớp học (chi tiết trong [docs/03-he-thong-danh-gia-chung-nhan.md](03-he-thong-danh-gia-chung-nhan.md)).

## 6. Câu hỏi thường gặp

**Con tôi 8 tuổi, chưa biết đọc trôi chảy, có học được không?**
Có. Các giai đoạn 01–03 và 17–18 được thiết kế hoạt động tốt kể cả khi phụ huynh đọc giúp. Kỹ năng đọc càng tốt, em càng tự chủ được — hãy đi chậm, ưu tiên hoạt động unplugged.

**Không có máy tính ở nhà thì học được đến đâu?**
Phần A học được hơn một nửa (các hoạt động unplugged) và có thể mượn máy ở thư viện/trường cho phần Scratch. Các phần sau bắt buộc cần máy tính — đề nghị nhà trường hỗ trợ là cách làm phổ biến.

**Học xong lộ trình có được việc làm không?**
Lộ trình đưa bạn tới trình độ "kỹ sư AI tập sự / nhà nghiên cứu tập sự" — đủ nền tảng thi tuyển thực tập sinh, tham gia dự án mã nguồn mở hoặc tiếp tục đại học chuyên ngành. Kho tài liệu không thay thế bằng cấp, nhưng portfolio 170 sản phẩm là lợi thế thật sự.

**Nếu học bị kẹt ở một giai đoạn thì làm sao?**
Không chuyển giai đoạn khi sản phẩm chưa xong — nhưng được giảm độ khó: làm lại bài tập lõi, xin gợi ý (không xin đáp án) từ AI hoặc giáo viên, hoặc học lại giai đoạn trước. Kẹt lâu hơn 3 buổi thì nghỉ 1 buổi rồi quay lại; thường sẽ "thông" ngay.

**AI có thay con người dạy học không?**
Không trong thiết kế này. AI là công cụ thực hành và "người bạn hỏi bài", còn việc đặt mục tiêu, kỷ luật học tập, đạo đức và sự đồng cảm thuộc về con người — giáo viên và gia đình.
