# Phần E — Machine Learning nhập môn (Chặn 101–120)

**Trạng thái: đang hoàn thiện** — khung nội dung chi tiết từng chặng có sẵn trong [ROADMAP.md](../ROADMAP.md); học liệu đầy đủ sẽ phát hành theo thứ tự sau Phần D.

## Mục tiêu phần

Học machine learning đúng quy trình kỹ thuật với **scikit-learn**: đặt bài toán, chia dữ liệu, huấn luyện, đánh giá, tinh chỉnh — với tư duy "đánh giá trung thực" xuyên suốt (overfitting, rò rỉ dữ liệu, cross-validation). Kết thúc phần, bạn có 3 notebook mô hình hoàn chỉnh và trải nghiệm cuộc thi mini theo phong cách Kaggle.

## Tiên quyết

- Đã hoàn thành Phần D (Pandas, trực quan hóa, thống kê nhập môn).
- Nếu bạn đã có kinh nghiệm ML, hãy làm bài tập cuối chặng 113 (Titanic) và 119 (cảm xúc tiếng Việt) để tự kiểm tra.

## Kết quả đầu ra chính

1. Mô hình hồi quy: dự đoán giá nhà (chặng 103–107).
2. Mô hình phân loại: Iris, Titanic (chặng 108–113) với báo cáo confusion matrix, precision/recall.
3. Phân cụm và giảm chiều: K-Means, PCA (chặng 114–115).
4. NLP nhập môn: phân tích cảm xúc tiếng Việt (chặng 118–119).
5. Cuộc thi mini Kaggle nội bộ (chặng 120) — cột mốc chứng nhận **"Kỹ sư ML tập sự"**.

## Cấu trúc 20 chặng

| Nhóm | Chặn | Chủ đề |
|------|------|--------|
| Nền tảng & hồi quy | 101–107 | Đặt bài toán, pipeline, linear regression, overfitting, regularization |
| Phân loại | 108–113 | Logistic, KNN, cây quyết định, ensemble, metric, dự án Titanic |
| Không giám sát & tinh chỉnh | 114–117 | K-Means, PCA, cross-validation, GridSearch |
| NLP & tổng kết | 118–120 | TF-IDF, cảm xúc tiếng Việt, cuộc thi mini |

## Chuẩn bị trước khi bắt đầu

- Python 3.10+ với scikit-learn, pandas, numpy, matplotlib (cài qua conda/pip).
- **Kaggle account** (miễn phí) để tải dataset.
- Khoảng 8–12 giờ mỗi tuần cho 1 chặng.
- Thư mục `portfolio-ai/phan-e/` để lưu notebook.

## Ghi chú triển khai

Phần E là phần "vượt sức ảo" phổ biến nhất của người tự học AI. Cảm giác "chạy code mẫu ra kết quả 95% accuracy" dễ khiến bạn nghĩ mình đã hiểu ML — nhưng đó là ảo giác. Đừng dán code mẫu. Hiểu mỗi dòng code, tự thay tham số, tự viết lại từ trang trắng. Một notebook bạn tự viết đạt 80% accuracy đáng giá hơn 10 notebook dán code đạt 95%.
