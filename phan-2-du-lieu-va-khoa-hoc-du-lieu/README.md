# Phần 2 — Dữ liệu và Khoa học dữ liệu (Chặng 53 đến 100)

Phần 2 gộp hai mảng vốn tách rời trước đây lại thành một mạch liền: dữ liệu và nhận thức AI (chặng 53 đến 76), rồi khoa học dữ liệu bằng Python (chặng 77 đến 100). Mục tiêu là biến dữ liệu từ "khái niệm" thành "công việc": bạn làm chủ bảng tính, cơ sở dữ liệu, SQL, sau đó chuyển sang công cụ của người làm dữ liệu thật, gồm NumPy, Pandas, Matplotlib, Seaborn, kèm nền thống kê cần thiết. Kết thúc Phần 2, bạn có một báo cáo phân tích dữ liệu end-to-end trên GitHub, từ câu hỏi đến làm sạch đến phân tích đến trực quan hóa đến kết luận.

## Mục tiêu Phần 2

Sau 48 chặng, bạn có thể làm sáu việc. Một, làm chủ bảng tính (Google Sheets), gồm công thức, biểu đồ, làm sạch, pivot table (chặng 53 đến 56). Hai, hiểu cơ sở dữ liệu, viết 10 truy vấn SQL cơ bản (chặng 58 đến 60). Ba, phân biệt AI với học máy với học sâu, học có giám sát với không giám sát, hiểu lịch sử và các lĩnh vực con (chặng 61 đến 68). Bốn, có hệ thống đạo đức số: thiên vị dữ liệu, quyền riêng tư, tin giả, deepfake, quy tắc dùng chatbot học tập trung thực (chặng 69 đến 74). Năm, làm chủ Python cho khoa học dữ liệu, gồm NumPy, Pandas, Matplotlib, Seaborn, Git, GitHub (chặng 77 đến 92). Sáu, có nền thống kê: mô tả, phân phối, lấy mẫu, xác suất, tương quan không phải nhân quả, kiểm định giả thuyết (chặng 93 đến 99).

Đích cuối của Phần 2: một báo cáo end-to-end (chặng 100) trên GitHub, kèm cột mốc "Nhà phân tích dữ liệu tập sự", cộng chứng nhận "Công dân AI thông thái".

## Cấu trúc 48 chặng

Phần 2 chia thành bốn nhóm lớn, mỗi nhóm có chủ đề rõ.

Nhóm thứ nhất là bảng tính và cơ sở dữ liệu (chặng 53 đến 60), gồm Sheets, công thức, biểu đồ, làm sạch, SQL đầu tiên. Bạn bắt đầu bằng công cụ quen thuộc (Excel, Sheets), sau đó nâng lên cơ sở dữ liệu thật (SQLite, SQL).

Nhóm thứ hai là nhận thức AI (chặng 61 đến 68), gồm lịch sử AI, phân loại khái niệm, thị giác máy, NLP, robot. Đây là lúc bạn quay lại các khái niệm ở chặng 01 với chiều sâu hơn.

Nhóm thứ ba là đạo đức và an toàn AI (chặng 69 đến 74), gồm thiên vị, riêng tư, tin giả, chatbot học tập, bản quyền, nghề nghiệp. Đây là phần tạo nên khác biệt giữa một "người dùng AI" và một "công dân AI có trách nhiệm". Đừng lướt qua dù bạn là người kỹ thuật.

Nhóm thứ tư là khoa học dữ liệu Python (chặng 77 đến 100), chi tiết tiếp theo đây.

## Khoa học dữ liệu Python (chặng 77 đến 100) chi tiết

Nhóm công cụ (chặng 77 đến 79) gồm môi trường, Git và GitHub, cấu trúc dự án chuẩn. Đây là lúc portfolio của bạn bắt đầu công khai trên GitHub.

Nhóm NumPy và Pandas (chặng 80 đến 87) gồm mảng, DataFrame, đọc, lọc, làm sạch, nhóm, và dự án bán hàng. Pandas là công cụ số một của người làm dữ liệu Python, bạn sẽ dùng nó mỗi ngày.

Nhóm trực quan hóa (chặng 88 đến 92) gồm Matplotlib, tùy chỉnh tiếng Việt, Seaborn, nguyên tắc trung thực trực quan, và dự án dashboard dữ liệu Việt Nam.

Nhóm thống kê (chặng 93 đến 99) gồm mô tả, phân phối chuẩn, lấy mẫu, xác suất, tương quan so với nhân quả, kiểm định giả thuyết, feature engineering. Đây là nền toán cần cho ML ở Phần 3.

Nhóm tổng kết (chặng 100) là báo cáo end-to-end: bạn chọn một bộ dữ liệu, đặt câu hỏi, làm sạch, phân tích, trực quan hóa, kết luận, và đẩy lên GitHub kèm README mô tả.

## Tiên quyết

Đã hoàn thành Phần 1 (chặng 01 đến 52), đặc biệt Python nền tảng (biến, điều kiện, vòng lặp, hàm, danh sách, tệp). Nếu bạn chưa học Phần 1 nhưng đã biết Python cơ bản (viết được hàm, dùng danh sách, đọc ghi tệp), hãy làm bài tập cuối chặng 60 của Phần 2 để tự kiểm tra. Qua được, bạn có thể bỏ qua Phần 1.

## Bạn cần chuẩn bị gì cho Phần 2

Về phần cứng, laptop 4 đến 8GB RAM, lý tưởng 8GB trở lên cho Pandas với dữ liệu lớn. Về phần mềm, ba công cụ chính: [Anaconda hoặc Miniconda](https://www.anaconda.com) (miễn phí) hoặc dùng [Google Colab](https://colab.research.google.com) (miễn phí, không cần cài), [VS Code](https://code.visualstudio.com) với extension Python và Jupyter, và một tài khoản [GitHub](https://github.com) miễn phí. Về tài khoản, một tài khoản Google để dùng Google Sheets và Colab. Về thời gian, khoảng 4 đến 8 giờ mỗi tuần cho 1 chặng. Về lưu trữ, thư mục `portfolio-ai/phan-2/` trên máy, công khai lên GitHub từ chặng 78.

## Ghi chú triển khai

Phần 2 là phần "vượt hầm" của lộ trình, nhiều công cụ, nhiều API, nhiều quy ước. Đừng nản nếu bạn phải tra Google 20 lần mỗi notebook. Đó là bình thường. Sau chặng 100, các API này thành phản xạ.

Phần đạo đức (chặng 69 đến 74) có vẻ "không kỹ thuật" nhưng lại quan trọng nhất về mặt hành nghề. Khi bạn đi làm, kỹ năng phân tích thiên vị dữ liệu và bảo vệ quyền riêng tư của người dùng quan trọng hơn việc viết code nhanh. Đừng lướt qua.

## Liệt kê chặng đã phát hành

Phần 2 đang hoàn thiện. Khung nội dung chi tiết từng chặng có sẵn trong [ROADMAP.md](../ROADMAP.md). Học liệu đầy đủ sẽ phát hành theo thứ tự sau Phần 1.
