# Chặn 02 — Bài tập thực hành

Bài tập cho chặng 02 — tư duy máy tính và thuật toán. Bài sao ★ là bắt buộc; bài không sao là tùy chọn. Tất cả tự làm một mình.

## Bài tập 1 ★: Phân rã 3 việc hằng ngày

Chọn 3 việc từ danh sách (hoặc tự chọn). Mỗi việc, phân rã thành 5–8 bước nhỏ rõ ràng, đúng trật tự.

**Việc đề xuất:**
- Tổ chức sinh nhật cho bạn
- Đi học đúng giờ (từ lúc ngủ dậy đến lúc vào lớp)
- Làm sạch bàn học
- Nấu một món bạn biết
- Mua sắm weekly ở siêu thị
- Lập kế hoạch đi du lịch 2 ngày
- Soạn cặp sách cho ngày hôm sau
- Trả lời một email quan trọng

**Format trả lời:**

```markdown
## Việc: [tên việc]

Bước 1: [hành động cụ thể]
Bước 2: [hành động cụ thể]
...
Bước N: [hành động cụ thể]
```

Lưu vào `portfolio-ai/phan-a/chặng-02-sach-thuat-toan/decomposition.md`.

**Tiêu chí đạt:**
- Mỗi việc có 5–8 bước (không quá ngắn, không quá dài)
- Mỗi bước là hành động cụ thể (có động từ rõ)
- Trật tự đúng logic
- Không có bước mơ hồ như "chuẩn bị xong" hay "làm tốt"

## Bài tập 2 ★: Sửa thuật toán "nấu mì bị hỏng"

Thuật toán sau có 3 lỗi cài sẵn. Tìm và sửa.

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
- Viết lý do sai cho mỗi lỗi
- Viết lại toàn bộ thuật toán đúng
- Có thể thêm bước thiếu nếu cần

Gợi ý: ít nhất 3 lỗi — về trật tự, về điều kiện thiếu, về bước thiếu.

Xem đáp án ở cuối tệp `README.md` của chặng 02 — nhưng đừng xem trước khi đã thử 30 phút.

## Bài tập 3 ★: Trò chơi "Chỉ lệnh cho máy" — phiên bản lưới ô vuông

Trò chơi giúp bạn trải nghiệm trực tiếp việc giao tiếp với máy.

**Chuẩn bị:**
- 2 tờ giấy kẻ ô vuông (lưới 5×5 hoặc 8×8)
- 1 vật nhỏ làm "mục tiêu" (đồng xu, cục tẩy)
- 1 vật nhỏ làm "robot" (hòn đá, cục tẩy khác)

**Cách chơi:**

**Lần 1 — bạn đóng vai "người ra lệnh":**
1. Đặt "robot" ở ô góc dưới trái của tờ 1. Đặt "mục tiêu" ở một ô khác (bạn chọn).
2. Bạn giữ tờ 1 (có robot và mục tiêu). Tờ 2 để trống, đặt cạnh.
3. Bạn sẽ chỉ lệnh cho "máy" (chính bạn, đóng vai máy) di chuyển robot đến mục tiêu — nhưng đóng vai máy không được nhìn tờ 1, chỉ dùng tờ 2 để vẽ lại vị trí robot sau mỗi lệnh.

Lệnh phải rất cụ thể:
- "Tiến 1 ô lên trên" — cụ thể ✓
- "Tiến đến gần mục tiêu" — mơ hồ ✗
- "Rẽ phải" — cụ thể ✓
- "Đi quanh phòng" — mơ hồ ✗

**Lần 2 — bẫy lệnh:**
Bạn cố tình ra lệnh mơ hồ và quan sát "máy" hỏi lại:
- "Đi chậm thôi" → máy: "Chậm là bao nhiêu ô/lượt?"
- "Đi vòng qua cái bàn" → máy: "Vòng qua bên nào? Mấy bước?"
- "Đến gần mục tiêu" → máy: "Gần là bao nhiêu ô?"

**Sau khi chơi, viết 2–3 dòng vào `decomposition.md`:**
- Việc gì khiến bạn nhận ra lệnh cần cụ thể?
- Một loại lệnh mơ hồ bạn thường vô tình dùng là gì?

Mục đích: rèn phản xạ viết lệnh cụ thể — đây là kỹ năng nền cho lập trình từ chặng 09 trở đi.

## Bài tập 4 ★: Viết thuật toán có điều kiện

Chọn 1 việc từ Bài 1. Viết lại thuật toán thêm ít nhất 2 bước có điều kiện "NẾU... THÌ...".

**Ví dụ:** thuật toán "đi học đúng giờ" có thể thêm:
- NẾU trời mưa THÌ mang theo ô
- NẾU đồng hồ báo 6:45 mà chưa ăn sáng THÌ ăn nhanh bánh mì thay vì bún
- NẾU quên sách THÌ gọi điện cho mẹ nhờ mang tới

Mục đích: tập viết điều kiện — nền tảng của lập trình rẽ nhánh (chặng 12 Scratch, chặng 29 Python).

## Bài tập 5 (tùy chọn): Mã giả cho "tìm số lớn nhất trong 4 số"

Viết mã giả (theo mẫu A.8 trong README) cho thuật toán tìm số lớn nhất trong **4 số** a, b, c, d.

Đừng xem gợi ý mẫu cho 3 số cho đến khi bạn đã thử 15 phút.

**Gợi ý format:**
```
INPUT: a, b, c, d (4 số)
OUTPUT: số lớn nhất

largest = a
IF b > largest THEN
    largest = b
...
RETURN largest
```

## Bài tập 6 (tùy chọn): Trò chơi tháp Hà Nội với 3 đĩa

Nếu có 3 đĩa kích thước khác nhau (dùng 3 đồng xu kích cỡ khác, hoặc 3 cuốn sách) và 3 cọc, thử giải bài toán tháp Hà Nội 3 đĩa:
- Đưa 3 đĩa từ cọc A sang cọc C, dùng cọc B làm trung gian
- Quy tắc: mỗi lần chỉ搬 1 đĩa, không đặt đĩa lớn lên đĩa nhỏ

Ghi lại các bước bạn làm. Đây là bài toán đệ quy kinh điển — bạn sẽ học phân tích sâu ở chặng 39.

**Format ghi:**
```
Bước 1: chuyển đĩa nhỏ từ A sang C
Bước 2: chuyển đĩa trung từ A sang B
Bước 3: chuyển đĩa nhỏ từ C sang B
...
```

Thử với 3 đĩa (cần 7 bước). Nếu thấy dễ, thử 4 đĩa (cần 15 bước).

## Bài tập 7 (tùy chọn): Gỡ lỗi thuật toán "đi siêu thị"

Thuật toán sau có nhiều lỗi tiềm năng. Tìm và sửa.

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
- Thiếu bước xếp đồ vào túi mang về

Viết lại thuật toán đầy đủ, gồm ít nhất 1 điều kiện "NẾU... THÌ...".

## Bài tập 8 (tùy chọn): Trừu tượng hóa — vẽ sơ đồ quy trình

Chọn 1 trong 3 thuật toán bạn viết ở Bài 1. Vẽ lại thành **sơ đồ quy trình** (*flowchart*):
- Hình chữ nhật = bước hành động
- Hình thoi = điều kiện rẽ nhánh (NẾU... THÌ... / NẾU KHÔNG THÌ...)
- Mũi tên = trật tự thực hiện

Vẽ trên giấy hoặc dùng tool online miễn phí như [draw.io](https://draw.io), [mermaid.live](https://mermaid.live).

Sơ đồ quy trình là cách giao tiếp thuật toán phổ biến trong tài liệu kỹ thuật. Bạn sẽ gặp lại ở mọi chặng sau.

## Bài tập 9 (tùy chọn): Tìm mẫu hình (*pattern recognition*)

So sánh 3 quy trình hằng ngày:
- Đánh răng
- Rửa mặt
- Tắm

Tìm các bước **giống nhau** giữa 3 quy trình (mẫu hình lặp lại). Ví dụ: đều bắt đầu bằng "chuẩn bị nước", đều kết thúc bằng "lau khô".

Ghi lại các mẫu hình bạn tìm được. Đây là bước đầu của trừu tượng hóa — bạn sẽ học sâu hơn ở chặng 08.

---

## Câu hỏi tự kiểm tra

Sau khi làm xong bài tập, trả lời 4 câu:

1. Tư duy máy tính gồm 4 thành phần nào? Nêu 1 ví dụ cho mỗi thành phần.
2. Vì sao máy tính cần lệnh chính xác, không đoán ý?
3. Nêu 4 điều kiện để một dãy bước được gọi là thuật toán.
4. Bạn đang gỡ lỗi 1 thuật toán. Quy trình 4 bước là gì?

Nếu trả lời được cả 4 câu mà không cần xem tài liệu — bạn đã sẵn sàng sang chặng 03.
