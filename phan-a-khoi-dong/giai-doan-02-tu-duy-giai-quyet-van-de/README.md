# Chặn 02 — Tư duy giải quyết vấn đề: các bước nhỏ dẫn đến thành công

Đây là chặng nền tảng quan trọng nhất của Phần A. Bạn sẽ học **tư duy máy tính** (*computational thinking*) — kỹ năng tư duy mà mọi lập trình viên, kỹ sư AI, nhà nghiên cứu đều dùng hằng ngày. Không cần máy tính; không cần biết gõ lệnh; cần duy nhất sự kiên nhẫn để phân rã việc lớn thành các bước nhỏ rõ ràng.

Sau chặng này, bạn sẽ hiểu vì sao máy tính chỉ làm đúng khi được chỉ dẫn chính xác, vì sao "đoán ý" là đặc quyền của người chứ không phải máy, và vì sao "gỡ lỗi" là kỹ năng quan trọng hơn "viết đúng ngay lần đầu".

---

## Phần A — Kiến thức

### A.1. Tư duy máy tính là gì

**Tư duy máy tính** (*computational thinking*, viết tắt **CT**) là quá trình tư duy để giải quyết vấn đề theo cách mà máy tính có thể thực hiện — gồm 4 thành phần:

| Thành phần | Tiếng Anh | Định nghĩa |
|-----------|-----------|------------|
| Phân rã | Decomposition | Chia vấn đề lớn thành các phần nhỏ dễ giải quyết |
| Mẫu hình | Pattern recognition | Tìm quy luật lặp lại trong vấn đề hoặc giữa các vấn đề |
| Trừu tượng hóa | Abstraction | Lọc thông tin quan trọng, bỏ chi tiết thừa |
| Thiết kế thuật toán | Algorithm design | Viết dãy bước rõ ràng, đúng thứ tự để giải quyết |

CT không phải "tư duy như máy" — nó là **tư duy để giao tiếp với máy**. Khi bạn giải thích một việc cho máy, bạn phải làm theo 4 bước trên vì máy không có trực giác, không có ngữ cảnh, không "đoán ý" được.

Lộ trình 170 chặng này xây toàn bộ kỹ năng AI trên nền CT — bạn sẽ gặp lại 4 thành phần này ở mọi chặng.

### A.2. Phân rã vấn đề (*decomposition*)

Một việc lớn luôn có thể chia thành các việc nhỏ hơn. **Phân rã** là kỹ năng chia việc lớn thành các phần nhỏ sao cho:

- Mỗi phần đủ nhỏ để giải quyết một mình
- Các phần có ranh giới rõ (không chồng lấn)
- Thứ tự các phần rõ ràng (nếu có phụ thuộc)
- Tổng các phần = việc lớn ban đầu

**Ví dụ — Phân rã "Tổ chức sinh nhật cho bạn":**

1. Chọn ngày tổ chức
2. Lập danh sách bạn mời
3. Viết thiệp mời và gửi
4. Đặt bánh kem
5. Chuẩn bị trò chơi
6. Trang trí phòng
7. Đón bạn đến
8. Cắt bánh và ăn
9. Dọn dẹp sau tiệc
10. Gửi lời cảm ơn

Mỗi bước trên lại có thể phân rã tiếp. Ví dụ "Đặt bánh kem":
1. Hỏi bạn thích vị gì
2. Tìm tiệm bánh gần nhà
3. Gọi điện đặt cọc
4. Đến lấy bánh đúng giờ

**Nguyên lý phân rã:** nếu một bước còn quá phức tạp để làm một lần — chưa đủ nhỏ. Phân rã tiếp cho đến khi mỗi bước bạn có thể làm trong vài phút.

**Sai lầm phổ biến khi phân rã:**
- Bước quá lớn ("chuẩn bị tiệc") — không hành động được
- Bước quá nhỏ ("mở mắt, ngồi dậy, đi đánh răng, v.v.") — quá chi tiết, mất trọng tâm
- Bước mơ hồ ("tổ chức tốt") — không có tiêu chí hoàn thành
- Thiếu bước trung gian ("mua bánh → ăn bánh" — thiếu "đặt bánh, đến lấy bánh")

### A.3. Thuật toán (*algorithm*)

**Thuật toán** (*algorithm*) là **dãy các bước rõ ràng, đúng thứ tự, có thể thực hiện được, để giải quyết một vấn đề hoặc hoàn thành một việc**.

Một dãy bước được gọi là thuật toán khi nó thỏa 4 điều kiện:

| Điều kiện | Diễn giải |
|-----------|-----------|
| Đầu vào rõ | Biết trước dữ liệu gì cần có (vd: nguyên liệu nấu mì) |
| Đầu ra rõ | Biết trước kết quả mong đợi (vd: tô mì ăn được) |
| Mỗi bước thực hiện được | Mỗi bước là hành động cụ thể, không mơ hồ |
| Dừng được | Sau hữu hạn bước, thuật toán kết thúc (không lặp vô hạn) |

**Ví dụ — Thuật toán nấu mì gói:**
1. Đun 500ml nước trong nồi đến khi sôi
2. Mở gói mì và gói gia vị
3. Khi nước sôi, thả mì vào nồi
4. Đun thêm 3 phút, khuấy nhẹ
5. Tắt bếp, đổ mì ra tô
6. Cho gói gia vị vào tô, trộn đều
7. Thưởng thức

**Thuật toán không phải duy nhất:** cùng một việc có nhiều thuật toán. Nấu mì có thể cho gia vị vào nồi trước khi tắt bếp, hoặc cho vào tô sau — cả hai đều đúng. Sự khác biệt nằm ở **trật tự bước** — đổi trật tự, đổi kết quả.

### A.4. Trật tự các bước (*sequence*)

Máy tính thực hiện lệnh theo **trật tự chính xác** như đã viết. Đổi trật tự — đổi kết quả. Đây là điểm khác biệt cốt lõi giữa giao tiếp với máy và giao tiếp với người:

- Người có thể hiểu "nấu mì rồi ăn" dù bạn nói ngược "ăn rồi nấu mì" — vì người có ngữ cảnh.
- Máy tính thực hiện đúng như bạn nói. Nếu bạn nói "ăn mì" trước "nấu mì" — máy sẽ cố ăn khi chưa có mì. Lỗi.

**Ví dụ trật tự quan trọng:** Thuật toán "sai trật tự" nấu mì:
1. Ăn mì
2. Nấu mì
3. Đun nước

Hiển nhiên vô lý — nhưng máy tính sẽ làm đúng theo thứ tự này nếu bạn ra lệnh vậy.

**Bài học:** Khi viết thuật toán cho máy, luôn tự hỏi "Trật tự này có ý nghĩa không? Đổi trật tự có ảnh hưởng kết quả không?". Đây là reflexe bạn cần rèn.

### A.5. Lệnh chính xác — máy không đoán ý

Máy tính thực hiện lệnh **đúng theo nghĩa đen** (*literal interpretation*). Nếu bạn nói "tiến đến gần cái bàn", máy sẽ hỏi: "Gần là bao nhiêu cm?". Nếu bạn nói "đi quanh phòng", máy sẽ hỏi: "Quanh theo chiều nào? Mấy bước?".

Khác với người — có thể "đoán ý" từ ngữ cảnh — máy cần **mọi lệnh đều cụ thể, đo lường được, không mơ hồ**.

**Ví dụ:** Bạn nói với trợ lý ảo "đặt báo thức sáng mai". Trợ lý sẽ hỏi:
- "Mấy giờ?"
- "Báo thức loại gì?" (chuông, nhạc, rung?)
- "Lặp lại không?"

Đây không phải vì trợ lý "ngu" — mà vì nó cần thông tin cụ thể để thực hiện. Người thì tự đoán "sáng mai chắc là 6 giờ" — nhưng đoán có thể sai.

**Nguyên lý giao tiếp với máy:**
- Lệnh cụ thể, không mơ hồ
- Số liệu rõ (khoảng cách, thời gian, số lượng)
- Điều kiện rõ ("nếu X thì làm Y, ngược lại làm Z")
- Không kỳ vọng máy "hiểu ý" khi bạn nói chung chung

Kỹ năng này trở thành phản xạ khi bạn lập trình (Phần B trở đi). Nhưng rèn ngay từ bây giờ — bằng bài tập phần B.

### A.6. Điều kiện (*condition*)

Nhiều việc thực tế không phải lúc nào cũng giống nhau. Có lúc cần quyết định: "nếu A thì làm X, nếu B thì làm Y". Đây là **điều kiện rẽ nhánh**.

**Ví dụ:** Thuật toán nấu mì có thể có điều kiện:
- **Nếu** nước chưa sôi → đợi thêm 1 phút rồi kiểm tra lại
- **Nếu** nước đã sôi → thả mì vào

Cấu trúc điều kiện phổ biến: `NẾU <điều kiện> THÌ <hành động>`. Có thể thêm `NẾU KHÔNG THÌ <hành động khác>`.

Điều kiện cho phép thuật toán **thích ứng với tình huống** thay vì chạy cứng theo một đường. Đây là nền tảng của mọi chương trình có logic phức tạp — và là khái niệm bạn sẽ viết bằng Scratch ở chặng 12, bằng Python ở chặng 29.

### A.7. Gỡ lỗi (*debugging*)

**Gỡ lỗi** (*debugging* hoặc *debug*) là quá trình tìm và sửa lỗi trong thuật toán hoặc chương trình. Đây không phải việc "xui xẻo" — đây là việc **hằng ngày** của mọi lập trình viên. Có ước tính: lập trình viên dành 50–80% thời gian gỡ lỗi, không phải viết code mới.

**Quy trình gỡ lỗi 4 bước:**

1. **Xác định triệu chứng:** kết quả sai kiểu gì? Khác mong đợi ở điểm nào?
2. **Cô lập vị trí lỗi:** bước nào trong thuật toán gây ra sai? (Chạy từng bước, kiểm tra kết quả trung gian.)
3. **Tìm nguyên nhân:** vì sao bước đó sai? (Nhập sai dữ liệu? Trật tự sai? Điều kiện sai?)
4. **Sửa và kiểm tra lại:** sửa lỗi, chạy lại toàn bộ, xác nhận kết quả đúng. Nếu vẫn sai — lặp lại quy trình.

**Ví dụ gỡ lỗi — thuật toán nấu mì bị sai:**
- Triệu chứng: mì bị nhão, không ngon
- Cô lập: bước 4 "Đun thêm 3 phút" — có thể quá lâu
- Nguyên nhân: mì gói thường chỉ cần 2 phút; 3 phút làm mì nhũn
- Sửa: đổi 3 phút thành 2 phút; nếm thử trước khi tắt bếp

**Tư duy quan trọng:** Lỗi không phải thất bại — lỗi là **dữ liệu**. Mỗi lần gặp lỗi và sửa được, bạn học thêm một "cái bẫy" để tránh sau này. Ghi lại vào `lessons-learned.md`. Vài tháng sau bạn có một kho "những cái bẫy đã qua" — tài sản quý nhất của người tự học.

### A.8. Mã giả (*pseudocode*) — viết thuật toán không cần ngôn ngữ lập trình

Trước khi viết code thật (Python, Scratch...), người ta thường viết **mã giả** (*pseudocode*) — dạng văn bản gần ngôn ngữ người, có cấu trúc gần ngôn ngữ máy. Mã giả không có cú pháp cố định; mục đích là làm rõ thuật toán trước khi hiện thực.

**Ví dụ mã giả cho "Tìm số lớn nhất trong 3 số":**

```
INPUT: a, b, c (3 số)
OUTPUT: số lớn nhất

largest = a
IF b > largest THEN
    largest = b
IF c > largest THEN
    largest = c
RETURN largest
```

Mã giả giúp bạn:
- Suy nghĩ thuật toán mà không vướng cú pháp ngôn ngữ
- Trao đổi thuật toán với người khác (không phụ thuộc ngôn ngữ lập trình)
- Chuyển sang code thật dễ hơn (mỗi dòng mã giả → 1–2 dòng code)

Từ chặng 25 (Python) trở đi, bạn sẽ viết mã giả trước khi code. Đây là thói quen quan trọng.

### A.9. Một câu thần chú để nhớ

> **Tư duy máy tính = phân rã + mẫu hình + trừu tượng hóa + thuật toán. Máy chỉ hiểu lệnh cụ thể, không đoán ý. Lỗi là dữ liệu quý — gỡ lỗi là kỹ năng hằng ngày.**

Nếu bạn viết lại được câu này bằng lời của mình mà không xem tài liệu — bạn đã hiểu phần Kiến thức.

---

## Phần B — Thực hành

### Bài 1 ★: Phân rã 3 việc hằng ngày

Chọn 3 việc từ danh sách dưới (hoặc tự chọn). Mỗi việc, phân rã thành 5–8 bước nhỏ, rõ ràng, đúng trật tự.

**Việc đề xuất:**
- Tổ chức sinh nhật cho bạn
- Đi học đúng giờ (từ lúc ngủ dậy đến lúc vào lớp)
- Làm sạch bàn học
- Nấu một món bạn biết (nếu không biết nấu, chọn việc khác)
- Mua sắm weekly ở siêu thị
- Lập kế hoạch đi du lịch 2 ngày

**Format trả lời:**
```
Việc: [tên việc]
Bước 1: [hành động cụ thể]
Bước 2: [hành động cụ thể]
...
Bước N: [hành động cụ thể]
```

Lưu vào `portfolio-ai/phan-a/chặng-02-sach-thuat-toan/decomposition.md`.

**Tiêu chí đạt:** mỗi việc ≥ 5 bước, mỗi bước là hành động cụ thể (có động từ rõ), trật tự đúng logic.

### Bài 2 ★: Sửa thuật toán "nấu mì bị hỏng"

Đây là thuật toán có 3 lỗi cài sẵn. Tìm và sửa.

```
Thuật toán nấu mì gói:

1. Đun 500ml nước trong nồi.
2. Thả mì vào nước lạnh ngay.
3. Đợi 5 phút, tắt bếp.
4. Sau đó mới mở gói gia vị bỏ vào.
5. Đổ mì ra tô và thưởng thức.
```

**Yêu cầu:**
- Gạch chân mỗi bước sai
- Viết lý do sai
- Viết lại toàn bộ thuật toán đúng
- Có thể thêm bước thiếu nếu cần

**Gợi ý:** ít nhất 3 lỗi — về trật tự, về điều kiện thiếu, về bước thiếu.

### Bài 3 ★: Trò chơi "Chỉ lệnh cho máy" — phiên bản lưới ô vuông

Trò chơi giúp bạn trải nghiệm trực tiếp việc giao tiếp với máy không đoán ý.

**Chuẩn bị:**
- 2 tờ giấy kẻ ô vuông (lưới 5×5 hoặc 8×8)
- 1 vật nhỏ làm "mục tiêu" (đồng xu, cục tẩy)
- 1 vật nhỏ làm "robot" (hòn đá, cục tẩy khác)

**Cách chơi:**

Lần 1 — bạn đóng vai "người ra lệnh":
1. Đặt "robot" ở ô góc dưới trái của tờ 1. Đặt "mục tiêu" ở một ô khác (bạn chọn).
2. Bạn giữ tờ 1 (có robot và mục tiêu). Tờ 2 để trống, đặt cạnh.
3. Bây giờ bạn sẽ chỉ lệnh cho "máy" (chính bạn, đóng vai máy) di chuyển robot đến mục tiêu — nhưng bạn không được nhìn tờ 1, chỉ dùng tờ 2 để vẽ lại vị trí robot sau mỗi lệnh.

Đây khó hơn tưởng tượng. Bạn phải ra lệnh rất cụ thể:
- "Tiến 1 ô lên trên" — cụ thể ✓
- "Tiến đến gần mục tiêu" — mơ hồ ✗ (gần là bao nhiêu ô?)
- "Rẽ phải" — cụ thể ✓
- "Đi quanh phòng" — mơ hồ ✗ (quanh theo chiều nào?)

Lần 2 — bẫy lệnh:
- Bạn cố tình ra lệnh mơ hồ và quan sát "máy" hỏi lại. Ví dụ:
  - "Đi chậm thôi" → máy: "Chậm là bao nhiêu ô/lượt?"
  - "Đi vòng qua cái bàn" → máy: "Vòng qua bên nào? Mấy bước?"
- Mục đích: rèn phản xạ viết lệnh cụ thể, không kỳ vọng máy đoán.

**Sau khi chơi, viết 2–3 dòng vào `decomposition.md`:**
- Việc gì khiến bạn nhận ra lệnh cần cụ thể?
- Một loại lệnh mơ hồ bạn thường vô tình dùng là gì?

### Bài 4 ★: Viết thuật toán có điều kiện

Chọn 1 việc từ Bài 1. Viết lại thuật toán thêm ít nhất 2 bước có điều kiện "NẾU... THÌ...".

**Ví dụ:** thuật toán "đi học đúng giờ" có thể thêm:
- NẾU trời mưa THÌ mang theo ô
- NẾU đồng hồ báo 6:45 mà chưa ăn sáng THÌ ăn nhanh bánh mì thay vì bún
- NẾU quên sách THÌ gọi điện cho mẹ nhờ mang tới

Mục đích: tập viết điều kiện — nền tảng của lập trình rẽ nhánh (chặng 12, 29).

### Bài 5 (tùy chọn): Mã giả cho "tìm số lớn nhất"

Viết mã giả (theo mẫu A.8) cho thuật toán tìm số lớn nhất trong **4 số** a, b, c, d.

Đừng xem gợi ý A.8 cho 3 số cho đến khi bạn đã thử 15 phút.

### Bài 6 (tùy chọn): Trò chơi tháp Hà Nội với 3 đĩa

Nếu có 3 đĩa kích thước khác nhau (dùng 3 đồng xu kích cỡ khác, hoặc 3 cuốn sách) và 3 cọc, thử giải bài toán tháp Hà Nội 3 đĩa:
- Đưa 3 đĩa từ cọc A sang cọc C, dùng cọc B làm trung gian
- Quy tắc: mỗi lần chỉ搬 1 đĩa, không đặt đĩa lớn lên đĩa nhỏ

Ghi lại các bước bạn làm. Đây là bài toán đệ quy kinh điển — bạn sẽ học phân tích sâu ở chặng 39.

### Bài 7 (tùy chọn): Gỡ lỗi thuật toán "đi siêu thị"

Đây là thuật toán đi siêu thị có 2 lỗi cài sẵn. Tìm và sửa.

```
Thuật toán đi siêu thị:

1. Lên danh sách cần mua.
2. Ra siêu thị, vào cửa.
3. Bỏ tất cả đồ vào giỏ mà không nhìn giá.
4. Đến quầy tính tiền, thanh toán.
5. Về nhà, cất đồ vào tủ lạnh.
```

**Lỗi tiềm năng:**
- Thiếu bước so sánh giá / chọn hàng
- Thiếu bước kiểm tra hạn sử dụng
- Thiếu bước xử lý khi hết hàng
- Thiếu bước kiểm tra túi tiền trước khi đi

Viết lại thuật toán đầy đủ.

---

## Phần C — Sản phẩm cuối chặng

### "Sách thuật toán" — 3 thuật toán của bạn

**Yêu cầu:** tạo tệp `portfolio-ai/phan-a/chặng-02-sach-thuat-toan/README.md` gồm 3 thuật toán bạn tự viết.

| Trang | Thuật toán | Điều kiện đạt |
|-------|-----------|---------------|
| 1 | Việc hằng ngày ở nhà (đánh răng, gấp chăn, tưới cây...) | 5–7 bước, đúng trật tự, mỗi bước có động từ cụ thể |
| 2 | Việc phức tạp hơn (lập kế hoạch tuần, đi siêu thị, dọn nhà...) | 6–10 bước + ít nhất 2 bước điều kiện "NẾU... THÌ..." |
| 3 | Việc bạn thực sự làm theo thuật toán của mình (nấu 1 món đơn giản, gấp máy bay giấy, lắp đồ chơi...) | 6–10 bước + đã thực sự làm theo + ghi chú ít nhất 1 chỗ bạn phải sửa (gỡ lỗi) |

**Điểm nhấn trang 3:** Bạn phải **thực sự chạy thử** thuật toán của chính mình (như chạy thử chương trình!) và ghi chú lại chỗ cần sửa. Đây là vòng đời "viết → chạy → gỡ lỗi" trong thực tế.

**Format gợi ý:**

```markdown
# Sách thuật toán của tôi

## Thuật toán 1: [tên việc]

Bước 1: ...
Bước 2: ...
...
Bước N: ...

## Thuật toán 2: [tên việc] (có điều kiện)

Bước 1: ...
Bước 2: ...
Bước 3: NẾU <điều kiện> THÌ <hành động A>, NẾU KHÔNG THÌ <hành động B>
...
Bước N: ...

## Thuật toán 3: [tên việc thực sự làm] (có gỡ lỗi)

### Bản gốc:
Bước 1: ...
...
Bước N: ...

### Đã thực hiện ngày: __/__/____

### Lỗi phát hiện khi chạy thử:
- Bước X sai vì: ...
- Bước Y thiếu vì: ...

### Bản sửa:
Bước 1: ...
...
Bước N: ...

### Bài học rút ra: [1–2 dòng]
```

Lưu tệp vào portfolio. Đây là artifact thứ 2 của bạn trong hành trình 170 chặng.

---

## Phần D — Tự đánh giá

Checklist cuối chặng:

```
□ Tôi hiểu 4 thành phần của tư duy máy tính (phân rã, mẫu hình, trừu tượng hóa, thuật toán)
□ Tôi có thể giải thích thuật toán là gì kèm 4 điều kiện
□ Tôi hiểu vì sao máy cần lệnh chính xác, không đoán ý
□ Tôi đã làm xong Bài 1, 2, 3, 4 (sao ★)
□ Tôi đã hoàn thành "Sách thuật toán" và lưu vào portfolio
□ Tôi đã thực sự "chạy thử" thuật toán trang 3 và ghi chú lỗi
□ Tôi đã ghi 1 mục vào learning-journal.md cho chặng này
□ Tôi đã trả lời được "Kết nối về sau" trong tu-dien-va-tai-nguyen.md
```

Nếu 8/8 ô được đánh dấu — chúc mừng, bạn đã hoàn thành chặng 02. Sang [Chặn 03](../giai-doan-03-du-lieu-va-thong-tin/README.md).

Nếu có ô chưa đánh dấu — đừng sang chặng sau. Trở lại phần tương ứng.

---

## Phần E — Đáp án Bài 2

**Thuật toán gốc:**
```
1. Đun 500ml nước trong nồi.
2. Thả mì vào nước lạnh ngay.
3. Đợi 5 phút, tắt bếp.
4. Sau đó mới mở gói gia vị bỏ vào.
5. Đổ mì ra tô và thưởng thức.
```

**3 lỗi:**

| Bước | Lỗi | Sửa |
|------|-----|-----|
| 2 | Thả mì vào nước lạnh — mì sẽ nhũn, không săn | Đợi nước sôi mới thả mì |
| 3 | Đợi 5 phút là quá lâu — mì thường chỉ cần 2–3 phút | Đợi 2–3 phút, khuấy nhẹ; nếm thử trước khi tắt bếp |
| Thiếu | Thiếu bước "Chuẩn bị tô, đũa" trước khi đổ mì ra | Thêm bước 0: chuẩn bị tô, đũa, gói gia vị |

**Bản sửa gợi ý:**
```
0. Chuẩn bị: nồi, 500ml nước, tô, đũa, gói mì, gói gia vị.
1. Đun 500ml nước trong nồi đến khi sôi (NẾU chưa sôi THÌ đợi thêm).
2. Khi nước sôi, mở gói mì, thả mì vào nồi.
3. Đun thêm 2–3 phút, khuấy nhẹ. NẾU mì đã mềm THÌ tắt bếp.
4. Đổ mì ra tô (đã chuẩn bị ở bước 0).
5. Cho gói gia vị vào tô, trộn đều.
6. Thưởng thức.
```

Lưu ý: có nhiều cách nấu mì đúng — đây là một. Quan trọng là đủ 4 điều kiện thuật toán: đầu vào rõ, đầu ra rõ, mỗi bước cụ thể, dừng được.
