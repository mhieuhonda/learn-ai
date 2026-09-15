# Phần E — Machine Learning nhập môn (Giai đoạn 101–120)

**Trạng thái: đang hoàn thiện** — khung nội dung chi tiết từng giai đoạn có sẵn trong [ROADMAP.md](../ROADMAP.md); học liệu đầy đủ sẽ phát hành theo thứ tự sau Phần D.

## Mục tiêu phần

Học machine learning đúng quy trình kỹ thuật với **scikit-learn**: đặt bài toán, chia dữ liệu, huấn luyện, đánh giá, tinh chỉnh — với tư duy "đánh giá trung thực" xuyên suốt (overfitting, rò rỉ dữ liệu, cross-validation). Kết thúc phần, người học có 3 notebook mô hình hoàn chỉnh và trải nghiệm cuộc thi mini theo phong cách Kaggle.

## Đối tượng & tiên quyết

- Đối tượng: học sinh THPT (lớp 10–11).
- Tiên quyết: Phần D (Pandas, trực quan hóa, thống kê nhập môn).

## Kết quả đầu ra chính

1. Mô hình hồi quy: dự đoán giá nhà (GĐ 103–107).
2. Mô hình phân loại: Iris, Titanic (GĐ 108–113) với báo cáo confusion matrix, precision/recall.
3. Phân cụm và giảm chiều: K-Means, PCA (GĐ 114–115).
4. NLP nhập môn: phân tích cảm xúc tiếng Việt (GĐ 118–119).
5. Cuộc thi mini Kaggle nội bộ (GĐ 120) — cột mốc chứng nhận **"Kỹ sư ML tập sự"**.

## Cấu trúc 20 giai đoạn

| Nhóm | GĐ | Chủ đề |
|------|----|--------|
| Nền tảng & hồi quy | 101–107 | Đặt bài toán, pipeline, linear regression, overfitting, regularization |
| Phân loại | 108–113 | Logistic, KNN, cây quyết định, ensemble, metric, dự án Titanic |
| Không giám sát & tinh chỉnh | 114–117 | K-Means, PCA, cross-validation, GridSearch |
| NLP & tổng kết | 118–120 | TF-IDF, cảm xúc tiếng Việt, cuộc thi mini |

## Ghi chú triển khai

- Nguyên tắc "hiểu trước khi chạy": mỗi mô hình đều bắt đầu bằng phiên bản unplugged/mini (giấy, bảng số) trước khi scikit-learn.
- Cảnh báo sớm về gian lận đánh giá: rò rỉ dữ liệu (data leakage) được dạy như "bệnh dịch" của ML — mô hình đẹp lạ phải nghi ngờ.
- Tập dữ liệu tiếng Việt: khuyến khích thu thập bình luận từ nguồn mở/khảo sát tự làm, chú ý ẩn danh hóa dữ liệu cá nhân.
