# Giai đoạn 03 — Dữ liệu và thông tin xung quanh ta

> "Robot Bi đói quá! Nhưng mình không ăn cơm đâu — mình ăn... DỮ LIỆU! Số, chữ, hình ảnh, âm thanh ghi lại được đều là đồ ăn của mình. Giai đoạn này, bạn sẽ học cách gom dữ liệu, xếp dữ liệu vào bảng, và vẽ biểu đồ — còn cuối cùng bạn sẽ hiểu: muốn mình khôn, cho mình dữ liệu tốt nhé!"

## Thông tin chung

| Mục | Chi tiết |
|-----|----------|
| Mã giai đoạn | GD-03 (Phần A — Khởi động) |
| Đối tượng | Học sinh tiểu học lớp 3–5; người mới bắt đầu mọi lứa tuổi |
| Thời lượng | 2 buổi x 35 phút + 15 phút cuối tuần cùng gia đình |
| Tiên quyết | Giai đoạn 01 (máy học từ ví dụ), Giai đoạn 02 (trình tự các bước) |
| Nguyên liệu | Giấy kẻ ô vuông, bút màu, thước kẻ, phiếu hỏi nhỏ (tự làm), băng keo |
| Sản phẩm cuối giai đoạn | **"Báo cáo dữ liệu đầu tiên"** — 1 bảng dữ liệu + 1 biểu đồ cột vẽ tay + 2 nhận xét |

## Mục tiêu học tập

**Kiến thức** — sau giai đoạn này, em có thể:
1. Nói được dữ liệu là thông tin được ghi lại (số, chữ, hình ảnh, âm thanh).
2. Thu thập dữ liệu bằng cách đếm, hỏi và ghi chép.
3. Sắp xếp dữ liệu vào bảng có hàng, cột, tiêu đề; đọc và vẽ biểu đồ cột đơn giản.

**Kỹ năng:**
1. Thiết kế một câu hỏi khảo sát đơn giản và thu thập trả lời từ 6–10 người.
2. Rút ra một nhận xét đúng từ dữ liệu mình thu thập.

**Thái độ:**
1. Trung thực khi ghi dữ liệu — ghi đúng số đếm được, không bịa.
2. Lịch sự khi hỏi người khác (chào, hỏi, cảm ơn).

**Đối chiếu chương trình:** môn Toán tiểu học (thống kê: thu thập, bảng, biểu đồ), môn Tin học (tổ chức thông tin), năng lực "dữ liệu và thông tin" trong Khung năng lực số.

## Vị trí của giai đoạn này trong hành trình

Giai đoạn 01 em biết máy **học từ ví dụ** — ví dụ đó chính là **dữ liệu**. Giai đoạn này em học quản lý "thức ăn" của máy: thu thập sạch, sắp xếp gọn, đọc hiểu đúng. Chủ đề dữ liệu sẽ quay lại xoáy ốc xuyên suốt lộ trình: bảng tính ở Phần C, phân tích dữ liệu ở Phần D, và feature engineering ở Phần G. Nền được đúc ngay từ đây: **số liệu trung thực, trình bày ngay ngắn, nhận xét cẩn trọng.**

---

## Nội dung bài học

### Bài 1 (35 phút): Dữ liệu là gì?

**Khởi động (5 phút):** Robot Bi đưa ra "đồ ăn" của mình để em đoán: "1,2 kilogram" (cân nặng của em), "hình bạn chụp lúc 7 tuổi", "âm thanh tiếng cười", "chữ 'Việt Nam'". Tất cả đều là dữ liệu!

**Khám phá (15 phút) — Săn tìm 4 loại dữ liệu:** Cùng liệt kê vào 4 cột trên bảng/paper:

| Dữ liệu dạng số | Dữ liệu dạng chữ | Dữ liệu dạng hình | Dữ liệu dạng âm thanh |
|------------------|-------------------|--------------------|------------------------|
| Cân nặng, chiều cao, số điện thoại (không đọc to!), tuổi | Tên, địa chỉ, bài thơ, lời bài hát | Ảnh, bản vẽ, chữ ký | Giọng nói, tiếng chim hót, bài hát |

**Điểm vàng của bài:** máy tính không phân biệt dữ liệu "đẹp xấu" — máy chỉ hiểu **dữ liệu được ghi lại**. Cân nặng ghi trên giấy là dữ liệu; cân nặng "trong đầu" thì máy không dùng được. Vì sao điều này quan trọng? Vì AI cần dữ liệu đã ghi lại để học!

**Kết nối AI (10 phút):** Quay lại 6 "dấu chân AI" ở giai đoạn 01. Hỏi: trợ lý ảo học nghe giọng từ dữ liệu gì? (hàng triệu mẫu giọng nói) — nhận dạng khuôn mặt học từ dữ liệu gì? (hàng nghìn ảnh khuôn mặt) — gợi ý video học từ dữ liệu gì? (lịch sử xem của hàng triệu người). Kết luận: **không có dữ liệu, không có AI. Dữ liệu là thức ăn của máy học.**

**Chốt (5 phút):** Em nói lại: "Dữ liệu là ______ được ghi lại" (điền: thông tin). Robot Bi khen: đúng rồi — và hôm nay mình sẽ đi gom "thức ăn"!

### Bài 2 (35 phút): Thu thập dữ liệu — dự án "Nước uống yêu thích của lớp"

**Chuẩn bị (10 phút) — Ba quy tắc của người thu thập dữ liệu:**

1. **Đúng:** ghi đúng ý/số người nói, không sửa theo ý mình.
2. **Đủ:** hỏi đủ số người đã định, không bỏ dở.
3. **Lịch sự:** chào hỏi trước, cảm ơn sau, không ép người khác trả lời.

**Thiết kế câu hỏi (5 phút):** Câu hỏi khảo sát: *"Trong các loại nước sau — nước lọc, nước cam, trà đào, sữa — bạn thích loại nào nhất?"* Lưu ý sư phạm: giới hạn 4 lựa chọn để dữ liệu gọn, dễ vẽ biểu đồ.

**Thu thập (15 phút):** Mỗi em nhận phiếu hỏi, đi hỏi 6 bạn (hoặc thành viên gia đình nếu học tại nhà). Ghi vào phiếu dạng ký hiệu đếm (tally):

```
Nước lọc   : ||||  
Nước cam   : ||
Trà đào    : |||
Sữa        : ||
```

**Kiểm tra chéo (5 phút):** Đếm lại phiếu của em: tổng số ký hiệu có đúng bằng số người đã hỏi không? Đây là kiểm tra dữ liệu đầu tiên trong đời — phụ huynh/giáo viên hỏi: "Nếu tổng không khớp thì làm sao?" (Trả lời: đi đếm lại, không tự thêm bớt!)

### Bài 3 (35 phút): Xếp dữ liệu vào bảng

**Từ ký hiệu sang bảng (15 phút):** Cùng xếp dữ liệu phiếu hỏi vào bảng chuẩn:

| Loại nước | Số bạn chọn |
|-----------|-------------|
| Nước lọc | 4 |
| Nước cam | 2 |
| Trà đào | 3 |
| Sữa | 2 |
| **Tổng** | **11** |

Đặt tên các thành phần: tiêu đề bảng (đặt trên đầu), tên cột, dòng tổng. Bảng là cách **sắp xếp** dữ liệu để nhìn một cái là hiểu — cũng giống như tủ đồ có ngăn: quần áo ở ngăn này, sách ở ngăn kia.

**Trò chơi "Tìm nhanh" (10 phút):** Che bảng đi, hỏi: "Trà đào được mấy bạn chọn?" — nhớ được không? Mở bảng: trả lời tức thì. So sánh: bảng giúp tra cứu nhanh hơn ký hiệu đếm nhiều!

**Chuyển tiếp (10 phút):** Robot Bi thắc mắc: "Mình thấy bảng rồi, nhưng mình vẫn muốn NHÌN thấy loại nào đang thắng một cách nhanh nhất cơ!" — dẫn dắt tự nhiên sang Bài 4: biểu đồ.

### Bài 4 (35 phút): Vẽ và đọc biểu đồ cột

**Vẽ biểu đồ (20 phút) trên giấy kẻ ô vuông:**

1. Vẽ trục ngang: ghi 4 tên loại nước, cách nhau đều.
2. Vẽ trục dọc bên trái: đánh số 0, 1, 2, 3, 4... (mỗi ô = 1 người).
3. Với mỗi loại nước, tô cột cao bằng số người chọn.
4. Viết tiêu đề trên cùng: "Nước uống yêu thích của nhóm em" và ghi "Số người" cạnh trục dọc.

**Đọc biểu đồ (15 phút) — bốn câu hỏi vàng:**
1. Loại nước nào được chọn nhiều nhất? (cột cao nhất)
2. Loại nào ít nhất?
3. Nước lọc hơn trà đào bao nhiêu người? (so sánh 2 cột)
4. Tổng cộng có bao nhiêu người tham gia? (cộng tất cả cột — phải khớp với bảng!)

**Kết AI (5 phút):** Robot Bi tiết lộ: "Biểu đồ em vừa vẽ chính là thứ máy tính vẽ cho người xem dữ liệu hàng ngày. Và máy học sâu hơn em tưởng từ biểu đồ: nhìn 4 cột, máy lập tức biết cột nào 'thắng' — không cần ai bảo!"

---

## Sản phẩm cuối giai đoạn: "Báo cáo dữ liệu đầu tiên"

**Yêu cầu:** 1 trang A4 (mặt trước) gồm 4 phần:

| Phần | Nội dung | Điều kiện đạt |
|------|----------|---------------|
| 1. Câu hỏi khảo sát | Viết câu hỏi em đã dùng + ghi ai được hỏi (lớp / nhóm / gia đình, số người) | Câu hỏi rõ, có đối tượng và số người |
| 2. Bảng dữ liệu | Bảng có tiêu đề, tên cột, số liệu, dòng tổng | Đủ cấu phần; tổng khớp số người |
| 3. Biểu đồ cột | Biểu đồ vẽ tay có tiêu đề, trục, cột đúng tỉ lệ | Cột đúng chiều cao theo số liệu bảng |
| 4. Hai nhận xét | 2 câu nhận xét rút ra từ dữ liệu | Mỗi câu có số liệu làm bằng chứng |

**Ví dụ nhận xét đúng:** "Nước lọc được 4 bạn chọn, nhiều nhất trong nhóm." — có số liệu làm bằng chứng. **Nhận xét cần tránh:** "Nước lọc ngon nhất" — đó là ý kiến về vị (mỗi người một gu), không phải nhận xét từ dữ liệu. Phân biệt "nhận xét từ dữ liệu" và "ý kiến cá nhân" là bài học đạo đức dữ liệu đầu tiên!

## Tiêu chí đánh giá (rubric)

| Tiêu chí | Mức 1 — Cần cố gắng | Mức 2 — Đạt | Mức 3 — Tốt |
|----------|---------------------|-------------|--------------|
| Thu thập dữ liệu | Phiếu còn thiếu, cần người lớn nhắc | Thu đủ số người, quy tắc đúng/lịch sự | Tự thiết kế thêm câu hỏi thứ 2 và thu thêm 1 bộ |
| Bảng dữ liệu | Thiếu tiêu đề hoặc tổng sai | Đủ cấu phần, số đúng | Bảng sạch + xếp hàng từ nhiều đến ít |
| Biểu đồ cột | Cột không đúng tỉ lệ | Cột đúng, đủ trục và tiêu đề | Biểu đồ đẹp + ghi chú rõ ràng cho người lạ đọc hiểu |
| Nhận xét | Ý kiến cá nhân, chưa có số liệu | 2 nhận xét có số liệu | 2 nhận xét + tự phát hiện 1 điều "dữ liệu này không nói lên được" |

## Lưu ý cho phụ huynh và giáo viên

- **Trung thực > đẹp.** Nếu em ghi sai số rồi sửa — tuyệt vời, đó là gỡ lỗi dữ liệu. Đừng bao giờ sửa giúp cho "báo cáo đẹp": sản phẩm mục đích là sự thật.
- **Bảo vệ thông tin cá nhân ngay từ bài này:** khi hỏi dữ liệu, chỉ hỏi sở thích (loại nước), **không** hỏi/ghi số điện thoại, địa chỉ nhà của bạn bè. Đây là dịp nhắc tự nhiên về thông tin cá nhân — chủ đề chính của Giai đoạn 21.
- **Không so biểu đồ của em với nhau:** mỗi em khảo sát một nhóm khác nhau nên số khác nhau là bình thường. So sánh chỉ dẫn đến "dữ liệu ai đúng hơn" sai lầm về tư duy.
- **Danh sách 4 lựa chọn nên "Việt hóa":** thay trà đào bằng nước mía, trà xanh... theo vùng miền — dữ liệu gần gũi với em hơn.
- **Người lớn tự học:** hãy làm đúng quy trình với câu hỏi công việc (ví dụ: "Thứ nào trong tuần bạn bận nhất?") — quy trình thu thập – bảng – biểu đồ – nhận xét y hệt những gì bạn sẽ làm bằng Pandas ở Giai đoạn 86–92.

## Bước tiếp theo

Em đã biết "nuôi" Robot Bi bằng dữ liệu sạch! Tiếp theo, Giai đoạn 04 sẽ cho em làm quen với người bạn số 1 của cả hành trình: **máy tính và các thiết bị số** — em sẽ hiểu máy tính gồm những gì, hệ điều hành là gì, và tập những thao tác nền tảng trước khi gặp Scratch ở Giai đoạn 09. Hẹn gặp em ở [Giai đoạn 04: Máy tính và thiết bị số](../README.md).
