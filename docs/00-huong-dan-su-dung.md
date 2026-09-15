# Hướng dẫn sử dụng lộ trình tự học

Tài liệu này giúp bạn tìm đúng điểm xuất phát và đi đúng nhịp trên lộ trình 170 chặng. Trước khi đọc tiếp, hãy mở [ROADMAP.md](../ROADMAP.md) một lượt để có bức tranh tổng thể về 8 phần của hành trình.

## 1. Xác định con đường tự học của bạn

Lộ trình thiết kế cho **một con đường duy nhất chia 170 chặng**, nhưng bạn có thể bước lên con đường đó với ba nhịp độ khác nhau tùy nền tảng sẵn có:

| Con đường | Phù hợp với | Điểm bắt đầu | Nhịp gợi ý |
|-----------|-------------|--------------|------------|
| **Tuần tự** | Người mới bắt đầu tuyệt đối, chưa từng lập trình | Chặng 01 | 1 chặng / 1–2 tuần |
| **Tăng tốc** | Người đã biết Python cơ bản hoặc có nền tảng kỹ thuật | Phần D (chặng 77) nếu rành Python; Phần C (chặng 53) nếu mới biết lập trình | 2–3 chặng / tuần |
| **Theo nhu cầu** | Người học có mục tiêu nghề nghiệp cụ thể | Tùy mục tiêu (xem bảng bên dưới) | Tùy chọn chặng |

### Gợi ý chọn chặng theo nhu cầu thực tế

| Bạn là... | Nên học | Có thể bỏ qua | Lý do |
|-----------|---------|----------------|-------|
| Người làm văn phòng muốn dùng AI hiệu quả | Chặng 53–56, 77–92, 146–149 | A, B, E–H | Bảng tính, phân tích dữ liệu, dùng LLM hiệu quả |
| Sinh viên ngành khác muốn chuyển sang AI | Chặng 53–170 | A, B (sau khi tự kiểm tra) | Nền dữ liệu + ML + DL + triển khai |
| Nhà báo, người làm truyền thông | Chặng 53–76, 71–72, 118–119 | A, B, D, E, F, G, H | Hiểu AI xã hội, đạo đức, phát hiện tin giả |
| Người quản lý muốn hiểu AI ra quyết định | Chặng 61–76, 101–112, 141–145 | A, B, F, G, H | Hiểu quy trình ML, đánh giá, giải thích mô hình |
| Lập trình viên muốn xây ứng dụng AI | Chặng 77–158 | A, B (sau khi kiểm tra) | Khoa học dữ liệu + ML + DL + triển khai |
| Người muốn đi nghiên cứu | Toàn bộ theo số thứ tự | Không | Mỗi chặng là nền cho chặng sau |

**Quy tắc vàng:** trước khi bỏ qua một phần, hãy tự làm bài tập cuối chặng tiêu biểu của phần đó. Làm được trọn vẹn thì mới có quyền bỏ qua — đây là cách tránh "tự tin ảo" mà không cần ai phán xét.

## 2. Cách dùng một thư mục chặng

Mỗi chặng đã phát hành gồm 3 tệp, dùng theo trình tự sau:

| Thứ tự | Tệp | Mục đích | Lời khuyên |
|--------|-----|----------|-----------|
| 1 | `README.md` | Đọc toàn bộ phần Kiến thức trước, không lướt qua | Ghi chú khái niệm mới bằng lời của mình |
| 2 | `bai-tap-thuc-hanh.md` | Làm lần lượt bài tập từ dễ đến khó; bài sao ★ là bắt buộc | Không xem đáp án (nếu có) trước khi đã thử 30 phút |
| 3 | `tu-dien-va-tai-nguyen.md` | Tra thuật ngữ khi quên; đọc tài nguyên mở rộng khi muốn sâu hơn | Đọc phần "Kết nối về sau" để biết chặng sau cần gì |

Sau khi hoàn thành 3 tệp, bạn làm **Sản phẩm cuối chặng** mô tả trong README. Sản phẩm là bằng chứng bạn đã học — không phải bài kiểm tra ai chấm, mà là artifact đưa vào portfolio cá nhân.

## 3. Bốn thói quen tự học giúp bạn đi hết 170 chặng

### Thói quen 1: Ghi chú kiểu Feynman

Khi đọc xong phần Kiến thức của một chặng, hãy đóng tài liệu lại và viết lại khái niệm bằng lời của mình như đang giải thích cho một người không biết gì về AI. Nếu bạn không viết được — bạn chưa hiểu. Quay lại đọc. Lặp lại.

Ví dụ thay vì chép "AI là trí tuệ nhân tạo", hãy viết: *"AI là ngành xây dựng hệ thống máy tính làm được những việc cần trí tuệ khi người làm — như nhận dạng ảnh, hiểu ngôn ngữ, chơi cờ. Cách tiếp cận phổ biến nhất là cho máy học từ rất nhiều ví dụ thay vì viết quy tắc tay."*

### Thói quen 2: Một chặng, một sản phẩm

Không chặng nào kết thúc bằng "tôi đã đọc xong". Mỗi chặng đều có một sản phẩm cụ thể: nhật ký, chương trình, notebook, mô hình. Sản phẩm đưa vào một thư mục `portfolio/` trên máy bạn (và sau này đẩy lên GitHub từ Phần D). Khi đến chặng 170, bạn có 170 sản phẩm — đó là hồ sơ năng lực thực sự, giá trị hơn bất kỳ chứng chỉ nào.

### Thói quen 3: Sai là dữ liệu

Khi làm bài tập mà code lỗi, mô hình cho kết quả sai, hoặc khái niệm khó hiểu — đừng nản. Thông báo lỗi của Python là tin nhắn từ hệ thống, kết quả sai là thí nghiệm thành công về "cách không làm". Ghi lại lỗi và nguyên nhân vào một tệp `lessons-learned.md` trong thư mục portfolio. Vài tháng sau bạn sẽ có một kho "những cái bẫy đã qua" — tài sản quý nhất của người tự học.

### Thói quan 4: Lặp lại theo chu kỳ

Khoa học não bộ chỉ ra rằng ôn lại kiến thức sau 1 ngày, 1 tuần, 1 tháng giúp chuyển vào trí nhớ dài hạn. Cuối mỗi tuần, giở lại danh sách thuật ngữ đã học trong tuần. Cuối mỗi tháng, đọc lại README của các chặng đã qua. Bạn sẽ nhận ra mình hiểu sâu hơn so với lần đầu — đó là dấu hiệu của lặp xoáy ốc.

## 4. Môi trường làm việc

Bạn không cần máy cấu hình cao cho phần lớn lộ trình. Gợi ý tối thiểu:

| Phần | Cấu hình tối thiểu | Công cụ bắt buộc | Tùy chọn |
|------|-------------------|------------------|----------|
| A | Bất kỳ máy tính/laptop nào có trình duyệt | Trình duyệt web, giấy bút | Tài khoản MIT Scratch (miễn phí) |
| B–C | Laptop 4GB RAM | Python 3.10+, VS Code | Google Colab (miễn phí) |
| D–E | Laptop 8GB RAM | Python, Jupyter, Git | Google Colab, Kaggle notebook |
| F | Laptop 8GB RAM + GPU hoặc Colab miễn phí | PyTorch, CUDA (nếu có GPU) | Colab Pro (~150k/tháng) |
| G | Laptop 8GB RAM + Docker | Docker, GitHub account | Cloud account (AWS/GCP/Azure miễn phí ban đầu) |
| H | Linh hoạt | Tùy dự án | Tùy dự án |

Nếu bạn chỉ có điện thoại thông minh: vẫn học được Phần A và một phần Phần C (đọc + quan sát + ghi chú). Hãy cố gắng sắp xếp có máy tính từ Phần B trở đi.

## 5. Khi gặp khó khăn

Tự học không có nghĩa là cô lập. Khi mắc ở một chặng quá 2 ngày:

1. **Đọc lại phần Tiên quyết** ở đầu README của chặng đó. Có thể bạn đang thiếu kiến thức nền của chặng trước.
2. **Tra từ điển thuật ngữ** trong `tu-dien-va-tai-nguyen.md` — đôi khi chỉ là hiểu nhầm một khái niệm.
3. **Tìm trên Google/Stack Overflow/arxiv** với từ khóa tiếng Anh (lý do lộ trình này ghi song ngữ). Phần lớn vấn đề đã có người gặp và giải thích.
4. **Hỏi AI trợ lý** (ChatGPT, Claude, Gemini, DeepSeek) — đây cũng là một kỹ năng cần học (chặng 72). Hỏi cụ thể, kèm code lỗi và thông báo lỗi nguyên văn.
5. **Tạm dừng 1–2 ngày rồi quay lại** — não cần thời gian xử lý ngầm. Nhiều vấn đề khó tự nhiên "bừng sáng" sau giấc ngủ.

Không có ai chấm điểm, không có deadline. Tốc độ của bạn là tốc độ của bạn. Quan trọng là đi tiếp, không phải đi nhanh.

## 6. Đánh giá bản thân

Xem [03-he-thong-danh-gia-chung-nhan.md](03-he-thong-danh-gia-chung-nhan.md) để biết cách tự đánh giá sau mỗi chặng và sau mỗi phần. Tóm tắt: mỗi chặng có một danh mục tự kiểm tra (checklist) thay cho rubric chấm điểm; mỗi phần có một sản phẩm tổng kết; toàn lộ trình kết thúc bằng portfolio 170 sản phẩm.

## 7. Một số quy ước đọc

- **In đậm** = thuật ngữ quan trọng xuất hiện lần đầu.
- *In nghiêng* = thuật ngữ tiếng Anh tương đương.
- `Monospace` = mã lệnh, tên tệp, hoặc output.
- > Đoạn trong khối trích dẫn = định nghĩa chuẩn hoặc nguyên lý quan trọng cần ghi nhớ.
- ★ sau tên bài tập = bài tập lõi, bắt buộc hoàn thành trước khi sang chặng sau.
