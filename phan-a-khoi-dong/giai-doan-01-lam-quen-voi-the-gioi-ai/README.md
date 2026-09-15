# Chặng 01 — Làm quen với thế giới AI xung quanh ta

Đây là chặng đầu tiên của lộ trình 170 chặng. Bạn sẽ học AI là gì, gồm những loại nào, các lĩnh vực con của AI, các ví dụ AI trong đời sống xung quanh bạn, và giới hạn hiện tại của công nghệ này. Sau chặng này, bạn sẽ không còn nhầm AI với "chatbot" hay "phần mềm tự động" — bạn sẽ có một khung khái niệm chính xác để tiếp thu 169 chặng tiếp theo.

---

## Phần A — Kiến thức

### A.1. Trí tuệ nhân tạo (AI) là gì

**Trí tuệ nhân tạo** (*Artificial Intelligence*, viết tắt **AI**) là ngành khoa học máy tính nghiên cứu việc xây dựng các hệ thống máy tính có thể thực hiện những việc từng cần trí tuệ người — như nhận dạng hình ảnh, hiểu ngôn ngữ nói, chơi cờ, dịch văn bản, hay đưa ra quyết định trong điều kiện không chắc chắn.

Định nghĩa chuẩn của Russell & Norvig trong giáo trình *Artificial Intelligence: A Modern Approach* (2020, 4th edition) là:

> "AI là nghiên cứu các *agent* (tác tử) nhận thông tin từ môi trường qua cảm biến và hành động qua cơ cấu tác động, sao cho hành động đó giúp đạt mục tiêu."

Định nghĩa này có hai ý quan trọng:
1. AI là một **agent** — nó nhận input và tạo ra output có mục đích, không ngẫu nhiên.
2. AI **tương tác với môi trường** — nó không tồn tại trong chân không, mà hành động dựa trên thông tin nhận được và ảnh hưởng trở lại môi trường.

Một cách định nghĩa khác, phổ biến trong công nghiệp: **AI là tập hợp các kỹ thuật cho phép máy tính học từ dữ liệu để thực hiện việc cần trí tuệ người**. Khác với phần mềm truyền thống (người viết quy tắc rõ ràng), phần mềm AI tự rút ra quy tắc từ dữ liệu.

### A.2. Ba cấp độ AI theo năng lực

Khi đọc báo chí, bạn sẽ thấy nhiều phân loại AI. Phân loại chuẩn nhất theo năng lực:

| Cấp độ | Tên | Đặc điểm | Tình trạng hiện tại (2025) |
|--------|-----|----------|----------------------------|
| 1 | **AI hẹp** (*Narrow AI / Weak AI*) | Xử lý một việc cụ thể: nhận dạng ảnh, dịch văn bản, chơi cờ vua | Tồn tại và phổ biến. Mọi AI bạn dùng hằng ngày đều hẹp. |
| 2 | **AI tổng quát** (*General AI / Strong AI / AGI*) | Học được mọi việc trí tuệ người có thể học, chuyển kiến thức giữa lĩnh vực | Chưa tồn tại. Là mục tiêu nghiên cứu dài hạn. |
| 3 | **Siêu trí tuệ** (*Superintelligence*) | Vượt người trên mọi lĩnh vực trí tuệ | Hoàn toàn giả thuyết. |

Lưu ý quan trọng: **không có AI tổng quát hay siêu trí tuệ tồn tại ở thời điểm hiện tại**, dù một số công ty (OpenAI, DeepMind, Anthropic) tuyên bố hướng tới AGI. Mọi "AI" bạn gặp — ChatGPT, Midjourney, Gemini, hệ thống tự lái Tesla — đều là AI hẹp, chỉ xử lý một (hoặc một vài) việc cụ thể rất giỏi.

### A.3. Bốn lĩnh vực con chính của AI

AI không phải khối thống nhất — nó là một ngành gồm nhiều lĩnh vực con. Bốn lĩnh vực phổ biến nhất, và là trọng tâm lộ trình này:

#### A.3.1. Học máy (*Machine Learning*, ML)

ML là nhánh AI trong đó máy **tự học quy tắc từ dữ liệu** thay vì được người lập trình từng quy tắc. Ví dụ: để máy nhận dạng mèo, không ai viết quy tắc "có tai nhọn + có ria + 4 chân = mèo" — người ta cho máy xem 10.000 ảnh mèo và 10.000 ảnh không phải mèo, máy tự tìm quy luật phân biệt.

ML lại chia thành:
- **Học có giám sát** (*supervised learning*): dữ liệu có nhãn (ảnh mèo có nhãn "mèo", ảnh chó có nhãn "chó"). Máy học ánh xạ input → nhãn.
- **Học không giám sát** (*unsupervised learning*): dữ liệu không nhãn. Máy tìm cấu trúc ẩn (phân cụm khách hàng, giảm chiều dữ liệu).
- **Học tăng cường** (*reinforcement learning*): máy học qua thử-sai với thưởng/phạt (chơi cờ, đi xe, robot).

ML được học chuyên sâu ở Phần E (chặng 101–120).

#### A.3.2. Học sâu (*Deep Learning*, DL)

DL là nhánh con của ML dùng **mạng nơ-ron nhân tạo nhiều lớp** (*deep neural networks*). "Sâu" ở đây không phải trí tuệ sâu — mà là mạng có nhiều lớp (lớp ẩn). DL đặc biệt mạnh với dữ liệu phi cấu trúc: ảnh, âm thanh, văn bản. ChatGPT, Midjourney, hệ thống tự lái — đều dùng DL.

DL được học chuyên sâu ở Phần F (chặng 121–140).

#### A.3.3. Thị giác máy tính (*Computer Vision*, CV)

CV là nhánh AI xử lý dữ liệu hình ảnh/video: nhận dạng đối tượng, phân đoạn ảnh, phát hiện khuôn mặt, mô tả ảnh bằng văn bản. CV kết hợp kỹ thuật DL (đặc biệt CNN) với xử lý ảnh số học.

CV được giới thiệu sơ lược ở chặng 19, 66; chuyên sâu ở chặng 127–132, 160.

#### A.3.4. Xử lý ngôn ngữ tự nhiên (*Natural Language Processing*, NLP)

NLP là nhánh AI xử lý ngôn ngữ người (văn bản, lời nói): dịch máy, tóm tắt, phân loại cảm xúc, chatbot, hỏi-đáp. NLP kết hợp kỹ thuật DL (đặc biệt Transformer) với ngôn ngữ học.

NLP được giới thiệu sơ lược ở chặng 20, 67; chuyên sâu ở chặng 133–140, 161.

Ngoài bốn lĩnh vực trên, AI còn có các nhánh khác: **robot học** (*robotics*), **hệ chuyên gia** (*expert systems*), **lập luận tự động** (*automated reasoning*), **tìm kiếm và tối ưu** (*search and optimization*). Các nhánh này ít phổ biến hơn trong ứng dụng thương mại hiện nay, nhưng quan trọng về mặt lịch sử và lý thuyết.

### A.4. AI quanh bạn — sáu dấu chân trong đời sống

Để hiểu AI không phải thứ viễn tưởng, hãy xem sáu hệ thống AI bạn có thể đã dùng hôm nay:

1. **Trợ lý ảo** (*virtual assistant*): Google Assistant, Siri, Alexa. Bạn nói "Bây giờ mấy giờ?" — máy nghe giọng bạn (NLP), chuyển thành chữ, hiểu ý định, tra dữ liệu, nói lại câu trả lời (TTS). Đây là pipeline NLP end-to-end.

2. **Gợi ý video** (*recommendation system*): YouTube, TikTok, Netflix. Khi bạn xem xong một video, hệ thống dùng lịch sử xem của bạn và hàng triệu người dùng tương tự để dự đoán video tiếp theo bạn có thể thích. Đây là ML học có giám sát + học không giám sát.

3. **Dịch máy** (*machine translation*): Google Dịch, DeepL. Bạn gõ câu tiếng Việt, hệ thống mã hóa câu thành vector số, dịch chuyển ngữ nghĩa qua không gian vector, rồi giải mã ra tiếng Anh. Đây là DL với kiến trúc Transformer (chặng 137).

4. **Mở khóa bằng khuôn mặt** (*face unlock*): điện thoại nhìn mặt bạn, so với khuôn mặt đã đăng ký. Hệ thống dùng CV (đặc biệt CNN) để trích đặc trưng khuôn mặt thành vector, so khoảng cách vector mới với vector đã lưu. Đây là DL + CV.

5. **Camera tự tìm mặt** (*face detection*): khung vàng quanh mặt khi chụp ảnh. Hệ thống quét ảnh theo cửa sổ trượt, mỗi cửa sổ đưa qua mạng CNN đã huấn luyện nhận "đây có phải mặt người không". Đây là CV + DL.

6. **Chatbot** (*chatbot*): ChatGPT, Claude, Gemini. Bạn hỏi bằng văn bản, hệ thống dự đoán token tiếp theo có xác suất cao nhất dựa trên văn bản đã có, lặp lại nhiều lần để tạo câu trả lời. Đây là DL + NLP với mô hình ngôn ngữ lớn (LLM).

Điểm chung của sáu hệ thống: **mỗi cái đều "học" từ lượng dữ liệu khổng lồ** trước khi hoạt động. Không có hệ thống nào được lập trình bằng tay từng quy tắc. Đây là đặc trưng của AI hiện đại.

### A.5. AI giỏi việc gì, chưa giỏi việc gì

Hiểu giới hạn AI quan trọng không kém hiểu năng lực của nó. Bảng sau tổng kết:

| Việc | AI hiện nay giỏi? | Lý do |
|------|-------------------|-------|
| Tính toán số học trên lượng lớn | Rất giỏi | Máy tính vốn sinh ra để tính |
| Tìm mẫu hình trong dữ liệu lớn | Rất giỏi | ML thiết kế cho việc này |
| Nhận dạng ảnh/âm thanh ở quy mô lớn | Rất giỏi | DL với CNN/Transformer đã vượt người |
| Dịch văn bản giữa ngôn ngữ phổ biến | Khá giỏi | Nhưng vẫn sai ở ngữ cảnh tinh tế |
| Hiểu cảm xúc người khác | Kém | Cần lý thuyết tâm trí, AI chưa có |
| Đưa ra quyết định đạo đức | Kém | Không có "hàm đạo đức" để tối ưu |
| Sáng tạo kiến thức mới | Kém | AI tổng hợp từ dữ liệu đã có, không kiến tạo |
| Học một việc mới từ 1–2 ví dụ | Rất kém | AI cần hàng nghìn/triệu ví dụ |
| Chuyển kiến thức giữa lĩnh vực khác nhau | Rất kém | Đây là ranh giới với AGI |

Nguyên lý sâu xa: AI hiện nay giỏi việc **lặp lại quy luật đã có trong dữ liệu**, kém việc **hiểu ngữ cảnh và chuyển ý nghĩa**. Khi đọc tin "AI sắp thay thế X", hãy hỏi: "X có phải việc lặp quy luật dữ liệu, hay việc hiểu ngữ cảnh?". Câu trả lời cho biết mức độ đáng tin của tin.

### A.6. Học máy khác lập trình truyền thống ở đâu

Để thực sự hiểu AI, phải hiểu sự khác biệt với lập trình truyền thống:

**Lập trình truyền thống**: người lập trình viết **quy tắc** rõ ràng. Ví dụ phần mềm tính thuế: `if (thu_nhap > 11e6) then thue = ... ` — mỗi trường hợp một dòng code. Ưu điểm: rõ ràng, kiểm chứng được. Nhược điểm: không khả thi với việc phức tạp (nhận dạng mèo cần bao nhiêu quy tắc?).

**Học máy**: người lập trình không viết quy tắc. Họ viết **thuật toán học**, cung cấp **dữ liệu** (input + nhãn), thuật toán tự tìm ra quy tắc. Ưu điểm: mở rộng được cho việc phức tạp. Nhược điểm: quy tắc tìm được không dễ giải thích ("tại sao máy đoán đây là mèo?").

Bảng so sánh:

| Khía cạnh | Lập trình truyền thống | Học máy |
|-----------|------------------------|---------|
| Người viết quy tắc | Lập trình viên | Thuật toán (tự rút từ dữ liệu) |
| Dữ liệu | Input cho chương trình | Vừa input vừa "giáo viên" của thuật toán |
| Khi quy luật phức tạp | Code rất dài, khó bảo trì | Thuật toán vẫn ngắn, chỉ cần thêm dữ liệu |
| Khi cần giải thích | Code chính là giải thích | Cần kỹ thuật riêng (SHAP, LIME — chặng 143) |
| Phù hợp khi | Quy luật rõ, cố định | Quy luật ẩn trong dữ liệu, khó viết tay |

Lộ trình này bắt đầu bằng lập trình truyền thống (Phần B) trước khi sang ML (Phần E) — vì hiểu lập trình là nền cho hiểu ML.

### A.7. Một câu thần chú để nhớ

Sau khi đọc phần Kiến thức, hãy nhẩm một câu tóm tắt:

> **AI là ngành xây dựng agent thông minh. Cách tiếp cận phổ biến nhất là cho máy học quy tắc từ rất nhiều dữ liệu (thay vì viết tay quy tắc). AI hiện nay đều là AI hẹp — giỏi việc lặp quy luật dữ liệu, kém việc hiểu ngữ cảnh.**

Nếu bạn có thể viết lại câu này bằng lời của mình mà không xem tài liệu — bạn đã hiểu phần Kiến thức. Nếu không, hãy đọc lại A.1–A.6 trước khi sang phần Thực hành.

---

## Phần B — Thực hành

Để biến kiến thức thành trực giác, bạn cần tự tay quan sát và phản xạ. Bài tập sau xếp từ dễ đến khó. Bài sao ★ là bắt buộc; bài không sao là tùy chọn mở rộng.

### Bài 1 ★: Săn tìm 6 dấu chân AI trong đời sống bạn

Mở một tệp markdown `portfolio-ai/phan-a/chặng-01-nhat-ky-ai/observations.md`. Trong 3 ngày tiếp theo, mỗi ngày quan sát ít nhất 2 hệ thống AI bạn dùng. Mỗi lần quan sát, ghi:

| Hệ thống | Input của nó | Output của nó | Dữ liệu nó đã học từ đâu | Lĩnh vực AI (ML/DL/CV/NLP) |
|----------|--------------|---------------|--------------------------|----------------------------|
| Gợi ý video YouTube | Lịch sử xem của tôi | Danh sách video gợi ý | Lịch sử xem hàng tỷ người | ML (học có giám sát) |
| ... | ... | ... | ... | ... |

Cố gắng thu được ít nhất 6 hệ thống. Đừng dán ví dụ của tài liệu — hãy quan sát đời sống bạn.

### Bài 2 ★: Phân biệt AI vs không-AI

Đánh dấu X vào cột phù hợp cho mỗi tình huống dưới đây. Cố gắng suy nghĩ trước khi xem đáp án ở cuối tệp.

| Tình huống | Có dùng AI | Không dùng AI |
|------------|------------|----------------|
| 1. Máy tính thường cộng 25 + 75 | | |
| 2. Điện thoại gợi ý từ tiếp theo khi bạn nhắn tin | | |
| 3. Quạt quay theo nút bấm cấp 1, 2, 3 | | |
| 4. Ứng dụng bản đồ vẽ lộ trình tránh đường kẹt | | |
| 5. Đồng hồ báo thức reo đúng 6 giờ sáng mỗi ngày | | |
| 6. Ứng dụng học tiếng Anh chấm giọng đọc của bạn | | |
| 7. Máy lạnh tự tăng giảm theo nhiệt độ phòng và thói quen nhà | | |
| 8. Cái kéo cắt giấy | | |
| 9. ChatGPT trả lời câu hỏi của bạn | | |
| 10. Email được tự động phân vào "Spam" | | |

Sau khi đánh dấu, viết 1 đoạn 100 chữ giải thích: **Điểm khác cốt lõi giữa hệ thống có AI và không AI là gì?** (Gợi ý: AI phải "học" từ dữ liệu; không AI thì làm theo quy tắc cố định.)

### Bài 3 (tùy chọn): Phân tích 1 hệ thống AI sâu hơn

Chọn 1 hệ thống AI bạn dùng nhiều (vd: ChatGPT, gợi ý YouTube, Google Dịch). Viết 1 bài 300–500 chữ trả lời:

1. Input chính của hệ thống là gì?
2. Output chính là gì?
3. Bạn đoán hệ thống đã học từ đâu? (kiểu dữ liệu, nguồn, lượng dữ liệu ước lượng)
4. Một việc hệ thống làm tốt — vì sao?
5. Một việc hệ thống làm kém — vì sao?
6. Nếu bạn là kỹ sư của hệ thống, bạn sẽ thu thập thêm dữ liệu gì để cải thiện?

Bài này không có đáp án "đúng". Mục đích là tập tư duy ngược: từ trải nghiệm người dùng → đoán thiết kế bên trong.

### Bài 4 (tùy chọn): Trò chơi "Huấn luyện máy từ thẻ hình"

Trò chơi này giúp bạn trải nghiệm trực giác về học máy — không cần máy tính.

Chuẩn bị 10 tấm thẻ: 6 tấm vẽ đồ vật (quả cam, quả bóng, cuốn sách, cái ly, viên gạch, quả bầu dục), 4 tấm trống để bạn tự điền.

Cách chơi:
1. Đóng vai "máy" — chỉ nhận biết bằng 2 tính chất bạn chọn.
2. Bạn (vai "người dạy") xem 3–4 ví dụ quả tròn (cam, bóng...) và tự phát hiện quy tắc: "tròn là quả tròn".
3. Đưa thẻ "viên gạch" — bạn (vai máy) hỏi "Đây là quả tròn không?" và trả lời kèm lý do dựa trên quy tắc đã học.
4. Thử "dữ liệu xấu": nếu ban đầu chỉ cho máy xem quả cam và quả bóng to — máy sẽ nói "to và tròn mới là quả tròn" rồi chối quả bầu dục nhỏ. Đây là hiện tượng **overfitting** — máy học quá khít vào ví dụ cụ thể, không khái quát được.

Sau khi chơi, viết 2–3 dòng vào `observations.md`: bạn rút ra được gì về mối quan hệ giữa dữ liệu huấn luyện và hành vi của "máy"? Đây là nền tảng trực giác cho chặng 105 (Overfitting & Underfitting) sau này.

### Bài 5 (tùy chọn): Báo cáo "Ví dụ xấu"

Nghĩ 1 tình huống: nếu huấn luyện máy nhận biết "cán bộ" chỉ bằng ảnh những người đeo kính, máy sẽ kết luận gì về người không đeo kính? Viết 2 câu:

1. Máy học sai khi: __________________________________
2. Để máy học đúng hơn, ta cần cho nó xem: __________________________________

Đây là lần đầu bạn chạm vào ý tưởng quan trọng: **dữ liệu không tốt làm máy đối xử không công bằng**. Lộ trình sẽ quay lại ý tưởng này ở chặng 69 (thiên vị dữ liệu) — khi bạn đã có đủ công cụ để phân tích sâu.

---

## Phần C — Sản phẩm cuối chặng

### "Nhật ký AI" — 5 trang ghi lại hệ thống AI trong đời sống bạn

**Yêu cầu:** tạo một tệp markdown `portfolio-ai/phan-a/chặng-01-nhat-ky-ai/README.md` gồm 5 phần:

| Phần | Nội dung | Điều kiện đạt |
|------|----------|---------------|
| 1. Định nghĩa AI | 1–2 câu định nghĩa bằng lời bạn, không chép tài liệu | Có nhắc "học từ dữ liệu" và "làm việc cần trí tuệ người" |
| 2. Bảng phân loại AI | 3 cấp độ (hẹp/tổng quát/siêu trí tuệ) + tình trạng hiện tại | Đúng theo bảng A.2 |
| 3. Bảng 4 lĩnh vực con | ML, DL, CV, NLP — 1 dòng mô tả mỗi lĩnh vực | Đúng định nghĩa |
| 4. 6 dấu chân AI | Bảng 6 hệ thống AI bạn quan sát được trong 3 ngày (theo mẫu Bài 1) | Đủ 6 ví dụ với 5 cột điền đủ |
| 5. Câu hỏi mở | 1 câu hỏi về AI bạn muốn tìm hiểu tiếp (vd: "Làm sao máy học được ngữ cảnh?") | Câu hỏi cụ thể, có thể trả lời dần qua lộ trình |

Lưu tệp vào portfolio. Đây là artifact đầu tiên trong hành trình 170 chặng.

---

## Phần D — Tự đánh giá

Checklist cuối chặng. Đánh dấu X vào mỗi ô khi đạt.

```
□ Tôi đã đọc toàn bộ phần Kiến thức (A.1–A.7)
□ Tôi có thể giải thích AI bằng lời của mình (Feynman test)
□ Tôi có thể phân biệt AI hẹp, tổng quát, siêu trí tuệ
□ Tôi có thể liệt kê 4 lĩnh vực con của AI kèm ví dụ
□ Tôi đã làm xong Bài 1 và Bài 2 (sao ★)
□ Tôi đã hoàn thành "Nhật ký AI" và lưu vào portfolio
□ Tôi đã ghi 1 mục vào learning-journal.md cho chặng này
□ Tôi đã trả lời được câu hỏi "Kết nối về sau" trong tu-dien-va-tai-nguyen.md
```

Nếu 8/8 ô được đánh dấu — chúc mừng, bạn đã hoàn thành chặng 01. Sang [Chặn 02](../giai-doan-02-tu-duy-giai-quyet-van-de/README.md).

Nếu có ô chưa đánh dấu — đừng sang chặng sau. Trở lại phần tương ứng.

---

## Phần E — Đáp án Bài 2

| Tình huống | Có AI | Không AI | Lý do |
|------------|-------|----------|-------|
| 1. Máy tính cộng 25 + 75 | | X | Tính toán cố định, không học |
| 2. Gợi ý từ nhắn tin | X | | Học từ lịch sử nhắn của hàng triệu người |
| 3. Quạt quay theo nút | | X | Quy tắc cơ học |
| 4. Bản đồ tránh kẹt | X | | Học từ dữ liệu giao thông thời gian thực |
| 5. Đồng hồ báo thức | | X | Quy tắc cố định |
| 6. Chấm giọng đọc tiếng Anh | X | | Học từ hàng triệu mẫu giọng |
| 7. Máy lạnh theo thói quen | X | | Học từ dữ liệu sử dụng |
| 8. Kéo cắt giấy | | X | Vật lý, không phải máy tính |
| 9. ChatGPT | X | | LLM dự đoán token từ dữ liệu huấn luyện |
| 10. Email vào Spam | X | | Học từ hàng triệu email đã được đánh dấu |

Điểm cốt lõi: **hệ thống có AI học từ dữ liệu để đưa ra quyết định; hệ thống không AI làm theo quy tắc cố định do người viết**.
