# Phần G — AI nâng cao & Triển khai (Giai đoạn 141–158)

**Trạng thái: đang hoàn thiện** — khung nội dung chi tiết từng giai đoạn có sẵn trong [ROADMAP.md](../ROADMAP.md); học liệu đầy đủ sẽ phát hành theo thứ tự sau Phần F.

## Mục tiêu phần

Từ "mô hình chạy trong notebook" đến "ứng dụng AI chạy thật cho người dùng": kỹ thuật ML nâng cao (dữ liệu lệch, giải thích mô hình, giám sát drift), ứng dụng LLM hiện đại (prompt engineering chuyên sâu, API, embeddings, RAG, Agent), và kỹ nghệ triển khai (Docker, FastAPI, CI/CD, MLflow, cloud). Kết thúc phần, người học ra mắt một ứng dụng AI hoàn chỉnh với giám sát và checklist an toàn.

## Đối tượng & tiên quyết

- Đối tượng: học sinh THPT cuối, sinh viên năm 1–2.
- Tiên quyết: Phần F.

## Kết quả đầu ra chính

1. Pipeline sklearn chuyên nghiệp xử lý dữ liệu lệch, có báo cáo giải thích SHAP/LIME (GĐ 141–143).
2. Thư viện prompt cá nhân + ứng dụng gọi LLM API quản lý token/chi phí (GĐ 146–147).
3. Bộ tìm kiếm ngữ nghĩa + chatbot RAG + agent mini (GĐ 148–150).
4. Trợ lý học tập tiếng Việt hoàn chỉnh (GĐ 151).
5. Ứng dụng end-to-end: mô hình → API → giao diện → giám sát (GĐ 158) — cột mốc **"Kỹ sư AI"**.

## Cấu trúc 18 giai đoạn

| Nhóm | GĐ | Chủ đề |
|------|----|--------|
| ML nâng cao | 141–145 | Feature engineering, dữ liệu lệch, giải thích, giám sát, AutoML |
| LLM & ứng dụng | 146–151 | Prompt, API, vector DB, RAG, Agent, trợ lý học tập |
| MLOps & cloud | 152–158 | Docker, FastAPI, CI/CD, MLflow, cloud/GPU, bảo mật, dự án end-to-end |

## Ghi chú triển khai

- An toàn bắt buộc: GĐ 157 dạy prompt injection và lạm dụng trước khi bất kỳ ứng dụng nào ra mắt công khai; ứng dụng phải có bộ lọc và giới hạn đầu vào.
- Chi phí: mọi bài học API đều có phiên bản "miễn phí/budget" (mô hình nhỏ, giới hạn token); người học dưới 18 tuổi dùng tài khoản do phụ huynh quản lý.
- Đạo đức nghề: sản phẩm cuối phải có "tờ khai trung thực" — mô tả giới hạn, dữ liệu huấn luyện, rủi ro còn lại.
