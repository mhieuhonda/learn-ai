# Chặn 03 — Dữ liệu và thông tin xung quanh ta

Chặn 01 bạn học AI học từ dữ liệu. Chặn 02 bạn học cách tư duy thuật toán để ra lệnh cho máy. Chặn này bạn học **chất liệu của AI** — dữ liệu. Bạn sẽ học dữ liệu là gì, các loại dữ liệu, cách thu thập, sắp xếp vào bảng, và trực quan hóa bằng biểu đồ cột. Đây là nền tảng cho mọi kỹ năng dữ liệu sau này: bảng tính (chặng 53–56), Pandas (chặng 80–87), SQL (chặng 58–60), thống kê (chặng 93–98).

Sau chặng này, bạn có thể thu thập dữ liệu một cách có kỷ luật, trình bày dữ liệu vào bảng chuẩn, và rút ra nhận xét đúng từ dữ liệu — không bịa, không phóng đại.

---

## Phần A — Kiến thức

### A.1. Dữ liệu là gì

**Dữ liệu** (*data*) là **thông tin được ghi lại dưới dạng có thể lưu trữ, truyền tải và xử lý**. Bốn dạng dữ liệu phổ biến:

| Dạng | Ví dụ |
|------|-------|
| Dữ liệu số | Cân nặng (62kg), chiều cao (1.65m), tuổi (25), nhiệt độ (28°C) |
| Dữ liệu chữ | Tên ("Nguyễn Văn A"), địa chỉ ("12 Lê Lợi"), bài thơ |
| Dữ liệu hình | Ảnh chụp, bản vẽ, chữ ký scan |
| Dữ liệu âm thanh | Ghi âm giọng nói, bài nhạc, tiếng chim hót |

**Điểm quan trọng:** thông tin "trong đầu" bạn không phải dữ liệu theo nghĩa máy tính — vì máy không tiếp cận được. Thông tin chỉ thành dữ liệu khi được **ghi lại** (trên giấy, trong tệp, trong database).

Ví dụ:
- Cân nặng của bạn "trong đầu" = không phải dữ liệu (máy không dùng được).
- Cân nặng ghi trên giấy khám bệnh = dữ liệu (máy có thể scan/đánh số).
- Cân nặng trong tệp Excel = dữ liệu (máy xử lý trực tiếp).

### A.2. Phân loại dữ liệu

Dữ liệu được phân loại theo nhiều chiều. Hai chiều quan trọng nhất:

#### A.2.1. Dữ liệu định tính vs định lượng

| Loại | Đặc điểm | Ví dụ |
|------|----------|-------|
| **Định lượng** (*quantitative*) | Đo lường được bằng số | Cân nặng, chiều cao, nhiệt độ, giá tiền |
| **Định tính** (*qualitative*) | Mô tả đặc tính, không đo lường trực tiếp | Màu sắc, giới tính, đánh giá ("tốt"/"trung bình"/"kém") |

Định lượng lại chia:
- **Liên tục** (*continuous*): có thể lấy mọi giá trị trong khoảng (cân nặng: 62.3kg, 62.35kg, 62.357kg...)
- **Rời rạc** (*discrete*): chỉ lấy giá trị đếm được (số con: 0, 1, 2, 3 — không có 2.5 con)

#### A.2.2. Dữ liệu có cấu trúc vs phi cấu trúc

| Loại | Đặc điểm | Ví dụ |
|------|----------|-------|
| **Có cấu trúc** (*structured*) | Sắp xếp theo hàng/cột, có lược đồ rõ | Bảng Excel, bảng SQL, CSV |
| **Bán cấu trúc** (*semi-structured*) | Có thẻ/nhãn nhưng không theo bảng | JSON, XML, HTML |
| **Phi cấu trúc** (*unstructured*) | Không có cấu trúc cố định | Văn bản tự do, ảnh, âm thanh, video |

80% dữ liệu thế giới hiện là phi cấu trúc (ảnh, video, văn bản). ML/DL hiện đại mạnh vì xử lý được dữ liệu phi cấu trúc. Bạn sẽ học sâu ở Phần F (CV, NLP).

### A.3. Thu thập dữ liệu — 3 quy tắc của người làm dữ liệu

Thu thập dữ liệu đúng là 80% chất lượng phân tích. Sai ở khâu này, mọi phân tích sau sai theo. Ba quy tắc:

| Quy tắc | Diễn giải | Ví dụ |
|---------|-----------|-------|
| **Đúng** | Ghi đúng ý/số người nói, không sửa theo ý mình | Người khảo sát nói "trà" không ghi thành "trà đào" |
| **Đủ** | Hỏi đủ số người đã định, không bỏ dở | Định khảo sát 10 người, không dừng ở 7 vì lười |
| **Trung thực** | Ghi đúng kết quả quan sát, không bịa | Người khảo sát trả lời "không biết" — ghi "không biết", không tự điền |

**Lưu ý về quyền riêng tư:** khi thu thập dữ liệu từ người khác, chỉ hỏi những thông tin thực sự cần cho bài toán. **Không** hỏi số điện thoại, CCCD, địa chỉ nhà trừ khi có lý do rõ ràng và được đồng ý. Đây là nền tảng đạo đức dữ liệu — sẽ học sâu ở chặng 70.

### A.4. Bias lấy mẫu (*sampling bias*)

Khi thu thập dữ liệu, bạn thường không thể hỏi **tất cả** dân số — bạn hỏi một **mẫu** (*sample*). Mẫu phải **đại diện** cho dân số, nếu không kết luận bị sai.

**Ví dụ bias lấy mẫu:**
- Muốn biết "người Việt thích thể thao gì", chỉ hỏi bạn cùng lớp → bias (mẫu chỉ là thanh niên cùng độ tuổi, không đại diện cho người già, trẻ em, người nông thôn).
- Muốn biết "ai sẽ thắng cử", chỉ gọi điện cho người có điện thoại cố định → bias (người giàu có điện thoại cố định nhiều hơn người nghèo).

**Cách tránh bias (cơ bản):**
1. Xác định dân số mục tiêu rõ ("người Việt 18+ toàn quốc")
2. Chọn mẫu sao cho mọi nhóm trong dân số đều có cơ hội được hỏi
3. Cỡ mẫu đủ lớn (thường ≥ 30 cho thống kê cơ bản; ≥ 400 cho khảo sát dân số lớn)

Bạn sẽ học sâu về lấy mẫu ở chặng 95.

### A.5. Bảng dữ liệu — cách sắp xếp dữ liệu

**Bảng** (*table*) là cách phổ biến nhất để sắp xếp dữ liệu có cấu trúc. Bảng gồm:

| Thành phần | Diễn giải |
|-----------|-----------|
| **Tiêu đề bảng** | Đặt trên cùng, mô tả bảng về cái gì |
| **Tên cột** (header) | Mô tả trường dữ liệu mỗi cột |
| **Hàng** (row) | Mỗi hàng = 1 bản ghi (1 đối tượng, 1 sự kiện) |
| **Ô** (cell) | Giao cột × hàng, chứa 1 giá trị |
| **Dòng tổng** (tùy chọn) | Tổng/Trung bình của cột số |

**Ví dụ — Bảng khảo sát nước uống yêu thích:**

| Loại nước | Số người chọn |
|-----------|---------------|
| Nước lọc | 4 |
| Nước cam | 2 |
| Trà đào | 3 |
| Sữa | 2 |
| **Tổng** | **11** |

Lý do dùng bảng:
- **Tra cứu nhanh:** "Trà đào được mấy người chọn?" — nhìn bảng trả lời tức thì.
- **So sánh:** nhìn thấy ngay loại nào nhiều nhất, ít nhất.
- **Tổng hợp:** tính tổng, trung bình bằng cách nhìn cột.

### A.6. Trực quan hóa dữ liệu — biểu đồ cột

Bảng tốt cho tra cứu, nhưng **biểu đồ** tốt hơn cho "nhìn một cái là hiểu xu hướng". Loại biểu đồ phổ biến nhất cho dữ liệu phân loại là **biểu đồ cột** (*bar chart*).

**Cách vẽ biểu đồ cột:**

1. Vẽ trục ngang (x-axis): mỗi loại dữ liệu là 1 cột, cách đều nhau.
2. Vẽ trục dọc (y-axis): thang số, từ 0 đến giá trị lớn nhất (+ biên độ).
3. Với mỗi loại, vẽ 1 cột cao bằng giá trị tương ứng.
4. Thêm tiêu đề trên cùng, nhãn trục, chú thích (nếu cần).

**Ví dụ — Biểu đồ cột cho bảng trên:**

```
Số người chọn
4 |  ■
3 |  ■       ■
2 |  ■   ■   ■   ■
1 |  ■   ■   ■   ■
0 +─────────────────
    Lọc Cam Đào Sữa
        Loại nước
```

**Đọc biểu đồ — 4 câu hỏi vàng:**
1. Cột cao nhất → loại được chọn nhiều nhất
2. Cột thấp nhất → loại ít nhất
3. So sánh 2 cột → chênh lệch bao nhiêu
4. Tổng các cột → tổng số người tham gia (phải khớp với bảng)

### A.7. Phân biệt "nhận xét từ dữ liệu" và "ý kiến cá nhân"

Đây là kỹ năng quan trọng nhất của người làm dữ liệu — và là kỹ năng nhiều người thiếu.

**Nhận xét từ dữ liệu:** câu nói có **số liệu làm bằng chứng**, rút ra từ bảng/biểu đồ.
- ✓ "Nước lọc được 4 người chọn, nhiều nhất trong nhóm."
- ✓ "Trà đào được chọn nhiều gấp 1.5 lần nước cam (3 vs 2)."
- ✓ "Tổng có 11 người tham gia khảo sát."

**Ý kiến cá nhân:** câu nói phản ánh cảm nhận, không có số liệu.
- ✗ "Nước lọc ngon nhất." (không có số liệu; "ngon" là cảm nhận)
- ✗ "Trà đào chắc chắn sẽ thắng." (dự đoán, không phải dữ liệu)
- ✗ "Nhóm này thích đồ uống lành mạnh." (suy diễn, không phải dữ liệu)

**Nguyên lý:** phân tích dữ liệu chỉ trả lời "cái gì" và "bao nhiêu" — không trả lời "tại sao" hoặc "có nên". Phân tích dữ liệu không thay thế phán đoán đạo đức hoặc quyết định giá trị.

### A.8. Vì sao dữ liệu quan trọng cho AI

Quay lại chặng 01: AI học từ dữ liệu. Hệ thống AI nào cũng cần **dữ liệu huấn luyện**:

| Hệ thống AI | Dữ liệu huấn luyện (ước lượng) |
|-------------|--------------------------------|
| FaceID điện thoại | 100+ ảnh khuôn mặt của bạn + biến đổi |
| Gợi ý YouTube | Lịch sử xem của hàng tỷ người |
| Google Dịch (EN-VI) | Hàng triệu cặp câu song ngữ |
| ChatGPT | ~500 tỷ token văn bản (khoảng 4 TB text) |
| Midjourney | ~5 tỷ cặp ảnh + chú thích |

**Hệ quả:**
- **Không có dữ liệu = không có AI.** AI không "hiểu" nếu không có dữ liệu học.
- **Dữ liệu sai = AI sai.** Dữ liệu huấn luyện có thiên vị → AI có thiên vị (chặng 69).
- **Dữ liệu ít = AI kém.** Học từ 10 ví dụ không khái quát được bằng học từ 1 triệu ví dụ.

Lộ trình sẽ quay lại dữ liệu ở mọi phần:
- Phần C (chặng 53–60): bảng tính, làm sạch, SQL
- Phần D (chặng 77–100): Pandas, thống kê, trực quan hóa
- Phần E (chặng 99, 101): feature engineering
- Phần G (chặng 141–144): dữ liệu drift, giám sát

Nền bạn đúc ngay từ chặng 03 này: **số liệu trung thực, trình bày ngay ngắn, nhận xét cẩn trọng**.

### A.9. Một câu thần chú để nhớ

> **Dữ liệu = thông tin được ghi lại. Thu thập đúng + đủ + trung thực. Bảng để tra cứu, biểu đồ để thấy xu hướng. Nhận xét phải có số liệu làm bằng chứng — không bịa, không phóng đại.**

---

## Phần B — Thực hành

### Bài 1 ★: Săn tìm 4 loại dữ liệu trong đời sống bạn

Trong 1 ngày, ghi lại ít nhất 3 ví dụ cho mỗi loại dữ liệu:

| Loại | Ví dụ của bạn |
|------|---------------|
| Số | 1. Cân nặng của tôi: 62kg<br>2. Số bước chân hôm nay: 7.234<br>3. Nhiệt độ ngoài trời: 28°C |
| Chữ | 1. Tên tôi: ...<br>2. Địa chỉ nhà: ...<br>3. Tên bài hát đang nghe: ... |
| Hình | 1. Ảnh chụp bữa trưa<br>2. Ảnh tự sướng sáng nay<br>3. Bản vẽ sơ đồ phòng |
| Âm thanh | 1. Ghi âm giọng nói của tôi<br>2. Tiếng chuông điện thoại<br>3. Bài hát đang nghe |

Lưu vào `portfolio-ai/phan-a/chặng-03-bao-cao-du-lieu/data-types.md`.

### Bài 2 ★: Khảo sát mini "Nước uống yêu thích"

Thực hiện 1 khảo sát nhỏ để thu thập dữ liệu thực.

**Câu hỏi khảo sát:** *"Trong các loại nước sau — nước lọc, nước cam, trà đào, sữa — bạn thích loại nào nhất?"*

**Quy trình:**

1. **Lên kế hoạch:** chọn 6–10 người để hỏi (bạn bè, người nhà, đồng nghiệp). Tránh bias — đừng chỉ hỏi người cùng độ tuổi.
2. **Hỏi lịch sự:** chào hỏi, giới thiệu mục đích ("Tôi đang học về dữ liệu, xin phép hỏi 1 câu"), cảm ơn sau.
3. **Ghi tally:** dùng ký hiệu đếm:

```
Nước lọc   : ||||
Nước cam   : ||
Trà đào    : |||
Sữa        : ||
```

4. **Kiểm tra chéo:** đếm lại tổng ký hiệu có bằng số người đã hỏi không? Nếu không — đếm lại, không tự thêm bớt.

### Bài 3 ★: Lập bảng dữ liệu từ khảo sát

Từ tally của Bài 2, lập bảng chuẩn:

| Loại nước | Số người chọn |
|-----------|---------------|
| Nước lọc | ? |
| Nước cam | ? |
| Trà đào | ? |
| Sữa | ? |
| **Tổng** | **?** |

Lưu vào `data-types.md`. Kiểm tra: tổng cột phải bằng tổng số người đã hỏi.

### Bài 4 ★: Vẽ biểu đồ cột trên giấy kẻ ô vuông

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

### Bài 5 ★: Viết 2 nhận xét từ dữ liệu

Từ bảng + biểu đồ, viết 2 nhận xét. Mỗi nhận xét phải **có số liệu làm bằng chứng**.

**Ví dụ nhận xét đúng:**
- "Nước lọc được 4 người chọn, nhiều nhất trong nhóm 11 người khảo sát."
- "Trà đào (3 người) gấp 1.5 lần nước cam (2 người)."

**Ví dụ nhận xét SAI (ý kiến cá nhân, không phải dữ liệu):**
- "Nước lọc ngon nhất." (cảm nhận, không có số liệu)
- "Nhóm này thích đồ uống lành mạnh." (suy diễn, không có số liệu)

Lưu vào `data-types.md`.

### Bài 6 (tùy chọn): Khảo sát câu hỏi thứ 2

Lặp lại Bài 2–5 với câu hỏi khác, ví dụ:
- *"Bạn thường xem video trên nền tảng nào nhất?"* (YouTube, TikTok, Facebook, Instagram)
- *"Bạn thường đi làm/đi học bằng phương tiện nào?"* (xem máy, xe buýt, đi bộ, ô tô)
- *"Bạn uống mấy ly nước mỗi ngày?"* (1, 2, 3, 4, 5+)

So sánh kết quả 2 khảo sát. Có mẫu hình gì thú vị không?

### Bài 7 (tùy chọn): Phát hiện bias lấy mẫu

Trong khảo sát Bài 2, trả lời:
1. Ai bạn đã hỏi? (độ tuổi, giới tính, nghề nghiệp...)
2. Nhóm này đại diện cho ai? (toàn dân Việt Nam? Thanh niên Hà Nội? Người ở nhà bạn?)
3. Nếu kết quả khảo sát được tuyên bố là "người Việt thích loại nước X nhất" — có bias không?
4. Để tránh bias, bạn cần thay đổi gì trong cách chọn người khảo sát?

Đây là nền tảng cho chặng 95 (lấy mẫu và tổng thể).

### Bài 8 (tùy chọn): Đọc 1 biểu đồ báo chí

Tìm 1 bài báo tiếng Việt có biểu đồ (VnExpress, Tuổi Trẻ thường có). Trả lời:
1. Biểu đồ loại gì? (cột, đường, tròn, area...)
2. Dữ liệu từ đâu?
3. Trục x và y thể hiện gì?
4. 2 nhận xét chính từ biểu đồ
5. Có gì đáng nghi không? (trục bị cắt, tỷ lệ không trung thực, thiếu nguồn...)

Đây là nền tảng cho chặng 91 (nguyên tắc trực quan hóa trung thực).

---

## Phần C — Sản phẩm cuối chặng

### "Báo cáo dữ liệu đầu tiên"

**Yêu cầu:** tạo tệp `portfolio-ai/phan-a/chặng-03-bao-cao-du-lieu/README.md` gồm 4 phần:

| Phần | Nội dung | Điều kiện đạt |
|------|----------|---------------|
| 1. Câu hỏi khảo sát | Viết câu hỏi bạn đã dùng + ghi ai được hỏi (nhóm, số người) | Câu hỏi rõ, có đối tượng và số người |
| 2. Bảng dữ liệu | Bảng có tiêu đề, tên cột, số liệu, dòng tổng | Đủ cấu phần; tổng khớp số người |
| 3. Biểu đồ cột | Biểu đồ vẽ (giấy scan/ảnh HOẶC vẽ trên tool) có tiêu đề, trục, cột đúng tỉ lệ | Cột đúng chiều cao theo số liệu bảng |
| 4. Hai nhận xét | 2 câu nhận xét rút ra từ dữ liệu | Mỗi câu có số liệu làm bằng chứng |

**Điểm nhấn:** Nếu bạn ghi sai số rồi sửa — tuyệt vời, đó là gỡ lỗi dữ liệu. **Đừng** sửa cho "báo cáo đẹp" — sản phẩm mục đích là sự thật, không phải thẩm mỹ.

Lưu tệp vào portfolio. Đây là artifact thứ 3 của bạn trong hành trình 170 chặng.

---

## Phần D — Tự đánh giá

Checklist cuối chặng:

```
□ Tôi hiểu dữ liệu là gì, 4 dạng dữ liệu phổ biến
□ Tôi phân biệt được dữ liệu định lượng vs định tính, có cấu trúc vs phi cấu trúc
□ Tôi biết 3 quy tắc thu thập dữ liệu (đúng, đủ, trung thực)
□ Tôi hiểu bias lấy mẫu là gì và vì sao cần tránh
□ Tôi đã làm xong Bài 1, 2, 3, 4, 5 (sao ★)
□ Tôi đã hoàn thành "Báo cáo dữ liệu đầu tiên" và lưu vào portfolio
□ Tôi phân biệt được "nhận xét từ dữ liệu" và "ý kiến cá nhân"
□ Tôi đã ghi 1 mục vào learning-journal.md cho chặng này
□ Tôi đã trả lời được "Kết nối về sau" trong tu-dien-va-tai-nguyen.md
```

Nếu 9/9 ô được đánh dấu — chúc mừng, bạn đã hoàn thành chặng 03. Phần A tiếp tục với chặng 04 (đang hoàn thiện).

---

## Phần E — Gợi ý phân tích thêm

### Tại sao không nên so sánh biểu đồ của bạn với người khác

Mỗi người khảo sát một nhóm khác nhau, nên số khác là bình thường. So sánh "biểu đồ của tôi đúng hơn của bạn" sai về tư duy — không có "đúng" tuyệt đối, chỉ có "đại diện cho nhóm nào".

### Nếu muốn khảo sát nghiêm túc hơn

Để khảo sát có giá trị thống kê:
1. Cỡ mẫu ≥ 30 (lý tưởng ≥ 100)
2. Chọn mẫu ngẫu nhiên từ dân số mục tiêu
3. Câu hỏi trung lập (không gợi ý đáp án)
4. Bảo vệ thông tin cá nhân (không hỏi tên, số điện thoại)

Bạn sẽ học kỹ thuật khảo sát nghiêm túc ở Phần D (chặng 95 — mẫu và tổng thể).

### Mở rộng — biểu đồ khác ngoài biểu đồ cột

Biểu đồ cột phù hợp dữ liệu phân loại (loại nước, thành phố, giới tính). Các loại dữ liệu khác cần loại biểu đồ khác:

| Loại dữ liệu | Biểu đồ phù hợp | Ví dụ |
|--------------|------------------|-------|
| Phân loại (ít loại) | Biểu đồ cột | Nước uống, giới tính |
| Tỷ lệ phần trăm | Biểu đồ tròn | Cơ cấu chi tiêu |
| Theo thời gian | Biểu đồ đường | Nhiệt độ 7 ngày |
| Quan hệ 2 biến | Biểu đồ phân tán (scatter) | Chiều cao vs cân nặng |
| Phân phối | Histogram | Phân bố điểm kiểm tra |

Bạn sẽ học các loại biểu đồ này ở chặng 56 (bảng tính), chặng 88–90 (Matplotlib/Seaborn).
