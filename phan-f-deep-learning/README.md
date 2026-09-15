# Phần F — Deep Learning & AI hiện đại (Giai đoạn 121–140)

**Trạng thái: đang hoàn thiện** — khung nội dung chi tiết từng giai đoạn có sẵn trong [ROADMAP.md](../ROADMAP.md); học liệu đầy đủ sẽ phát hành theo thứ tự sau Phần E.

## Mục tiêu phần

Đi vào trái tim của AI hiện đại: **mạng nơ-ron và deep learning với PyTorch** — từ nơ-ron đơn lẻ đến CNN, RNN và kiến trúc Transformer; hiểu cách GPT/BERT vận hành; biết dùng generative AI có trách nhiệm. Kết thúc phần, người học huấn luyện được mô hình thị giác nhận diện đặc trưng Việt Nam, xây dựng chatbot đơn giản tiếng Việt, và fine-tune một mô hình nhỏ.

## Đối tượng & tiên quyết

- Đối tượng: học sinh THPT (lớp 11–12); sinh viên năm nhất.
- Tiên quyết: Phần E (quy trình ML, đánh giá mô hình).

## Kết quả đầu ra chính

1. Mạng nơ-ron đầu tiên đạt 95%+ trên MNIST (GĐ 125) kèm nhật ký huấn luyện.
2. Mô hình thị giác "Việt Nam của em": tự thu thập dữ liệu, transfer learning, đánh giá trung thực (GĐ 127–132).
3. Chatbot tiếng Việt đơn giản (GĐ 133–136).
4. Sơ đồ họ mô hình LLM + sản phẩm sáng tạo cùng GenAI có quy tắc (GĐ 137–139).
5. Fine-tune mô hình nhỏ cho tiếng Việt (GĐ 140) — cột mốc **"Nhà phát triển Deep Learning"**.

## Cấu trúc 20 giai đoạn

| Nhóm | GĐ | Chủ đề |
|------|----|--------|
| Nền tảng DL | 121–126 | Nơ-ron, mạng đa tầng, gradient, PyTorch, MNIST, điều chỉnh huấn luyện |
| Thị giác máy tính | 127–132 | CNN, kiến trúc kinh điển, transfer learning, augmentation, YOLO, dự án CV |
| Ngôn ngữ | 133–136 | Embedding, RNN/LSTM, seq2seq, chatbot |
| Transformer & GenAI | 137–140 | Attention, BERT/GPT, generative AI, fine-tune tiếng Việt |

## Ghi chú triển khai

- Nên huấn luyện trên GPU (Google Colab miễn phí); mọi notebook có chế độ "CPU-only dự phòng" để không ai bị bỏ lại.
- Nguyên tắc sức khỏe máy học: luôn bắt đầu bằng mô hình nhỏ chậm để "thấy" quá trình học, mới nâng dữ liệu/mô hình lớn.
- GenAI có trách nhiệm: GĐ 139 quy định ghi rõ nội dung nào do AI sinh, kiểm chứng mọi thông tin, không sinh nội dung mạo danh người thật.
