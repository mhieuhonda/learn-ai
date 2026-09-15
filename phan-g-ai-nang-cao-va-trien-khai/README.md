# Phần G — AI nâng cao & Triển khai (Chặn 141–158)

**Trạng thái: đang hoàn thiện** — khung nội dung chi tiết từng chặng có sẵn trong [ROADMAP.md](../ROADMAP.md); học liệu đầy đủ sẽ phát hành theo thứ tự sau Phần F.

## Mục tiêu phần

Từ "mô hình chạy trong notebook" đến "ứng dụng AI chạy thật cho người dùng": kỹ thuật ML nâng cao (dữ liệu lệch, giải thích mô hình, giám sát drift), ứng dụng LLM hiện đại (prompt engineering chuyên sâu, API, embeddings, RAG, Agent), và kỹ nghệ triển khai (Docker, FastAPI, CI/CD, MLflow, cloud). Kết thúc phần, bạn ra mắt một ứng dụng AI hoàn chỉnh với giám sát và checklist an toàn.

## Tiên quyết

- Đã hoàn thành Phần F.
- Nếu bạn đã có kinh nghiệm triển khai ML, hãy làm bài tập cuối chặng 149 (RAG) và 158 (end-to-end) để tự kiểm tra.

## Kết quả đầu ra chính

1. Pipeline sklearn chuyên nghiệp xử lý dữ liệu lệch, có báo cáo giải thích SHAP/LIME (chặng 141–143).
2. Thư viện prompt cá nhân + ứng dụng gọi LLM API quản lý token/chi phí (chặng 146–147).
3. Bộ tìm kiếm ngữ nghĩa + chatbot RAG + agent mini (chặng 148–150).
4. Trợ lý học tập tiếng Việt hoàn chỉnh (chặng 151).
5. Ứng dụng end-to-end: mô hình → API → giao diện → giám sát (chặng 158) — cột mốc **"Kỹ sư AI"**.

## Cấu trúc 18 chặng

| Nhóm | Chặn | Chủ đề |
|------|------|--------|
| ML nâng cao | 141–145 | Feature engineering, dữ liệu lệch, giải thích, giám sát, AutoML |
| LLM & ứng dụng | 146–151 | Prompt, API, vector DB, RAG, Agent, trợ lý học tập |
| MLOps & cloud | 152–158 | Docker, FastAPI, CI/CD, MLflow, cloud/GPU, bảo mật, dự án end-to-end |

## Chuẩn bị trước khi bắt đầu

- Python 3.10+, Docker, git.
- **API key** của một LLM provider (OpenAI, Anthropic, hoặc dùng LLM cục bộ với Ollama).
- **Cloud account** (AWS/GCP/Azure) — có free tier; hoặc dùng Colab Pro.
- Khoảng 12–20 giờ mỗi tuần cho 1 chặng.
- Thư mục `portfolio-ai/phan-g/` để lưu ứng dụng.

## Ghi chú triển khai

Phần G chuyển trọng tâm từ "huấn luyện mô hình" sang "đưa mô hình ra production". Đây là kỹ năng mà nhiều người tự học bỏ qua — nhưng lại là kỹ năng được nhà tuyển dụng ai cũng cần. Đừng dừng ở notebook. Hoàn tất chặng 158 có nghĩa là bạn có một URL công khai cho ứng dụng AI của mình — đó là lúc portfolio của bạn thực sự "lên cấp".
