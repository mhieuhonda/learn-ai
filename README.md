# Học AI — Tài liệu tự học nghiêm túc 170 chặng

Một lộ trình tự học Trí tuệ Nhân tạo từ con số không đến chuyên sâu, viết cho người đọc tự mình học — không phải cho người đi dạy. Mỗi chặng đặt kiến thức lên trước, thực hành theo sau. Toàn bộ nội dung được thiết kế để bạn làm một mình, không cần lớp học, không cần giáo viên, không cần người lớn đồng hành.

---

## Vì sao có kho tài liệu này

Trí tuệ nhân tạo đang định hình lại cách con người học, làm việc và sáng tạo. Hầu hết tài liệu hiện có rơi vào hai cực: hoặc quá hàn lâm (dành cho nghiên cứu sinh), hoặc quá rời rạc (bài blog, video ngắn không nối tiếp nhau). Kho tài liệu này lấp khoảng trống ở giữa — một con đường liền mạch **170 chặng**, mỗi chặng xây trực tiếp trên chặng trước, đi từ khái niệm nền tảng đến nghiên cứu chuyên sâu.

Toàn bộ học liệu được viết theo nguyên tắc **đọc là học được**, không phải "đọc rồi đem đi dạy cho người khác". Bạn không cần ai đồng hành, không cần lớp học, không cần giấy phép. Cần duy nhất: một máy tính kết nối mạng, sự tò mò và kỷ luật tự học.

## Triết lý thiết kế

| Nguyên tắc | Diễn giải |
|------------|-----------|
| **Kiến thức trước, thực hành sau** | Mỗi chặng mở đầu bằng khái niệm, định nghĩa, cơ chế — rồi mới đến bài tập và dự án. Bạn phải hiểu vì sao trước khi làm. |
| **Tự làm một mình** | Không có hoạt động nhóm, không có "giáo viên phát lệnh", không cần phụ huynh. Mọi bài tập đều thực hiện độc lập. |
| **Từ gần đến xa** | Mọi khái niệm mới bắt đầu từ ví dụ đời sống bạn đã gặp, rồi mới đến ký hiệu, công thức, mã giả. |
| **Lặp xoáy ốc** | Các chủ đề then chốt (dữ liệu, thuật toán, đạo đức AI) quay lại nhiều lần ở mức sâu hơn — dữ liệu xuất hiện ở chặng 03, 23, 53–60, 77–100, 141–144. |
| **An toàn và đạo đức ngay từ đầu** | An toàn số ở chặng 21–22, đạo đức AI từ Phần C trở đi và xuyên suốt đến chặng cuối. Không có chặng nào khuyến khích dùng AI để gian lận. |
| **Song ngữ thuật ngữ** | Mọi thuật ngữ ghi song ngữ Việt–Anh ngay từ đầu, vì tài liệu chuyên sâu đều bằng tiếng Anh. |
| **Sản phẩm kết thúc chặng** | Mỗi chặng kết thúc bằng một sản phẩm cụ thể (chương trình, notebook, báo cáo, mô hình) đưa vào portfolio cá nhân. |

## Bản đồ hành trình 170 chặng

| Phần | Chặng | Hành trình | Đỉnh cột mốc |
|------|-------|-----------|--------------|
| **A** | 01–24 | Khởi động: Tư duy máy tính & Thế giới số | Portfolio 24 sản phẩm nền |
| **B** | 25–52 | Lập trình nền tảng & Logic (Python, web, toán tư duy) | Portfolio Python + web cá nhân |
| **C** | 53–76 | Dữ liệu & Nhận thức AI, đạo đức số | Dự án "AI xung quanh tôi" |
| **D** | 77–100 | Python Khoa học dữ liệu (NumPy, Pandas, thống kê) | Báo cáo phân tích dữ liệu end-to-end |
| **E** | 101–120 | Machine Learning nhập môn (scikit-learn) | 3 mô hình ML + cuộc thi mini |
| **F** | 121–140 | Deep Learning & AI hiện đại (CNN, Transformer, GenAI) | Mô hình CV + chatbot + fine-tune |
| **G** | 141–158 | AI nâng cao & Triển khai (LLM, RAG, MLOps) | Ứng dụng AI triển khai thực tế |
| **H** | 159–170 | Chuyên sâu, nghiên cứu & định hướng nghề nghiệp | Portfolio nghiên cứu + dự án xã hội |

Xem chi tiết toàn bộ 170 chặng tại **[ROADMAP.md](ROADMAP.md)**.

## Cách bắt đầu

1. **Đọc [ROADMAP.md](ROADMAP.md)** để có bức tranh tổng thể 8 phần.
2. **Đọc [docs/00-huong-dan-su-dung.md](docs/00-huong-dan-su-dung.md)** để chọn điểm xuất phát phù hợp với nền tảng hiện tại của bạn.
3. **Vào chặng đầu tiên phù hợp** — người mới bắt đầu tuyệt đối vào `phan-a-khoi-dong/giai-doan-01-lam-quen-voi-the-gioi-ai/`; người đã có Python nền tảng có thể nhảy thẳng đến Phần D.
4. **Học theo trình tự trong mỗi chặng**: đọc phần Kiến thức → làm phần Thực hành → tra cứu phần Thuật ngữ → hoàn thành sản phẩm cuối chặng → tự đánh giá trước khi sang chặng kế.

## Cấu trúc kho tài liệu

```
learn-ai/
├── README.md                        ← Trang chủ (tệp này)
├── ROADMAP.md                       ← Lộ trình đầy đủ 170 chặng
├── docs/                            ← Tài liệu hướng dẫn tự học
│   ├── 00-huong-dan-su-dung.md            Cách sử dụng, các con đường tự học
│   ├── 01-chuan-hoa-va-khung-chuong-trinh.md  Ánh xạ kiến thức, tài liệu tham chiếu
│   ├── 02-phuong-phap-tu-hoc.md           Phương pháp tự học hiệu quả
│   └── 03-he-thong-danh-gia-chung-nhan.md Tự đánh giá, portfolio, chứng nhận
├── phan-a-khoi-dong/                ← Phần A (chặng 01–24)
│   └── giai-doan-01-lam-quen-voi-the-gioi-ai/
│   └── giai-doan-02-tu-duy-giai-quyet-van-de/
│   └── giai-doan-03-du-lieu-va-thong-tin/
│   └── ...
├── phan-b-lap-trinh-nen-tang/       ← Phần B (chặng 25–52)
├── phan-c-du-lieu-va-nhan-thuc-ai/  ← Phần C (chặng 53–76)
├── phan-d-python-khoa-hoc-du-lieu/  ← Phần D (chặng 77–100)
├── phan-e-machine-learning/         ← Phần E (chặng 101–120)
├── phan-f-deep-learning/            ← Phần F (chặng 121–140)
├── phan-g-ai-nang-cao-va-trien-khai/← Phần G (chặng 141–158)
└── phan-h-chuyen-sau-va-nghien-cuu/ ← Phần H (chặng 159–170)
```

Mỗi thư mục chặng hoàn chỉnh gồm 3 tệp:

| Tệp | Nội dung |
|-----|----------|
| `README.md` | Toàn bộ kiến thức của chặng: khái niệm, định nghĩa, cơ chế, ví dụ, dẫn đến bài tập và sản phẩm |
| `bai-tap-thuc-hanh.md` | Bài tập tự làm, dự án nhỏ, câu hỏi tự kiểm tra |
| `tu-dien-va-tai-nguyen.md` | Thuật ngữ Việt–Anh, tài nguyên đọc thêm, kết nối với các chặng sau |

## Tiến độ phát hành

| Phần | Chặng | Trạng thái |
|------|-------|-----------|
| A | 01–03 | **Đã phát hành nội dung chi tiết** |
| A | 04–24 | Đang hoàn thiện |
| B | 25–52 | Đang hoàn thiện |
| C | 53–76 | Đang hoàn thiện |
| D | 77–100 | Đang hoàn thiện |
| E | 101–120 | Đang hoàn thiện |
| F | 121–140 | Đang hoàn thiện |
| G | 141–158 | Đang hoàn thiện |
| H | 159–170 | Đang hoàn thiện |

## Quy ước chung

- Thuật ngữ chuyên môn ghi theo mẫu: **thuật toán** (*algorithm*).
- Đơn vị thời gian ở mỗi chặng chỉ là gợi ý cho nhịp tự học — bạn có thể nhanh hơn hoặc chậm hơn tùy khả năng, không có ai chấm điểm.
- Mọi hoạt động sử dụng công cụ AI trực tuyến đều yêu cầu bạn tự đọc điều khoản và tự chịu trách nhiệm về dữ liệu cá nhân của mình.

## Giấy phép & góp ý

Kho tài liệu phát hành với tinh thần mở cho người Việt Nam tự học AI. Khi trích dẫn hoặc sử dụng lại, vui lòng ghi rõ nguồn "Học AI — learn-ai". Mọi góp ý để cải thiện học liệu, vui lòng tạo Issue trên kho này.

**Bắt đầu hành trình của bạn tại [ROADMAP.md](ROADMAP.md).**
