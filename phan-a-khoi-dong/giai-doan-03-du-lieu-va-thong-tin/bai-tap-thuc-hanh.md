# Chặn 03 — Bài tập thực hành

Bài tập cho chặng 03 — dữ liệu và thông tin. Bài sao ★ là bắt buộc; bài không sao là tùy chọn. Tất cả tự làm một mình.

## Bài tập 1 ★: Săn tìm 4 loại dữ liệu trong đời sống

Trong 1 ngày, ghi lại ít nhất 3 ví dụ cho mỗi loại dữ liệu:

| Loại | Ví dụ của bạn |
|------|---------------|
| Số | 1. Cân nặng của tôi: 62kg<br>2. Số bước chân hôm nay: 7.234<br>3. Nhiệt độ ngoài trời: 28°C |
| Chữ | 1. Tên tôi: ...<br>2. Địa chỉ nhà: ...<br>3. Tên bài hát đang nghe: ... |
| Hình | 1. Ảnh chụp bữa trưa<br>2. Ảnh tự sướng sáng nay<br>3. Bản vẽ sơ đồ phòng |
| Âm thanh | 1. Ghi âm giọng nói của tôi<br>2. Tiếng chuông điện thoại<br>3. Bài hát đang nghe |

Lưu vào `portfolio-ai/phan-a/chặng-03-bao-cao-du-lieu/data-types.md`.

**Tiêu chí đạt:** mỗi loại có ≥ 3 ví dụ cụ thể, không chép ví dụ mẫu.

## Bài tập 2 ★: Khảo sát mini "Nước uống yêu thích"

Thực hiện 1 khảo sát nhỏ để thu thập dữ liệu thực.

**Câu hỏi khảo sát:** *"Trong các loại nước sau — nước lọc, nước cam, trà đào, sữa — bạn thích loại nào nhất?"*

**Quy trình:**

1. **Lên kế hoạch:** chọn 6–10 người để hỏi (bạn bè, người nhà, đồng nghiệp).
2. **Hỏi lịch sự:** chào hỏi, giới thiệu mục đích, cảm ơn sau.
3. **Ghi tally:** dùng ký hiệu đếm:

```
Nước lọc   : ||||
Nước cam   : ||
Trà đào    : |||
Sữa        : ||
```

4. **Kiểm tra chéo:** đếm lại tổng ký hiệu có bằng số người đã hỏi không? Nếu không — đếm lại, không tự thêm bớt.

**Lưu ý:**
- Chỉ hỏi sở thích, **không** hỏi số điện thoại, địa chỉ nhà, CCCD — quyền riêng tư từ đầu.
- Nếu người hỏi "không biết" hoặc "thích nhiều loại", ghi theo câu trả lời, không ép chọn 1.
- Tránh bias — đừng chỉ hỏi người cùng độ tuổi, cùng giới tính, cùng nghề nghiệp.

## Bài tập 3 ★: Lập bảng dữ liệu từ khảo sát

Từ tally của Bài 2, lập bảng chuẩn:

```
Bảng: Nước uống yêu thích — khảo sát nhóm tôi

| Loại nước | Số người chọn |
|-----------|---------------|
| Nước lọc  | ?             |
| Nước cam  | ?             |
| Trà đào   | ?             |
| Sữa       | ?             |
| Tổng      | ?             |
```

Lưu vào `data-types.md`. Kiểm tra: tổng cột phải bằng tổng số người đã hỏi.

## Bài tập 4 ★: Vẽ biểu đồ cột trên giấy kẻ ô vuông

Từ bảng Bài 3, vẽ biểu đồ cột trên giấy kẻ ô vuông (hoặc dùng tool online như [datastudio.google.com](https://datastudio.google.com), Excel, Google Sheets).

**Quy trình vẽ:**
1. Vẽ trục ngang: ghi 4 tên loại nước, cách đều nhau.
2. Vẽ trục dọc bên trái: đánh số 0, 1, 2, 3, 4... (mỗi ô = 1 người).
3. Với mỗi loại nước, tô cột cao bằng số người chọn.
4. Viết tiêu đề trên cùng: "Nước uống yêu thích — khảo sát nhóm tôi".
5. Ghi "Số người" cạnh trục dọc; "Loại nước" dưới trục ngang.

**Trả lời 4 câu hỏi vàng:**
1. Loại nước nào được chọn nhiều nhất? (cột cao nhất)
2. Loại nào ít nhất?
3. Nước lọc hơn trà đào bao nhiêu người?
4. Tổng cộng có bao nhiêu người tham gia? (cộng tất cả cột — phải khớp với bảng!)

Chụp ảnh biểu đồ (nếu vẽ tay) hoặc export PDF (nếu vẽ tool), lưu vào thư mục portfolio.

## Bài tập 5 ★: Viết 2 nhận xét từ dữ liệu

Từ bảng + biểu đồ, viết 2 nhận xét. Mỗi nhận xét phải **có số liệu làm bằng chứng**.

**Ví dụ nhận xét đúng:**
- "Nước lọc được 4 người chọn, nhiều nhất trong nhóm 11 người khảo sát."
- "Trà đào (3 người) gấp 1.5 lần nước cam (2 người)."
- "Tổng có 11 người tham gia khảo sát, trong đó 4 người (36%) chọn nước lọc."

**Ví dụ nhận xét SAI (ý kiến cá nhân):**
- "Nước lọc ngon nhất." (cảm nhận, không có số liệu)
- "Trà đào chắc chắn sẽ thắng." (dự đoán, không phải dữ liệu)
- "Nhóm này thích đồ uống lành mạnh." (suy diễn, không có số liệu)

Lưu 2 nhận xét vào `data-types.md`.

## Bài tập 6 (tùy chọn): Khảo sát câu hỏi thứ 2

Lặp lại Bài 2–5 với câu hỏi khác. Gợi ý:
- *"Bạn thường xem video trên nền tảng nào nhất?"* (YouTube, TikTok, Facebook, Instagram)
- *"Bạn thường đi làm/đi học bằng phương tiện nào?"* (xe máy, xe buýt, đi bộ, ô tô)
- *"Bạn uống mấy ly nước mỗi ngày?"* (1, 2, 3, 4, 5+)
- *"Bạn thường nghe nhạc lúc nào?"* (sáng, trưa, chiều, tối, đêm)

So sánh kết quả 2 khảo sát. Có mẫu hình gì thú vị không?

## Bài tập 7 (tùy chọn): Phát hiện bias lấy mẫu

Trong khảo sát Bài 2, trả lời:

1. Ai bạn đã hỏi? (độ tuổi, giới tính, nghề nghiệp, khu vực...)
2. Nhóm này đại diện cho ai? (toàn dân Việt Nam? Thanh niên Hà Nội? Người ở nhà bạn?)
3. Nếu kết quả khảo sát được tuyên bố là "người Việt thích loại nước X nhất" — có bias không?
4. Để tránh bias, bạn cần thay đổi gì trong cách chọn người khảo sát?

Đây là nền tảng cho chặng 95 (lấy mẫu và tổng thể) và chặng 69 (thiên vị dữ liệu).

## Bài tập 8 (tùy chọn): Đọc 1 biểu đồ báo chí

Tìm 1 bài báo tiếng Việt có biểu đồ (VnExpress, Tuổi Trẻ, Zing thường có). Trả lời:

1. Biểu đồ loại gì? (cột, đường, tròn, area...)
2. Dữ liệu từ đâu?
3. Trục x và y thể hiện gì?
4. 2 nhận xét chính từ biểu đồ
5. Có gì đáng nghi không? (trục bị cắt, tỷ lệ không trung thực, thiếu nguồn...)

Đây là nền tảng cho chặng 91 (nguyên tắc trực quan hóa trung thực).

## Bài tập 9 (tùy chọn): Trừu tượng hóa dữ liệu

Bạn có bảng dữ liệu 5 cột: Tên, Tuổi, Cân nặng, Chiều cao, Nghề nghiệp. Trả lời:

1. Cột nào định lượng? Cột nào định tính?
2. Cột nào liên tục? Cột nào rời rạc?
3. Nếu chỉ được giữ 2 cột để phân tích "sức khỏe", bạn giữ cột nào? Vì sao?
4. Bỏ cột nào trước nếu muốn bảo vệ quyền riêng tư? Vì sao?

Đây là bài tập về trừu tượng hóa + đạo đức dữ liệu, nền tảng cho chặng 08 và 70.

## Bài tập 10 (tùy chọn): Tự tạo bộ dữ liệu cá nhân

Tạo một tệp CSV (dùng Notepad/VS Code) ghi lại 7 ngày dữ liệu về 1 việc bạn làm hằng ngày. Ví dụ:

```csv
ngay,buoi,gio_bd,gio_kt,phut_tap_the_thao,calo_tieu_hao
2025-09-15,sang,06:00,06:30,30,250
2025-09-16,chieu,17:00,17:45,45,380
...
```

Mở tệp CSV bằng Excel/Google Sheets. Quan sát:
- Dữ liệu có cấu trúc không?
- Có thể vẽ biểu đồ được không?
- Bias có thể có (ngày cuối tuần vs ngày thường)?

Bạn sẽ làm việc kiểu này mỗi ngày ở Phần D (Pandas).

---

## Câu hỏi tự kiểm tra

Sau khi làm xong bài tập, trả lời 4 câu:

1. Dữ liệu là gì? Nêu 4 dạng dữ liệu phổ biến kèm ví dụ.
2. Nêu 3 quy tắc thu thập dữ liệu và 1 ví dụ vi phạm mỗi quy tắc.
3. Phân biệt "nhận xét từ dữ liệu" và "ý kiến cá nhân" — kèm 1 ví dụ mỗi loại.
4. Vì sao dữ liệu quan trọng cho AI? Nêu 2 hệ quả.

Nếu trả lời được cả 4 câu mà không cần xem tài liệu — bạn đã sẵn sàng sang chặng 04 (khi phát hành).
