# Hướng dẫn sử dụng lộ trình tự học

Tài liệu này giúp bạn tìm đúng điểm xuất phát và đi đúng nhịp trên lộ trình 170 chặng. Trước khi đọc tiếp, hãy mở [ROADMAP.md](../ROADMAP.md) một lượt để có bức tranh tổng thể về bốn phần của hành trình.

## 1. Xác định con đường tự học của bạn

Lộ trình thiết kế cho một con đường duy nhất chia 170 chặng, nhưng bạn có thể bước lên con đường đó với ba nhịp độ khác nhau tùy nền tảng sẵn có. Con đường tuần tự phù hợp người mới bắt đầu tuyệt đối, chưa từng lập trình, bắt đầu từ chặng 01, nhịp 1 chặng mỗi 1 đến 2 tuần. Con đường tăng tốc phù hợp người đã biết Python cơ bản hoặc có nền tảng kỹ thuật, bắt đầu từ Phần 2 (chặng 53) nếu mới biết lập trình, hoặc từ chặng 77 nếu rành Python, nhịp 2 đến 3 chặng mỗi tuần. Con đường theo nhu cầu phù hợp người có mục tiêu nghề nghiệp cụ thể, chọn chặng tùy mục tiêu, nhịp tùy chọn.

### Gợi ý chọn chặng theo nhu cầu thực tế

| Bạn là... | Nên học | Có thể bỏ qua | Lý do |
|-----------|---------|----------------|-------|
| Người làm văn phòng muốn dùng AI hiệu quả | Chặng 53 đến 56, 77 đến 92, 146 đến 149 | Phần 1, Phần 3 từ 101 trở đi | Bảng tính, phân tích dữ liệu, dùng LLM hiệu quả |
| Sinh viên ngành khác muốn chuyển sang AI | Chặng 53 đến 170 | Phần 1 (sau khi tự kiểm tra) | Nền dữ liệu cộng ML cộng DL cộng triển khai |
| Nhà báo, người làm truyền thông | Chặng 53 đến 76, 118 đến 119 | Phần 1, chặng 77 đến 100, 121 trở đi | Hiểu AI xã hội, đạo đức, phát hiện tin giả |
| Người quản lý muốn hiểu AI ra quyết định | Chặng 61 đến 76, 101 đến 112, 141 đến 145 | Phần 1, chặng 121 trở đi | Hiểu quy trình ML, đánh giá, giải thích mô hình |
| Lập trình viên muốn xây ứng dụng AI | Chặng 77 đến 158 | Phần 1 (sau khi kiểm tra) | Khoa học dữ liệu cộng ML cộng DL cộng triển khai |
| Người muốn đi nghiên cứu | Toàn bộ theo số thứ tự | Không | Mỗi chặng là nền cho chặng sau |

Quy tắc vàng: trước khi bỏ qua một phần, hãy tự làm bài tập cuối chặng tiêu biểu của phần đó. Làm được trọn vẹn thì mới có quyền bỏ qua. Đây là cách tránh "tự tin ảo" mà không cần ai phán xét.

## 2. Cách dùng một chặng

Mỗi chặng đã phát hành là một tệp README duy nhất, không cần nhảy giữa các tệp rời rạc. Đọc từ đầu đến cuối là hiểu. Tệp chia bốn phần theo trật tự: Kiến thức (định nghĩa, cơ chế, ví dụ, định nghĩa thuật ngữ ngay tại chỗ dùng lần đầu), Thực hành (bài tập từ dễ đến khó, bài có sao là bắt buộc), Sản phẩm cuối chặng (artifact đưa vào portfolio), và Tự đánh giá cộng kết nối về sau (checklist, thuật ngữ cần nhớ, tài nguyên mở rộng, gợi ý nhật ký học tập).

Cách đọc hiệu quả: đầu tiên đọc trọn phần Kiến thức, không lướt qua, ghi chú khái niệm mới bằng lời của mình. Sau đó làm phần Thực hành, không xem đáp án (nếu có) trước khi đã thử 30 phút. Khi xong, làm Sản phẩm cuối chặng và lưu vào portfolio. Cuối cùng, đánh dấu checklist Tự đánh giá và đọc phần Kết nối về sau để biết chặng sau cần gì.

## 3. Bốn thói quen tự học giúp bạn đi hết 170 chặng

Thói quen thứ nhất là ghi chú kiểu Feynman. Khi đọc xong phần Kiến thức của một chặng, hãy đóng tài liệu lại và viết lại khái niệm bằng lời của mình như đang giải thích cho một người không biết gì về AI. Nếu bạn không viết được, bạn chưa hiểu. Quay lại đọc, lặp lại. Ví dụ thay vì chép "AI là trí tuệ nhân tạo", hãy viết: "AI là ngành xây dựng hệ thống máy tính làm được những việc cần trí tuệ khi người làm, như nhận dạng ảnh, hiểu ngôn ngữ, chơi cờ. Cách tiếp cận phổ biến nhất là cho máy học từ rất nhiều ví dụ thay vì viết quy tắc tay."

Thói quen thứ hai là một chặng, một sản phẩm. Không chặng nào kết thúc bằng "tôi đã đọc xong". Mỗi chặng đều có một sản phẩm cụ thể: nhật ký, chương trình, notebook, mô hình. Sản phẩm đưa vào một thư mục `portfolio-ai/` trên máy bạn, và từ Phần 2 trở đi đẩy lên GitHub. Khi đến chặng 170, bạn có 170 sản phẩm, đó là hồ sơ năng lực thực sự, giá trị hơn bất kỳ chứng chỉ nào.

Thói quen thứ ba là sai là dữ liệu. Khi làm bài tập mà code lỗi, mô hình cho kết quả sai, hoặc khái niệm khó hiểu, đừng nản. Thông báo lỗi của Python là tin nhắn từ hệ thống, kết quả sai là thí nghiệm thành công về "cách không làm". Ghi lại lỗi và nguyên nhân vào một tệp `lessons-learned.md` trong thư mục portfolio. Vài tháng sau bạn sẽ có một kho "những cái bẫy đã qua", tài sản quý nhất của người tự học.

Thói quen thứ tư là lặp lại theo chu kỳ. Khoa học não bộ chỉ ra rằng ôn lại kiến thức sau 1 ngày, 1 tuần, 1 tháng giúp chuyển vào trí nhớ dài hạn. Cuối mỗi tuần, giở lại danh sách thuật ngữ đã học trong tuần. Cuối mỗi tháng, đọc lại README của các chặng đã qua. Bạn sẽ nhận ra mình hiểu sâu hơn so với lần đầu, đó là dấu hiệu của lặp xoáy ốc.

## 4. Môi trường làm việc

Bạn không cần máy cấu hình cao cho phần lớn lộ trình. Gợi ý tối thiểu theo từng phần:

| Phần | Cấu hình tối thiểu | Công cụ bắt buộc | Tùy chọn |
|------|---------------------|------------------|----------|
| 1 (chặng 01 đến 24) | Bất kỳ máy tính hoặc laptop nào có trình duyệt | Trình duyệt web, giấy bút | Tài khoản MIT Scratch miễn phí |
| 1 (chặng 25 đến 52) | Laptop 4GB RAM | Python 3.10 trở lên, VS Code | Google Colab miễn phí |
| 2 (chặng 53 đến 76) | Laptop 4GB RAM | Google Sheets, SQLite | Google Colab, DB Browser |
| 2 (chặng 77 đến 100) | Laptop 8GB RAM | Python, Jupyter, Git | Google Colab, Kaggle notebook |
| 3 | Laptop 8GB RAM cộng GPU hoặc Colab miễn phí | PyTorch, CUDA nếu có GPU | Colab Pro khoảng 150 nghìn một tháng |
| 4 | Laptop 8GB RAM cộng Docker | Docker, GitHub account | Cloud account AWS GCP Azure miễn phí ban đầu |

Nếu bạn chỉ có điện thoại thông minh, vẫn học được Phần 1 (chặng 01 đến 24) ở mức đọc, quan sát, ghi chú. Hãy cố gắng sắp xếp có máy tính từ chặng 25 trở đi.

## 5. Khi gặp khó khăn

Tự học không có nghĩa là cô lập. Khi mắc ở một chặng quá 2 ngày, có năm bước xử lý. Một, đọc lại phần Tiên quyết ở đầu README của chặng đó, có thể bạn đang thiếu kiến thức nền của chặng trước. Hai, tra phần Thuật ngữ cần nhớ ở cuối tệp, đôi khi chỉ là hiểu nhầm một khái niệm. Ba, tìm trên Google, Stack Overflow, arxiv với từ khóa tiếng Anh, lý do lộ trình ghi song ngữ. Bốn, hỏi AI trợ lý như ChatGPT, Claude, Gemini, DeepSeek, đây cũng là một kỹ năng cần học (chặng 72). Hỏi cụ thể, kèm code lỗi và thông báo lỗi nguyên văn. Năm, tạm dừng 1 đến 2 ngày rồi quay lại, não cần thời gian xử lý ngầm, nhiều vấn đề khó tự nhiên "bừng sáng" sau giấc ngủ.

Không có ai chấm điểm, không có deadline. Tốc độ của bạn là tốc độ của bạn. Quan trọng là đi tiếp, không phải đi nhanh.

## 6. Đánh giá bản thân

Xem [03-he-thong-danh-gia-chung-nhan.md](03-he-thong-danh-gia-chung-nhan.md) để biết cách tự đánh giá sau mỗi chặng và sau mỗi phần. Tóm tắt: mỗi chặng có một danh mục tự kiểm tra thay cho rubric chấm điểm, mỗi phần có một sản phẩm tổng kết, toàn lộ trình kết thúc bằng portfolio 170 sản phẩm.

## 7. Một số quy ước đọc

In đậm là thuật ngữ quan trọng xuất hiện lần đầu. In nghiêng là thuật ngữ tiếng Anh tương đương. Monospace là mã lệnh, tên tệp, hoặc output. Đoạn trong khối trích dẫn là định nghĩa chuẩn hoặc nguyên lý quan trọng cần ghi nhớ. Dấu sao sau tên bài tập là bài tập lõi, bắt buộc hoàn thành trước khi sang chặng sau.
