# Phần F — Deep Learning & AI hiện đại (Chặn 121–140)

**Trạng thái: đang hoàn thiện** — khung nội dung chi tiết từng chặng có sẵn trong [ROADMAP.md](../ROADMAP.md); học liệu đầy đủ sẽ phát hành theo thứ tự sau Phần E.

## Mục tiêu phần

Đi vào trái tim của AI hiện đại: **mạng nơ-ron và deep learning với PyTorch** — từ nơ-ron đơn lẻ đến CNN, RNN và kiến trúc Transformer; hiểu cách GPT/BERT vận hành; biết dùng generative AI có trách nhiệm. Kết thúc phần, bạn huấn luyện được mô hình thị giác nhận diện đặc trưng Việt Nam, xây dựng chatbot đơn giản tiếng Việt, và fine-tune một mô hình nhỏ.

## Tiên quyết

- Đã hoàn thành Phần E (quy trình ML, đánh giá mô hình).
- Nếu bạn đã có kinh nghiệm DL, hãy làm bài tập cuối chặng 125 (MNIST) và 132 (CV Việt Nam) để tự kiểm tra.

## Kết quả đầu ra chính

1. Mạng nơ-ron đầu tiên đạt 95%+ trên MNIST (chặng 125) kèm nhật ký huấn luyện.
2. Mô hình thị giác "Việt Nam của tôi": tự thu thập dữ liệu, transfer learning, đánh giá trung thực (chặng 127–132).
3. Chatbot tiếng Việt đơn giản (chặng 133–136).
4. Sơ đồ họ mô hình LLM + sản phẩm sáng tạo cùng GenAI có quy tắc (chặng 137–139).
5. Fine-tune mô hình nhỏ cho tiếng Việt (chặng 140) — cột mốc **"Nhà phát triển Deep Learning"**.

## Cấu trúc 20 chặng

| Nhóm | Chặn | Chủ đề |
|------|------|--------|
| Nền tảng DL | 121–126 | Nơ-ron, mạng đa tầng, gradient, PyTorch, MNIST, điều chỉnh huấn luyện |
| Thị giác máy tính | 127–132 | CNN, kiến trúc kinh điển, transfer learning, augmentation, YOLO, dự án CV |
| Ngôn ngữ | 133–136 | Embedding, RNN/LSTM, seq2seq, chatbot |
| Transformer & GenAI | 137–140 | Attention, BERT/GPT, generative AI, fine-tune tiếng Việt |

## Chuẩn bị trước khi bắt đầu

- Python 3.10+ với PyTorch (khuyến nghị CUDA nếu có GPU NVIDIA).
- **Google Colab** (miễn phí, có GPU T4) hoặc Kaggle Notebooks (miễn phí, có GPU P100 30h/tuần).
- Khoảng 12–16 giờ mỗi tuần cho 1 chặng.
- Thư mục `portfolio-ai/phan-f/` để lưu notebook và mô hình.

## Ghi chú triển khai

Phần F là phần khó nhất của lộ trình. Khái niệm như backpropagation, attention, embedding không "bật đèn" trong lần đầu — đó là bình thường. Đọc nhiều nguồn, vẽ nhiều hình, chạy nhiều code nhỏ. Một mẹo: khi học một kiến trúc mới (CNN, RNN, Transformer), đừng vội triển khai bằng PyTorch ngay. Viết numpy thuần trước — bạn sẽ hiểu từng phép tính. Sau đó mới dùng PyTorch để mở rộng.
