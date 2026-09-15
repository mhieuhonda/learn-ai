# Tự đánh giá, portfolio và chứng nhận

Tài liệu này định nghĩa cách bạn tự đánh giá tiến độ, xây portfolio và — khi hoàn thành — tự cấp "chứng nhận" cho mình. Không có ai chấm điểm. Không có cơ quan nào cấp bằng. Điều duy nhất chứng minh bạn đã học được AI là **portfolio công khai** của bạn trên GitHub.

## 1. Nguyên tắc tự đánh giá

1. **Đánh giá vì sự tiến bộ, không phải để xếp loại.** Mục đích của tự đánh giá là biết bạn đã hiểu đến đâu, còn thiếu gì, cần làm lại phần nào — không phải để tự khen hay tự chê.
2. **Đa nguồn bằng chứng:** sản phẩm (file, notebook, mã), quá trình thực hiện (commit Git, lịch sử thay đổi), phần giải thích bằng văn bản (README, journal), và khả năng áp dụng ở chặng sau.
3. **Cho phép làm lại không giới hạn.** Sản phẩm chưa đạt checklist thì sửa rồi nộp lại (đẩy commit mới). Kỷ luật hoàn thiện quan trọng hơn tốc độ.
4. **Không dùng AI để làm thay sản phẩm ở mọi chặng.** AI có thể được dùng để gợi ý, kiểm tra, giải thích. Từ Phần 2 trở đi, ghi rõ phần nào mình nhờ AI hỗ trợ (trung thực học thuật là kỹ năng được đào tạo chính thức ở chặng 72).

## 2. Checklist tự kiểm tra cuối mỗi chặng

Mỗi chặng có một checklist ở cuối tệp README. Dạng tổng quát:

```
□ Tôi đã đọc toàn bộ phần Kiến thức và hiểu các khái niệm chính
□ Tôi có thể giải thích các khái niệm chính bằng lời của mình (Feynman)
□ Tôi đã làm xong các bài tập có sao trong phần Thực hành của tệp README
□ Tôi đã hoàn thành Sản phẩm cuối chặng và lưu vào portfolio
□ Tôi đã ghi nhật ký học tập (learning-journal.md) cho chặng này
□ Tôi đã trả lời được câu hỏi "Kết nối về sau" ở cuối tệp README
```

Bạn có thể in hoặc sao chép checklist này vào `learning-journal.md` sau mỗi chặng. Đánh dấu X vào mỗi ô khi đạt. Không có mức 1/2/3, chỉ có "đạt" hoặc "chưa đạt". Chưa đạt thì làm lại.

## 3. Portfolio cá nhân

Portfolio là thứ giá trị nhất bạn có sau lộ trình. Khi đi phỏng vấn, khi xin học bổng, khi thuyết phục sếp cho làm dự án AI — portfolio công khai trên GitHub nói lên tất cả. Bằng cấp thì ai cũng có thể có; portfolio thì không.

### Cấu trúc thư mục portfolio gợi ý

```
portfolio-ai/
├── README.md                          ← Giới thiệu bản thân, tóm tắt lộ trình đã đi
├── learning-journal.md                ← Nhật ký học tập theo chặng
├── lessons-learned.md                 ← Các cái bẫy đã qua
├── notes/                             ← Ghi chú theo chặng (Zettelkasten nhẹ)
│   ├── chặng-01-ai-la-gi.md
│   ├── chặng-02-thuat-toan.md
│   └── ...
├── phan-1/                            ← Sản phẩm theo phần
│   ├── chặng-01-nhat-ky-ai/
│   ├── chặng-02-sach-thuat-toan/
│   └── ... (chặng 25 đến 52 thuộc Phần 1 luôn)
├── phan-2/                            ← Sản phẩm Phần 2 (chặng 53 đến 100)
├── phan-3/                            ← Sản phẩm Phần 3 (chặng 101 đến 140)
├── phan-4/                            ← Sản phẩm Phần 4 (chặng 141 đến 170)
└── final-portfolio/                   ← Tổng kết toàn lộ trình (chặng 170)
    ├── personal-statement.md
    ├── projects-showcase.md
    └── career-roadmap.md
```

### Yêu cầu tối thiểu cho mỗi sản phẩm trong portfolio

Mỗi sản phẩm cuối chặng được lưu trong một thư mục con, gồm:

| Tệp | Mục đích |
|-----|----------|
| `README.md` | Mô tả sản phẩm: câu hỏi bài toán, cách tiếp cận, kết quả, học được gì |
| Sản phẩm chính | File `.py`, `.ipynb`, hình ảnh, v.v. tùy loại |
| (Tùy chọn) `process.md` | Quá trình thực hiện: thử gì, sai gì, sửa thế nào |

Nếu chỉ có file sản phẩm mà không có README giải thích — đó chưa phải portfolio, đó chỉ là code vứt.

## 4. Tự đánh giá cuối mỗi phần

Cuối mỗi phần (sau chặng 24, 52, 76, 100, 120, 140, 158, 170), bạn thực hiện **Bài tự đánh giá phần** gồm 4 bước:

### Bước 1: Đếm sản phẩm

Đếm số chặng trong phần bạn đã hoàn thành checklist. Mục tiêu: ít nhất 80% chặng trong phần (ví dụ Phần 1 giai đoạn khởi động có 24 chặng, tối thiểu 20 chặng đạt checklist).

### Bước 2: Dự án tổng kết

Mỗi phần có một chặng tổng kết (24, 52, 76, 100, 120, 140, 158, 170). Phải hoàn thành dự án tổng kết. Đây là bằng chứng bạn có thể tổng hợp kiến thức phần.

### Bước 3: Bài kiểm tra Feynman

Viết 1 bài 800 đến 1500 chữ tổng kết: "Tôi đã học được gì trong Phần X". Bài viết phải:
- Nêu được 5 đến 10 khái niệm chính và định nghĩa bằng lời bạn
- Cho ví dụ từ sản phẩm bạn đã làm
- Nêu 3 khó khăn lớn nhất và cách vượt qua
- Nêu 3 câu hỏi mở bạn muốn tìm hiểu tiếp

Không ai đọc bài này, bạn tự đọc lại sau 6 tháng sẽ thấy tiến bộ của mình.

### Bước 4: Cập nhật portfolio README

Cập nhật `README.md` ở thư mục gốc portfolio:
- Đánh dấu phần vừa hoàn thành
- Thêm 1 đến 2 dòng mô tả sản phẩm nổi bật nhất của phần
- Cập nhật "Kế hoạch học tiếp theo"

## 5. Chứng nhận tự cấp

Lộ trình không cấp chứng nhận chính thức. Bạn tự cấp cho mình khi đáp ứng đủ điều kiện. Chứng nhận là một mục trong `README.md` của portfolio:

```markdown
## Chứng nhận lộ trình

- ✅ Phần 1 giai đoạn khởi động — Nhà thám hiểm AI (hoàn thành ngày __/__/____)
- ⬜ Phần 1 — Lập trình viên tập sự
- ⬜ Phần 2 — Công dân AI thông thái cộng Nhà phân tích dữ liệu tập sự
- ⬜ Phần 3 — Kỹ sư ML tập sự cộng Nhà phát triển Deep Learning
- ⬜ Phần 4 — Kỹ sư AI cộng Nhà nghiên cứu AI tập sự
```

| Cột mốc | Sau chặng | Danh hiệu | Yêu cầu cốt lõi |
|---------|-----------|-----------|------------------|
| CK-1 | 24 | Nhà thám hiểm AI | Portfolio 24 sản phẩm nền cộng poster tổng kết |
| CK-1 | 52 | Lập trình viên tập sự | 2 dự án Python cộng portfolio web |
| CK-2 | 76 | Công dân AI thông thái | Dự án CSDL cộng báo cáo "AI xung quanh tôi" |
| CK-2 | 100 | Nhà phân tích dữ liệu tập sự | Báo cáo end-to-end trên GitHub |
| CK-3 | 120 | Kỹ sư ML tập sự | 3 mô hình cộng cuộc thi mini |
| CK-3 | 140 | Nhà phát triển Deep Learning | 3 mô hình DL cộng báo cáo đánh giá |
| CK-4 | 158 | Kỹ sư AI | Ứng dụng AI chạy thật cộng giám sát |
| CK-4 | 170 | Nhà nghiên cứu AI tập sự | Poster nghiên cứu cộng dự án xã hội cộng portfolio |

## 6. Mẫu nhật ký học tập

Tạo tệp `learning-journal.md` từ chặng 01. Mỗi chặng thêm một mục. Mẫu:

```markdown
# Nhật ký học tập — [Tên bạn]

## Chặng 01 — Làm quen với thế giới AI (hoàn thành __/__/____)

**Hôm nay tôi học được:**
- AI là ... (giải thích bằng lời mình, 2–3 dòng)
- 3 loại AI: hẹp, tổng quát, siêu trí tuệ
- 6 dấu chân AI trong đời sống: ...

**Khó khăn lớn nhất:** Hiểu phân biệt AI hẹp và AI tổng quát — AI tổng quát chưa tồn tại thực sự, chỉ có trong lý thuyết.

**Cách tôi vượt qua:** Đọc thêm bài "Narrow AI vs General AI" trên IBM blog; tự nhẩm lại bằng ví dụ.

**Sản phẩm đã làm:** `portfolio-ai/phan-1/chặng-01-nhat-ky-ai/` — 5 trang ghi AI trong tuần.

**Câu hỏi mở cho chặng sau:** Nếu AI học từ ví dụ, ai chọn ví dụ cho AI học? (Thấy sẽ quay lại ở chặng 69 — thiên vị dữ liệu.)

**Checklist:**
- [x] Đọc phần Kiến thức
- [x] Feynman test
- [x] Bài tập sao ★
- [x] Sản phẩm cuối chặng
- [x] Cập nhật journal
- [x] Trả lời "Kết nối về sau"
```

## 7. Khi đánh giá bản thân "chưa đạt"

Nếu checklist cuối chặng có ô chưa đánh dấu:

1. **Đừng bỏ qua.** Lát nền móng hở, nhà sau sẽ nghiêng. Đặc biệt ở Phần 1 và Phần 2, mỗi chặng là nền cho 5 đến 10 chặng sau.
2. **Xác định ô cụ thể chưa đạt.** Ví dụ: "Chưa làm bài tập 3 vì chưa hiểu đệ quy".
3. **Trở lại phần Kiến thức của chặng đó.** Đọc riêng phần liên quan đến ô chưa đạt.
4. **Làm bài tập/hoàn thiện sản phẩm.** Nếu vẫn kẹt, áp dụng "Khi gặp khó khăn" trong [02-phuong-phap-tu-hoc.md](02-phuong-phap-tu-hoc.md).
5. **Chỉ đánh dấu X khi thực sự đạt.** Tự lừa mình = tự đạp chân tại chỗ.

## 8. Một lần nữa: portfolio > chứng chỉ

Có người học xong đại học CNTT mà không code được ứng dụng 100 dòng. Có người chưa tốt nghiệp trung học mà có 50 repo GitHub chất lượng. Trong ngành AI — nơi thay đổi từng tháng — portfolio công khai là thước đo thực sự.

170 chặng này đều hướng tới việc xây portfolio cho bạn. Mỗi sản phẩm cuối chặng là một artifact. Mỗi cột mốc cuối phần là một dự án lớn. Cuối lộ trình, bạn có 170 artifact và 8 cột mốc đánh giá tổng kết. Đó là hồ sơ năng lực không cần bằng cấp chứng minh.
