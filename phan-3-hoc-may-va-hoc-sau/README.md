# Phần 3 — Học máy và Học sâu (Chặng 101 đến 140)

Phần 3 gộp hai mảng cốt lõi của AI hiện đại lại thành một mạch liền: học máy (chặng 101 đến 120) và học sâu (chặng 121 đến 140). Mục tiêu là đưa bạn từ "hiểu khái niệm ML" đến "xây dựng mô hình DL chạy được". Đây là phần kỹ thuật đặc nhất của lộ trình, đòi hỏi nền Python vững (Phần 1) và nền dữ liệu chắc (Phần 2). Kết thúc Phần 3, bạn có thể huấn luyện mô hình ML từ đầu, fine-tune mô hình DL có sẵn, xây dựng ứng dụng CV hoặc NLP cơ bản, và đọc hiểu được code của các thư viện PyTorch.

## Mục tiêu Phần 3

Sau 40 chặng, bạn có thể làm năm việc. Một, xây dựng pipeline ML hoàn chỉnh, từ dữ liệu thô đến mô hình đánh giá, gồm feature engineering, chia train và test, chọn thuật toán, đánh giá bằng metric phù hợp (chặng 101 đến 112). Hai, hiểu cơ chế của ba thuật toán kinh điển: hồi quy tuyến, cây quyết định, mạng nơ-ron nhân tạo (chặng 113 đến 120). Ba, xây dựng mạng nơ-ron nhân tạo bằng PyTorch, hiểu lan truyền ngược (backpropagation), huấn luyện trên MNIST (chặng 121 đến 126). Bốn, làm ứng dụng thị giác máy tính cơ bản, gồm CNN, transfer learning, augmentation, YOLO (chặng 127 đến 132). Năm, làm ứng dụng xử lý ngôn ngữ tự nhiên cơ bản, gồm embedding, RNN/LSTM, Transformer, BERT, GPT (chặng 133 đến 140).

Đích cuối của Phần 3: một dự án CV hoặc NLP end-to-end (chặng 140), kèm cột mốc "Kỹ sư AI tập sự".

## Cấu trúc 40 chặng

Phần 3 chia thành bốn nhóm lớn, mỗi nhóm có chủ đề rõ.

Nhóm thứ nhất là nền tảng học máy (chặng 101 đến 112), gồm định nghĩa chính thức ML, học có giám sát và không giám sát, học tăng cường, chia dữ liệu, overfitting và underfitting, metric đánh giá, feature engineering, ba thuật toán kinh điển, lựa chọn mô hình.

Nhóm thứ hai là thuật toán ML kinh điển (chặng 113 đến 120), gồm hồi quy tuyến, logistic, cây quyết định, rừng ngẫu nhiên, boosting, k-means, PCA, mạng nơ-ron cơ bản.

Nhóm thứ ba là nền tảng học sâu (chặng 121 đến 126), gồm nơ-ron nhân tạo, mạng đa tầng, lan truyền ngược, PyTorch cơ bản, huấn luyện MNIST, điều chỉnh hyperparameter.

Nhóm thứ tư là học sâu chuyên ngành (chặng 127 đến 140), chi tiết tiếp theo đây.

## Học sâu chuyên ngành (chặng 127 đến 140) chi tiết

Nhóm thị giác máy tính (chặng 127 đến 132) gồm CNN, kiến trúc kinh điển (ResNet, VGG), transfer learning, augmentation, YOLO, và dự án CV. Kết thúc nhóm, bạn có một mô hình nhận dạng ảnh chạy được trên dữ liệu mới.

Nhóm ngôn ngữ (chặng 133 đến 136) gồm embedding, RNN và LSTM, seq2seq, chatbot cơ bản. Bạn hiểu được vì sao ChatGPT có thể sinh văn bản mạch lạc.

Nhóm Transformer và GenAI (chặng 137 đến 140) gồm attention, BERT và GPT, generative AI, fine-tune tiếng Việt. Đây là lúc bạn chạm vào công nghệ đứng sau ChatGPT, Midjourney, và các LLM hiện đại.

## Tiên quyết

Đã hoàn thành Phần 1 và Phần 2 (Python, Pandas, thống kê cơ bản). Nếu bạn đã có kinh nghiệm ML hoặc DL, hãy làm bài tập cuối chặng 120 (ML) và 140 (DL) để tự kiểm tra. Qua được, bạn có thể bỏ qua nhóm tương ứng.

## Bạn cần chuẩn bị gì cho Phần 3

Về phần cứng, laptop 8GB RAM trở lên, lý tưởng có GPU NVIDIA. Nếu không có GPU, dùng [Google Colab Pro](https://colab.research.google.com) khoảng 150 nghìn một tháng, có GPU T4. Hoặc dùng [Kaggle Notebooks](https://www.kaggle.com/code) miễn phí với GPU P100, 30 giờ mỗi tuần.

Về phần mềm, ba công cụ chính: Python 3.10 trở lên với PyTorch, VS Code với extension Python và Jupyter, Git để version control. Về dữ liệu, các bộ dữ liệu kinh điển (MNIST, CIFAR, IMDB) đều tải miễn phí. Về thời gian, khoảng 12 đến 16 giờ mỗi tuần cho 1 chặng, đây là phần khó nhất của lộ trình. Về lưu trữ, thư mục `portfolio-ai/phan-3/` cho notebook và mô hình.

## Ghi chú triển khai

Phần 3 là phần khó nhất của lộ trình. Khái niệm như backpropagation, attention, embedding không "bật đèn" trong lần đầu. Đó là bình thường. Đọc nhiều nguồn, vẽ nhiều hình, chạy nhiều code nhỏ. Một mẹo hữu ích: khi học một kiến trúc mới (CNN, RNN, Transformer), đừng vội triển khai bằng PyTorch ngay. Viết numpy thuần trước, bạn sẽ hiểu từng phép tính. Sau đó mới dùng PyTorch để mở rộng.

## Liệt kê chặng đã phát hành

Phần 3 đang hoàn thiện. Khung nội dung chi tiết từng chặng có sẵn trong [ROADMAP.md](../ROADMAP.md). Học liệu đầy đủ sẽ phát hành theo thứ tự sau Phần 2.
