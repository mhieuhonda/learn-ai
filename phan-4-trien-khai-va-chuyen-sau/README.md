# Phần 4 — Triển khai, Đạo đức và Chuyên sâu (Chặng 141 đến 170)

Phần 4 gộp hai mảng vốn tách rời trước đây lại thành một mạch liền: triển khai và ứng dụng AI (chặng 141 đến 160), rồi chuyên sâu và nghiên cứu (chặng 161 đến 170). Mục tiêu là đưa bạn từ "mô hình chạy trong notebook" đến "ứng dụng AI chạy thật cho người dùng", đồng thời chạm tới ranh giới kiến thức của lĩnh vực, đọc và tái hiện nghiên cứu khoa học, định hướng nghề nghiệp lâu dài. Kết thúc Phần 4, bạn có một ứng dụng AI hoàn chỉnh trên cloud kèm giám sát, một portfolio tổng 170 sản phẩm, và một bản định hướng nghề nghiệp trung thực về việc dùng AI trong 5 đến 10 năm tiếp theo.

## Mục tiêu Phần 4

Sau 30 chặng, bạn có thể làm sáu việc. Một, xây pipeline ML chuyên nghiệp xử lý dữ liệu lệch, có báo cáo giải thích mô hình (chặng 141 đến 143). Hai, làm ứng dụng LLM hiện đại, gồm prompt engineering chuyên sâu, API, embeddings, RAG, agent (chặng 146 đến 151). Ba, triển khai ứng dụng AI end-to-end bằng Docker, FastAPI, CI/CD, MLflow, cloud (chặng 152 đến 158). Bốn, chọn chuyên ngành có phương pháp (CV, NLP, RL, mô hình sinh) và làm dự án chuyên ngành (chặng 159 đến 163). Năm, đọc và tái hiện nghiên cứu khoa học, viết và trình bày khoa học (chặng 164 đến 167). Sáu, đóng góp mã nguồn mở, làm dự án AI vì cộng đồng (chặng 168 đến 170).

Đích cuối của Phần 4: một ứng dụng AI end-to-end (chặng 158) cộng một portfolio tổng (chặng 170) cộng một personal statement về định hướng nghề nghiệp. Cột mốc "Kỹ sư AI" (chặng 158) và "Nhà nghiên cứu AI tập sự" (chặng 170).

## Cấu trúc 30 chặng

Phần 4 chia thành bốn nhóm lớn, mỗi nhóm có chủ đề rõ.

Nhóm thứ nhất là ML nâng cao (chặng 141 đến 145), gồm feature engineering chuyên sâu, xử lý dữ liệu lệch (imbalanced data), giải thích mô hình bằng SHAP và LIME, giám sát drift, AutoML. Đây là lúc bạn học các kỹ thuật mà người làm ML thực sự cần khi làm việc với dữ liệu thật.

Nhóm thứ hai là LLM và ứng dụng (chặng 146 đến 151), gồm prompt engineering chuyên sâu, gọi LLM API, vector database, RAG (retrieval-augmented generation), agent, trợ lý học tập tiếng Việt. Đây là phần mới nhất của lộ trình, cập nhật với công nghệ 2024 đến 2025.

Nhóm thứ ba là MLOps và cloud (chặng 152 đến 158), gồm Docker, FastAPI, CI/CD, MLflow, cloud (AWS, GCP, Azure), bảo mật, dự án end-to-end. Đây là phần nhiều người tự học bỏ qua, nhưng lại là kỹ năng nhà tuyển dụng ai cũng cần.

Nhóm thứ tư là chuyên sâu và nghiên cứu (chặng 161 đến 170), chi tiết tiếp theo đây.

## Chuyên sâu và nghiên cứu (chặng 161 đến 170) chi tiết

Nhóm chọn hướng (chặng 159) là bản đồ chuyên ngành, bạn chọn một trong bốn hướng: computer vision chuyên sâu, NLP và LLM, reinforcement learning, mô hình sinh.

Nhóm chuyên ngành (chặng 160 đến 163) đi sâu vào hướng bạn chọn. CV chuyên sâu gồm object detection nâng cao, segment image, video AI. NLP và LLM gồm tối ưu hóa attention, fine-tune LLM với LoRA, RLHF. RL gồm Q-learning, PPO, môi trường. Mô hình sinh gồm diffusion, GAN.

Nhóm nghiên cứu (chặng 164 đến 167) gồm đọc paper, tái hiện nghiên cứu, phương pháp nghiên cứu, viết và trình bày khoa học. Bạn viết một bản tóm tắt 1 paper, một báo cáo tái hiện, một đề cương nghiên cứu, một poster.

Nhóm cộng đồng và tổng kết (chặng 168 đến 170) gồm Kaggle và đóng góp mã nguồn mở, dự án AI vì cộng đồng, và portfolio tổng. Portfolio tổng yêu cầu bạn viết personal statement: "Tôi là ai, tôi đã học gì, tôi muốn đi đâu". Câu trả lời không cần hoàn hảo, nhưng cần trung thực.

## Tiên quyết

Đã hoàn thành Phần 3 (ML và DL). Nếu bạn đã có kinh nghiệm triển khai ML hoặc nghiên cứu, hãy làm bài tập cuối chặng 149 (RAG) và 158 (end-to-end) để tự kiểm tra. Qua được, bạn có thể bỏ qua nhóm tương ứng.

## Bạn cần chuẩn bị gì cho Phần 4

Về phần cứng, laptop 8GB RAM trở lên cộng Docker. Nếu làm DL chuyên sâu, cần GPU hoặc Colab Pro. Về phần mềm, bốn công cụ chính: Python 3.10 trở lên, Docker, Git, một trong các cloud (AWS, GCP, Azure, có free tier). Về tài khoản, một API key của một LLM provider (OpenAI, Anthropic, hoặc dùng LLM cục bộ với Ollama miễn phí), một tài khoản [Hugging Face](https://huggingface.co), một tài khoản [Kaggle](https://www.kaggle.com), một tài khoản [arxiv-vanity.com](https://www.arxiv-vanity.com) hoặc [ar5iv.labs.arxiv.org](https://ar5iv.labs.arxiv.org) để đọc paper dễ hơn. Về thời gian, 12 đến 20 giờ mỗi tuần cho 1 chặng ở chặng 141 đến 160, linh hoạt 1 đến 4 tuần mỗi chặng ở chặng 161 đến 170. Về lưu trữ, thư mục `portfolio-ai/phan-4/` và `portfolio-ai/final-portfolio/`.

## Ghi chú triển khai

Phần 4 chuyển trọng tâm từ "huấn luyện mô hình" sang "đưa mô hình ra production" (chặng 141 đến 160) rồi sang "nghiên cứu và định hướng" (chặng 161 đến 170). Đây là phần tạo nên khác biệt giữa một "người biết làm ML" và một "kỹ sư AI thực thụ" hoặc "nghiên cứu viên tương lai".

Đừng dừng ở notebook. Hoàn tất chặng 158 có nghĩa là bạn có một URL công khai cho ứng dụng AI của mình, đó là lúc portfolio của bạn thực sự "lên cấp". Đừng bỏ qua chặng 170 (portfolio tổng), vì đó là lúc bạn định hình bạn sẽ dùng AI để làm gì trong 5 đến 10 năm tiếp theo. Phần giá trị nhất của toàn lộ trình không phải kiến thức, mà là sự tự nhận thức.

## Liệt kê chặng đã phát hành

Phần 4 đang hoàn thiện. Khung nội dung chi tiết từng chặng có sẵn trong [ROADMAP.md](../ROADMAP.md). Học liệu đầy đủ sẽ phát hành theo thứ tự sau Phần 3.
