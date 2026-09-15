# Phương pháp tự học AI hiệu quả

Tài liệu này tổng hợp các phương pháp tự học đã được kiểm chứng, áp dụng vào 170 chặng của lộ trình. Nếu bạn chỉ đọc một tài liệu về "cách học" trước khi bắt đầu, hãy đọc tài liệu này.

## 1. Ba trụ cột của tự học hiệu quả

**Trụ cột 1 — Hiểu trước, làm sau.** Mỗi chặng trong lộ trình mở đầu bằng phần Kiến thức: định nghĩa, cơ chế, ví dụ, lý giải. Bạn phải đọc và hiểu phần này trước khi đụng tay vào code. Nguyên lý thần kinh: não cần khung khái niệm trước thì thông tin mới (từ thực hành) mới có chỗ bám. Đảo ngược trật tự — làm trước hiểu sau — dẫn đến "thực hành mù", bạn có thể ra sản phẩm nhưng không giải thích được vì sao, và chặng sau sẽ tắc.

**Trụ cột 2 — Sản phẩm là bằng chứng hiểu.** Bạn không thực sự hiểu một khái niệm cho đến khi bạn tạo ra được một thứ bằng khái niệm đó. Mỗi chặng có một sản phẩm cuối chặng — đừng bỏ qua. Sản phẩm không cần đẹp, không cần lớn, chỉ cần đúng yêu cầu và là của bạn. Portfolio 170 sản phẩm cuối lộ trình là hồ sơ năng lực thực sự, giá trị hơn bất kỳ chứng chỉ bài thi nào.

**Trụ cột 3 — Sai là dữ liệu.** Code lỗi, mô hình cho kết quả tệ, khái niệm khó hiểu — tất cả đều là tín hiệu, không phải thất bại. Mỗi lỗi bạn gặp và hiểu nguyên nhân là một điểm dữ liệu về "cách hệ thống này vận hành". Ghi lại vào `lessons-learned.md`. Sau 50 chặng, bạn có một kho bẫy đã qua — đó là tài sản quý nhất của người tự học.

## 2. Chu trình học một chặng (45–90 phút mỗi phiên)

| Bước | Thời gian gợi ý | Hoạt động | Đầu ra |
|------|------------------|-----------|--------|
| 1. Đọc Kiến thức | 15–30 phút | Đọc chậm, ghi chú khái niệm mới bằng lời của mình | 1 trang note tay hoặc markdown |
| 2. Self-test Feynman | 5–10 phút | Đóng tài liệu, viết lại định nghĩa chính bằng lời mình | Đoạn văn 100–300 chữ |
| 3. Thực hành bài tập | 20–40 phút | Làm bài tập sao ★ trước, bài không sao sau | Code/note kết quả |
| 4. Hoàn thành sản phẩm | 15–30 phút (có thể sang phiên sau) | Sản phẩm cuối chặng, đưa vào portfolio | Artifact (file, notebook, ảnh) |
| 5. Tự đánh giá | 5 phút | Checklist tự kiểm tra ở cuối README | Đánh dấu đạt/chưa đạt |
| 6. Cập nhật nhật ký | 5 phút | Ghi vào `learning-journal.md`: học gì, khó gì, kế tiếp | Mục nhật ký mới |

Một chặng thường cần 2–4 phiên như vậy tùy độ phức tạp. Không cần hoàn thành trong một ngày.

## 3. Kỹ thuật ghi nhớ dài hạn

Tự học AI khác tự học một kỹ năng tay: bạn cần nhớ nhiều khái niệm trừu tượng trong thời gian dài (vì chặng 121 cần nhớ chặng 02). Áp dụng ba kỹ thuật sau:

### 3.1. Lặp lại ngắt quãng (Spaced repetition)

Dùng Anki (miễn phí) hoặc Mochi để tạo flashcard các thuật ngữ. Lịch lặp lại tự động: sau 1 ngày → 3 ngày → 1 tuần → 1 tháng → 3 tháng. Khi gặp một thuật ngữ mới trong chặng, tạo flashcard ngay với mặt trước là thuật ngữ + định nghĩa ngắn, mặt sau là ví dụ + chặng xuất hiện.

### 3.2. Ghi chú kép (Zettelkasten nhẹ)

Mỗi chặng tạo 1 file note trong thư mục `notes/` của portfolio. Mỗi note có:
- Tiêu đề = khái niệm chính
- 3–5 dòng định nghĩa bằng lời mình
- 2–3 link đến chặng liên quan (vd: "Xem thêm: chặng 64 — học có giám sát")
- 1 ví dụ cụ thể từ thực hành

Sau 30 chặng, bạn có một web 30 note liên kết — đây là "bộ não thứ hai" của bạn về AI.

### 3.3. Tóm tắt cuối tuần

Mỗi cuối tuần, giở lại các note của tuần và viết một đoạn 200 chữ tổng kết "Tuần này tôi học được gì quan trọng nhất". Phần này ép bạn tổng hợp, không chỉ lướt qua. Sau một năm, bạn có 52 đoạn tổng kết — đó là cuốn sách AI do chính bạn viết.

## 4. Khi gặp khái niệm khó

Một số khái niệm trong lộ trình (gradient descent, attention, p-value) nổi tiếng là khó hiểu lần đầu. Đừng bỏ cuộc. Thử theo thứ tự:

1. **Đọc lại phần Kiến thức của chặng, chậm gấp 2 lần bình thường.** Gạch chân câu nào khó, đọc lại riêng câu đó.
2. **Tìm một giải thích khác.** Đôi khi cùng một khái niệm, người giải thích khác sẽ "bật đèn". Gợi ý:
   - YouTube: 3Blue1Brown (toán học trực quan), StatQuest (thống kê), Andrej Karpathy (deep learning).
   - Blog: Jay Alammar (Transformer, embeddings), Distill.pub (trực quan ML).
   - Hỏi chatbot AI: "Giải thích gradient descent cho người mới bắt đầu, kèm 1 ví dụ số cụ thể."
3. **Lấy giấy vẽ.** Nhiều khái niệm AI trở nên rõ khi bạn vẽ: mạng nơ-ron, biểu đồ mất mát, ma trận attention. Vẽ không cần đẹp — cần đúng.
4. **Bỏ qua tạm, quay lại sau 1 tuần.** Một số khái niệm cần thời gian "ngấm". Đi tiếp chặng sau nếu chặng sau không phụ thuộc trực tiếp; quay lại khi đã có thêm ngữ cảnh.

## 5. Tự học với AI trợ lý — đúng cách

Từ Phần 2 trở đi, bạn nên dùng một trợ lý AI (ChatGPT, Claude, Gemini, DeepSeek, v.v.) như một người hướng dẫn cá nhân. Dùng đúng cách:

| Việc NÊN làm | Việc KHÔNG nên làm |
|---------------|---------------------|
| Hỏi "Tại sao code này lỗi?" kèm thông báo lỗi nguyên văn | Dán đề bài và yêu cầu AI làm giúp |
| Hỏi "Giải thích khái niệm X bằng ví dụ đời sống" | Yêu cầu AI tóm tắt toàn bộ chặng để khỏi đọc |
| Hỏi "So sánh phương pháp A và B, ưu nhược điểm" | Tin 100% câu trả lời AI mà không kiểm chứng |
| Hỏi "Gợi ý 5 hướng đi cho dự án Y" rồi tự chọn | Yêu cầu AI viết code sản phẩm cuối chặng thay mình |
| Hỏi "Phản biện luận điểm của tôi: ..." | Trích dẫn AI vào bài luận mà không ghi rõ |

Nguyên tắc: AI là người hướng dẫn, không phải người làm thay. Bạn học được khi bạn tự tay làm. Ai làm thay bạn = bạn không học.

Chi tiết về quy tắc dùng AI trong học tập: chặng 72.

## 6. Quản lý thời gian tự học

Tự học không có lớp, không có lịch cố định — đó là ưu điểm cũng là thách thức. Ba chiến lược hiệu quả:

### 6.1. Khung thời gian cố định

Chọn 2–4 khung giờ cố định trong tuần dành riêng cho học. Ví dụ: 20:00–22:00 thứ 3, 5, 7 và 9:00–12:00 Chủ nhật. Đặt lịch nhắc. Khi đến giờ, mở máy và bắt đầu — không cần "có hứng". Hứng đến sau hành động, không trước.

### 6.2. Mục tiêu tuần, không mục tiêu ngày

Cuối mỗi tuần, đặt mục tiêu tuần sau: "Hoàn thành chặng 25 và 26, làm xong 2 sản phẩm". Mục tiêu ngày linh hoạt tùy lịch. Mục tiêu tuần giúp bạn không bị rối khi một bận đột xuất.

### 6.3. Quản lý năng lượng, không quản lý thời gian

Một số chặng ở Phần 3 (Deep Learning) cần đầu óc tươi. Một số chặng ở Phần 2 (làm sạch dữ liệu) cần kiên nhẫn hơn là thông minh. Sắp xếp chặng cần sáng tạo vào giờ bạn tỉnh nhất (thường là sáng); chặng cần tỉ mỉ vào giờ bạn đang bình tĩnh hơn (chiều hoặc tối). Đừng cố học gradient descent sau khi đã làm việc 10 tiếng.

## 7. Bốn dấu hiệu bạn đang học đúng

Tự đánh giá định kỳ bằng 4 câu hỏi:

1. **Tôi có thể giải thích khái niệm vừa học cho người không biết AI không?** (Nếu không — chưa hiểu, đọc lại.)
2. **Tôi có sản phẩm cụ thể cho chặng này không?** (Nếu không — chưa hoàn thành, làm tiếp.)
3. **Tôi có ghi chú trong `learning-journal.md` về khó khăn và cách vượt qua không?** (Nếu không — đang học thụ động, ghi lại.)
4. **Tôi có muốn đọc tiếp chặng sau không?** (Nếu không — có thể bạn đang quá tải, nghỉ 1–2 ngày.)

Nếu 3/4 câu trả lời "có" — bạn đang đi đúng hướng. Tiếp tục.

## 8. Khi cần nghỉ

Burnout là rủi ro thật của tự học dài hạn. Dấu hiệu: bạn ghét mở máy, không nhớ gì vừa đọc, cáu kỉnh vô cớ. Lúc đó:

- Nghỉ 3–7 ngày hoàn toàn không đụng AI.
- Đi bộ, tập thể dục, gặp bạn bè, đọc sách không liên quan.
- Khi quay lại, bắt đầu từ chặng gần nhất bạn đã hoàn thành (không phải chặng đang dở), đọc lại phần Kiến thức để lấy đà.
- Nếu burnout kéo dài, xem lại nhịp học — có thể bạn đang ép quá nhanh. Lộ trình 170 chặng là marathon, không phải nước rút.
