# Giai đoạn 02 — Tư duy giải quyết vấn đề: các bước nhỏ dẫn đến thành công

> "Robot Bi có một bí mật nè: mình hiểu được bạn nói gì đó... nhưng chỉ khi bạn nói ĐÚNG từng bước thôi đấy! Cứ nói 'hãy nấu mì cho mình' là mình bối rối ngay. Giai đoạn này, bạn sẽ học cách nói chuyện với một người 'cứng đầu' như mình — đó chính là kỹ năng quan trọng nhất của người làm máy tính!"

## Thông tin chung

| Mục | Chi tiết |
|-----|----------|
| Mã giai đoạn | GD-02 (Phần A — Khởi động) |
| Đối tượng | Học sinh tiểu học lớp 3–5; người mới bắt đầu mọi lứa tuổi |
| Thời lượng | 2 buổi x 35 phút + 15 phút cuối tuần cùng gia đình |
| Tiên quyết | Giai đoạn 01 (biết AI học từ ví dụ; có tinh thần quan sát) |
| Nguyên liệu | Giấy A4, bút màu, 2 tờ giấy kẻ ô vuông (lưới 5x5), 1 món đồ chơi nhỏ làm "mục tiêu", mì gói/khẩu phần đồ ăn đơn giản (cho hoạt động thực tế, tùy chọn) |
| Sản phẩm cuối giai đoạn | **"Sách thuật toán của em"** — bộ 3 trang vẽ quy trình làm 3 việc hằng ngày |

## Mục tiêu học tập

**Kiến thức** — sau giai đoạn này, em có thể:
1. Phân rã một việc lớn thành các bước nhỏ theo trình tự đúng.
2. Nói được thuật toán là dãy các bước rõ ràng để làm một việc.
3. Hiểu máy tính chỉ làm đúng theo từng lệnh, không tự "đoán ý".

**Kỹ năng:**
1. Viết/mô tả quy trình từng bước bằng lời và bằng hình vẽ.
2. Tìm được lỗi (bước sai, bước thiếu, bước thừa) trong quy trình của bạn và sửa lại.

**Thái độ:**
1. Kiên nhẫn với sai sót — sai là phát hiện quý giá, sửa là tiến bộ.
2. Thích giúp bạn: khen được ý hay, góp ý được chỗ chưa rõ.

**Đối chiếu chương trình:** năng lực giải quyết vấn đề và sáng tạo (GDPT 2018); chủ đề "tổ chức thông tin, giải quyết vấn đề với sự trợ giúp của máy tính" (Tin học tiểu học).

## Vị trí của giai đoạn này trong hành trình

Giai đoạn 01 cho em biết AI **là gì**. Giai đoạn này cho em công cụ tư duy số 1 của cả ngành máy tính: **chia việc lớn thành các bước nhỏ, rõ ràng, có thứ tự** — người ta gọi đó là tư duy thuật toán. Giai đoạn 03 sẽ thêm viên gạch thứ hai: **dữ liệu**. Ba viên gạch này hợp thành nền móng cho toàn bộ 167 giai đoạn phía sau.

---

## Nội dung bài học

### Bài 1 (35 phút): Việc lớn — các bước nhỏ

**Khởi động (5 phút):** Robot Bi "giao nhiệm vụ" ngược đời: "Hãy làm giúp mình việc 'tổ chức sinh nhật cho bạn' — đi thôi!" Lớp/gia đình sẽ bối rối: tổ chức ở đâu? mời ai? mua gì? Đây là trải nghiệm: **chỉ dẫn quá chung chung thì không làm được**.

**Khám phá (15 phút) — Phân rã "bức tường khổng lồ":** Đặt câu hỏi: "Làm sao ăn hết một cái bánh rất to?" — "Cắt nhỏ ra!" Đúng vậy, mọi việc lớn đều cắt được thành các bước nhỏ. Cùng làm "máy cắt việc" cho 3 việc sau (mỗi em chọn 1, viết/vẽ thành 5–7 bước):

- *Tổ chức sinh nhật cho bạn:* chọn ngày → lập danh sách bạn mời → viết thiệp → chuẩn bị bánh và trò chơi → trang trí → đón bạn → chơi và cắt bánh → dọn dẹp và cảm ơn.
- *Đi học đúng giờ:* nghe chuông báo thức → rửa mặt, đánh răng → mặc đồng phục → ăn sáng → kiểm tra cặp sách → đi đến trường → vào lớp trước giờ học.
- *Làm sạch bàn học:* gom sách vở xếp vào ngăn → bỏ rác vào thùng → lau bụng → xếp bút vào hộp → đặt lại chỗ đèn/nước.

**Chốt (10 phút):** So sánh các bước của em với bạn bên cạnh: ai thiếu bước nào, ai thừa bước nào? Rồi Robot Bi giới thiệu khái niệm: **Phân rã** (*decomposition*) — chia việc lớn thành các việc nhỏ có thứ tự. Nửa sau của bài: gọi tên một khái niệm mới — **Thuật toán** (*algorithm*): dãy các bước rõ ràng, đúng thứ tự để hoàn thành một việc. Công thức nấu ăn, hướng dẫn lắp ghép, quy tắc an toàn giao thông — tất cả đều là thuật toán của đời sống!

### Bài 2 (35 phút): Lệnh chính xác — máy không đoán ý

**Trò chơi chính (25 phút) — "Chỉ lệnh cho Robot Bi" (phiên bản lưới ô vuông):**

1. Chuẩn bị: 2 tờ giấy kẻ lưới 5x5 đặt cạnh nhau. Em giữ tờ của mình (bản đồ) — trên đó có đặt "mục tiêu" ở ô nào đó và "Robot Bi" (hình tròn) ở ô góc.
2. Người thân/bạn cầm tờ giấy trắng (bản đồ trống), đóng vai Robot Bi — không nhìn bản đồ của em.
3. Em ra lệnh, Robot Bi làm đúng từng lệnh: "Tiến 1 ô", "Rẽ phải", "Tiến 2 ô"...
4. Kết thúc, đối chiếu 2 tờ: Robot Bi có đến đúng ô mục tiêu không?

**Lần 2 — chơi "bẫy lệnh":** Người lớn điều khiển Robot Bi cực kỳ literal: lệnh "Tiến đến gần cái ghế" → robot hỏi "Gần là bao nhiêu ô?"; lệnh "Đi quanh bàn" → "Quanh mấy bước? Đi ngược chiều nào?" Trẻ sẽ bật cười và rút ra bài học vàng: **lệnh cho máy phải chính xác, rõ ràng, không để máy đoán.**

**Chốt (10 phút):** Ba điều em vừa học — gọi tên chính thức:
- **Lệnh** (*command/instruction*): chỉ dẫn một hành động cụ thể.
- **Trình tự** (*sequence*): thứ tự các lệnh — đổi thứ tự là đổi kết quả.
- **Gỡ lỗi** (*debug*): khi Robot Bi đi sai, ta xem lại từng lệnh tìm chỗ sai rồi sửa — hành động này gọi là gỡ lỗi, và nó là công việc hằng ngày của mọi lập trình viên trên thế giới!

### Bài 3 (35 phút): Thuật toán trong đời sống — sửa lỗi thuật toán

**Hoạt động 1 (15 phút) — "Thuật toán nấu mì bị hỏng":** Đưa cho em một quy trình có cài sẵn 3 lỗi:

1. Đun 1 nồi nước lạnh.
2. Thả mì vào **nước lạnh** ngay.
3. Đợi 5 phút, tắt bếp.
4. **Sau đó mới mở gói gia vị bỏ vào.**
5. Đổ mì ra tô và thưởng thức.

Nhiệm vụ: gạch chân các bước sai/thiếu và viết lại đúng. (Lỗi: thả mì vào nước lạnh trước khi sôi; thiếu bước "chờ nước sôi"; gia vị phải cho sau khi tắt bếp hoặc trước khi múc ra tô — tùy loại mì; thiếu bước chuẩn bị tô.) Học sinh mạnh dạn có thể phát hiện thêm lỗi thiếu "chuẩn bị tô trước".

**Hoạt động 2 (15 phút) — Điều kiện xuất hiện:** Trò chuyện về các bước có "nếu... thì...": "Nếu nước chưa sôi thì đợi thêm"; "Nếu mì đã mềm thì tắt bếp". Robot Bi giải thích: máy tính xử lý được cả những bước có điều kiện này — em sẽ tự tay viết chúng bằng Scratch ở Giai đoạn 12! Trẻ ghi vào sổ: **Điều kiện** (*condition*) — bước chỉ thực hiện khi thoả "nếu...".

**Chốt (5 phút):** Lặp lại khái niệm 4 từ khóa của giai đoạn: phân rã – thuật toán – lệnh/trình tự – gỡ lỗi. Em tự đặt cho mình 1 sao cho mỗi từ nhớ được.

### Bài 4 (35 phút): Làm sách thuật toán của em

**Thực hiện sản phẩm (30 phút):** Làm "Sách thuật toán của em" gồm 3 trang (xem mục Sản phẩm). Phụ huynh/giáo viên đi vòng quanh hỗ trợ bằng câu hỏi, không thay em vẽ: "Bước này làm gì?", "Bước 3 và bước 4 đổi chỗ được không?", "Nếu em đi ngủ trước khi đánh răng thì sao?"

**Trình bày và kết (5 phút):** Mỗi em giới thiệu 1 trang sách trong 30 giây. Kết giai đoạn, Robot Bi tặng câu nói: "Người giỏi máy tính không phải người trả lời nhanh nhất — mà là người nói rõ từng bước nhất!"

---

## Sản phẩm cuối giai đoạn: "Sách thuật toán của em"

**Yêu cầu:** bộ 3 trang giấy A4 (có thể ghép thành quyển), mỗi trang một thuật toán của em:

| Trang | Thuật toán | Điều kiện đạt |
|-------|-----------|---------------|
| 1 | Việc hằng ngày ở nhà (đánh răng, gấp chăn, tưới cây...) | 5–7 bước, đúng thứ tự, có hình minh họa |
| 2 | Việc ở trường (chuẩn bị bài, làm việc nhóm, dọn lớp...) | 5–7 bước + có ít nhất 1 bước "nếu... thì..." |
| 3 | Việc em tự chọn mà có thử nghiệm thật (nấu 1 món đơn giản cùng người lớn, gấp máy bay giấy...) | 6–8 bước + đã thử làm theo chính thuật toán của em 1 lần và ghi "sửa lỗi" đã làm |

**Điểm nhấn của trang 3:** em phải **chạy thử** thuật toán của chính mình (như chạy thử chương trình!) và ghi chú lại chỗ cần sửa. Đây chính là vòng đời "viết – chạy – gỡ lỗi" trong thực tế.

## Tiêu chí đánh giá (rubric)

| Tiêu chí | Mức 1 — Cần cố gắng | Mức 2 — Đạt | Mức 3 — Tốt |
|----------|---------------------|-------------|--------------|
| Phân rã việc lớn | Còn viết theo cụm chung chung ("chuẩn bị xong") | Các bước nhỏ, rõ, đúng thứ tự | Bước chi tiết vừa đủ + tự phát hiện và ghi chú bước có thể đổi chỗ |
| Lệnh chính xác | Lệnh còn mơ hồ ("làm đẹp bàn học") | Lệnh cụ thể, máy "không cần đoán" | Tự nhận ra lệnh mơ hồ của chính mình và sửa ngay khi trình bày |
| Điều kiện "nếu... thì..." | Chưa có bước điều kiện | Có 1+ bước điều kiện hợp lý | Dùng 2+ điều kiện và giải thích được vì sao cần |
| Gỡ lỗi | Chưa phát hiện lỗi trong thuật toán mẫu | Tìm đủ 3 lỗi thuật toán nấu mì | Tìm đủ 3 lỗi + chỉ ra thêm 1 cải tiến |
| Sách thuật toán | 1–2 trang, cần hỗ trợ nhiều | Đủ 3 trang đúng yêu cầu | Đủ 3 trang + trang trí + ghi chú "sửa lỗi" có thật ở trang 3 |

## Lưu ý cho phụ huynh và giáo viên

- **Dùng ngôn ngữ của em trước, thuật ngữ sau:** giới thiệu thuật ngữ "phân rã", "thuật toán", "gỡ lỗi" chỉ sau khi em đã làm trải nghiệm xong. Tên gọi đến sau, trải nghiệm đến trước — nguyên tắc chung của cả bộ học liệu.
- **Chơi bẫy lệnh vui vẻ:** mục đích của trò chơi "bẫy lệnh" là tiếng cười, không phải trêu chọc. Người lớn điều khiển robot nên nghiêm túc "máy móc" — càng nghiêm túc càng vui.
- **An toàn thực hành:** nếu làm thuật toán nấu ăn thật, người lớn luôn cùng làm, xa lửa/nước sôi với trẻ nhỏ.
- **Đừng sửa giúp, hãy hỏi:** khi thuật toán của em có lỗi, hỏi "Chạy thử chưa? Lỗi ở bước mấy?" thay vì chỉ chỗ sai. Kỹ năng tự gỡ lỗi chỉ hình thành khi em được tự tìm.
- **Người lớn tự học:** hãy thử viết thuật toán cho một công việc chuyên môn của bạn (ví dụ: quy trình xử lý đơn hàng) theo 5–7 bước — bạn sẽ dùng kỹ năng này sớm thôi ở mọi giai đoạn lập trình phía sau.

## Bước tiếp theo

Em đã có "ngôn ngữ tư duy" của máy tính. Nhưng máy tính sống bằng gì? Bằng **dữ liệu** — số, chữ, hình ảnh, âm thanh được ghi lại. Giai đoạn 03 sẽ dạy em thu thập, sắp xếp và "đọc" dữ liệu như một nhà khoa học tí hon — và hiểu vì sao dữ liệu chính là "thức ăn" nuôi máy học mà em đã gặp ở giai đoạn 01. Hẹn gặp em ở [Giai đoạn 03: Dữ liệu và thông tin xung quanh ta](../giai-doan-03-du-lieu-va-thong-tin/README.md).
