# Chặng 03 — Dữ liệu và thông tin xung quanh ta

Chặng 01 bạn học AI học từ dữ liệu. Chặng 02 bạn học cách tư duy thuật toán để ra lệnh cho máy. Chặng này bạn học **chất liệu của AI**, đó là dữ liệu. Bạn sẽ học dữ liệu là gì, các loại dữ liệu phổ biến, cách thu thập đúng, cách sắp xếp vào bảng, và trực quan hóa bằng biểu đồ cột. Đây là nền tảng cho mọi kỹ năng dữ liệu sau này: bảng tính (chặng 53 đến 56), Pandas (chặng 80 đến 87), SQL (chặng 58 đến 60), thống kê (chặng 93 đến 98). Sau chặng này, bạn có thể thu thập dữ liệu một cách có kỷ luật, trình bày dữ liệu vào bảng chuẩn, và rút ra nhận xét đúng từ dữ liệu, không bịa, không phóng đại.

Cách đọc chặng này giống hai chặng trước: đi từ đầu đến cuối, không nhảy. Khi gặp khái niệm mới, định nghĩa sẽ ở ngay tại chỗ, kèm ví dụ cụ thể trước khi đi vào lý thuyết.

## 1. Kiến thức

### Dữ liệu là gì và tại sao nó là chất liệu của AI

Hãy bắt đầu từ câu hỏi tưởng dễ: bạn biết cân nặng của mình là 62kg. Đó là thông tin. Nhưng với máy tính, câu đó chưa thành dữ liệu cho đến khi được ghi lại. Nếu cân nặng nằm "trong đầu" bạn, máy không tiếp cận được, nên theo nghĩa máy tính, đó không phải dữ liệu. Nếu cân nặng ghi trên giấy khám bệnh, máy có thể scan và đánh số được, lúc đó là dữ liệu. Nếu cân nặng lưu trong tệp Excel, máy xử lý trực tiếp, đó là dữ liệu theo nghĩa đầy đủ. Vậy **dữ liệu** (*data*) là thông tin được ghi lại dưới dạng có thể lưu trữ, truyền tải, và xử lý.

Bốn dạng dữ liệu phổ biến bạn gặp hằng ngày. **Dữ liệu số** như cân nặng 62kg, chiều cao 1.65m, nhiệt độ 28°C. **Dữ liệu chữ** như tên "Nguyễn Văn A", địa chỉ "12 Lê Lợi", bài thơ. **Dữ liệu hình** như ảnh chụp, bản vẽ, chữ ký scan. **Dữ liệu âm thanh** như ghi âm giọng nói, bài nhạc, tiếng chim hót. Mỗi dạng đòi hỏi kỹ thuật xử lý khác nhau: số thì tính toán, chữ thì phân tích cú pháp, hình thì mạng nơ-ron tích chập, âm thanh thì phân tích phổ tần số. Bạn sẽ học kỹ thuật xử lý từng dạng ở các Phần sau.

Dữ liệu quan trọng cho AI vì sao? Quay lại chặng 01: AI học từ dữ liệu, không có dữ liệu là không có AI. Mỗi hệ thống AI cần **dữ liệu huấn luyện** (*training dataset*), lượng dữ liệu này thường khổng lồ. FaceID điện thoại cần hơn 100 ảnh khuôn mặt của bạn cộng các biến đổi. Gợi ý YouTube cần lịch sử xem của hàng tỷ người. Google Dịch (cặp Anh-Việt) cần hàng triệu cặp câu song ngữ. ChatGPT được ước lượng huấn luyện trên khoảng 500 tỷ token văn bản, tương đương 4 TB text. Midjourney cần khoảng 5 tỷ cặp ảnh kèm chú thích.

Hệ quả thực tiễn: không có dữ liệu, không có AI, AI không "hiểu" nếu không có dữ liệu học. Dữ liệu sai, AI sai, dữ liệu huấn luyện có thiên vị thì AI có thiên vị (sẽ học sâu ở chặng 69). Dữ liệu ít, AI kém, học từ 10 ví dụ không khái quát được bằng học từ 1 triệu ví dụ. Lộ trình sẽ quay lại dữ liệu ở mọi Phần: Phần 2 (chặng 53 đến 60) làm sạch và SQL, Phần 2 (chặng 77 đến 100) Pandas và thống kê, Phần 3 (chặng 99 và 101) feature engineering, Phần 4 (chặng 141 đến 144) dữ liệu drift và giám sát. Nền bạn đúc ngay từ chặng 03 này: số liệu trung thực, trình bày ngay ngắn, nhận xét cẩn trọng.

### Phân loại dữ liệu theo hai chiều quan trọng

Dữ liệu phân loại theo nhiều chiều, hai chiều quan trọng nhất thường gặp. Chiều thứ nhất là định lượng so với định tính. **Dữ liệu định lượng** (*quantitative data*) đo lường được bằng số, ví dụ cân nặng, nhiệt độ, giá tiền. **Dữ liệu định tính** (*qualitative data*) mô tả đặc tính, không đo lường trực tiếp, ví dụ màu sắc, giới tính, đánh giá "tốt" hay "trung bình". Dữ liệu định lượng lại chia: **liên tục** (*continuous*) có thể lấy mọi giá trị trong khoảng (cân nặng 62.3kg, 62.35kg, 62.357kg, càng đo càng chi tiết), **rời rạc** (*discrete*) chỉ lấy giá trị đếm được (số con người là 0, 1, 2, 3, không có 2.5 con người).

Chiều thứ hai là cấu trúc. **Dữ liệu có cấu trúc** (*structured data*) sắp xếp theo hàng và cột, có lược đồ rõ, ví dụ bảng Excel, bảng SQL, file CSV. **Dữ liệu bán cấu trúc** (*semi-structured data*) có thẻ hoặc nhãn nhưng không theo bảng, ví dụ JSON, XML, HTML. **Dữ liệu phi cấu trúc** (*unstructured data*) không có cấu trúc cố định, ví dụ văn bản tự do, ảnh, âm thanh, video. Ước tính 80% dữ liệu thế giới hiện là phi cấu trúc (ảnh, video, văn bản). ML và DL hiện đại mạnh vì xử lý được dữ liệu phi cấu trúc, điều mà công cụ truyền thống không làm được. Bạn sẽ học sâu ở Phần 3.

### Thu thập dữ liệu đúng: ba quy tắc và cạm bẫy bias lấy mẫu

Thu thập dữ liệu đúng là 80% chất lượng phân tích. Sai ở khâu này, mọi phân tích sau sai theo. Ba quy tắc. **Đúng** là ghi đúng ý hoặc số người nói, không sửa theo ý mình, ví dụ người khảo sát nói "trà" thì không ghi thành "trà đào". **Đủ** là hỏi đủ số người đã định, không bỏ dở, ví dụ định khảo sát 10 người thì không dừng ở 7 vì lười. **Trung thực** là ghi đúng kết quả quan sát, không bịa, ví dụ người khảo sát trả lời "không biết" thì ghi "không biết", không tự điền đại.

Lưu ý về quyền riêng tư: khi thu thập dữ liệu từ người khác, chỉ hỏi những thông tin thực sự cần cho bài toán. Không hỏi số điện thoại, CCCD, địa chỉ nhà trừ khi có lý do rõ ràng và được đồng ý. Đây là nền tảng đạo đức dữ liệu, sẽ học sâu ở chặng 70.

Khi thu thập dữ liệu, bạn thường không thể hỏi tất cả dân số, mà chỉ hỏi một **mẫu** (*sample*). Mẫu phải **đại diện** cho dân số, nếu không kết luận bị sai. **Bias lấy mẫu** (*sampling bias*) xảy ra khi mẫu không đại diện. Ví dụ: muốn biết "người Việt thích thể thao gì", chỉ hỏi bạn cùng lớp thì bị bias, vì mẫu chỉ là thanh niên cùng độ tuổi, không đại diện cho người già, trẻ em, người nông thôn. Hoặc muốn biết "ai sẽ thắng cử", chỉ gọi điện cho người có điện thoại cố định thì bị bias, vì người giàu có điện thoại cố định nhiều hơn người nghèo.

Cách tránh bias cơ bản: xác định dân số mục tiêu rõ ("người Việt 18+ toàn quốc"), chọn mẫu sao cho mọi nhóm trong dân số đều có cơ hội được hỏi, cỡ mẫu đủ lớn (thường ít nhất 30 cho thống kê cơ bản, ít nhất 400 cho khảo sát dân số lớn). Sẽ học sâu về lấy mẫu ở chặng 95.

### Trình bày dữ liệu: bảng và biểu đồ cột

**Bảng** (*table*) là cách phổ biến nhất để sắp xếp dữ liệu có cấu trúc. Bảng gồm các thành phần: tiêu đề bảng đặt trên cùng, mô tả bảng về cái gì. Tên cột (header) mô tả trường dữ liệu mỗi cột. Hàng (row), mỗi hàng là 1 bản ghi (1 đối tượng hoặc 1 sự kiện). Ô (cell) là giao cột và hàng, chứa 1 giá trị. Dòng tổng (tùy chọn) là tổng hoặc trung bình của cột số.

Ví dụ: bảng khảo sát nước uống yêu thích, với 2 cột là "Loại nước" và "Số người chọn". Hàng "Nước lọc" có số 4, hàng "Nước cam" có số 2, hàng "Trà đào" có số 3, hàng "Sữa" có số 2, dòng tổng là 11. Lý do dùng bảng: tra cứu nhanh (hỏi "Trà đào được mấy người chọn", nhìn bảng trả lời tức thì), so sánh (nhìn thấy ngay loại nào nhiều nhất, ít nhất), tổng hợp (tính tổng, trung bình bằng cách nhìn cột).

Bảng tốt cho tra cứu, nhưng **biểu đồ** tốt hơn cho "nhìn một cái là hiểu xu hướng". Loại biểu đồ phổ biến nhất cho dữ liệu phân loại là **biểu đồ cột** (*bar chart*). Cách vẽ: vẽ trục ngang (x-axis), mỗi loại dữ liệu là 1 cột, cách đều nhau. Vẽ trục dọc (y-axis) với thang số, từ 0 đến giá trị lớn nhất cộng biên độ. Với mỗi loại, vẽ 1 cột cao bằng giá trị tương ứng. Thêm tiêu đề trên cùng, nhãn trục, chú thích nếu cần.

Khi đọc biểu đồ, có 4 câu hỏi vàng. Cột cao nhất cho biết loại được chọn nhiều nhất. Cột thấp nhất cho biết loại ít nhất. So sánh 2 cột cho biết chênh lệch bao nhiêu. Tổng các cột cho biết tổng số người tham gia, phải khớp với bảng.

### Phân biệt nhận xét từ dữ liệu và ý kiến cá nhân

Đây là kỹ năng quan trọng nhất của người làm dữ liệu, và là kỹ năng nhiều người thiếu. **Nhận xét từ dữ liệu** là câu nói có số liệu làm bằng chứng, rút ra từ bảng hoặc biểu đồ. Ví dụ đúng: "Nước lọc được 4 người chọn, nhiều nhất trong nhóm 11 người khảo sát". Hoặc "Trà đào được chọn nhiều gấp 1.5 lần nước cam (3 so với 2)". Hoặc "Tổng có 11 người tham gia khảo sát, trong đó 4 người (36%) chọn nước lọc".

**Ý kiến cá nhân** là câu nói phản ánh cảm nhận, không có số liệu. Ví dụ sai (vì là ý kiến): "Nước lọc ngon nhất" (không có số liệu, "ngon" là cảm nhận). "Trà đào chắc chắn sẽ thắng" (dự đoán, không phải dữ liệu). "Nhóm này thích đồ uống lành mạnh" (suy diễn, không có số liệu).

Nguyên lý: phân tích dữ liệu chỉ trả lời "cái gì" và "bao nhiêu", không trả lời "tại sao" hoặc "có nên". Phân tích dữ liệu không thay thế phán đoán đạo đức hoặc quyết định giá trị. Khi bạn nghe một câu kết luận về dữ liệu, hãy luôn hỏi: "Câu này có số liệu nào làm bằng chứng không?". Nếu không, đó là ý kiến, không phải nhận xét từ dữ liệu, dù người nói có thể là chuyên gia.

### Một câu thần chú để nhớ

Dữ liệu là thông tin được ghi lại. Thu thập đúng cộng đủ cộng trung thực. Bảng để tra cứu, biểu đồ để thấy xu hướng. Nhận xét phải có số liệu làm bằng chứng, không bịa, không phóng đại. Nếu bạn viết lại được câu này bằng lời của mình mà không xem tài liệu, bạn đã hiểu phần Kiến thức.

## 2. Thực hành

Bài tập cho chặng 03 xếp từ dễ đến khó. Bài có dấu sao (★) là bắt buộc, bài không sao là tùy chọn mở rộng. Tất cả tự làm một mình.

### Bài 1 ★: Săn tìm 4 loại dữ liệu trong 1 ngày

Trong 1 ngày, ghi lại ít nhất 3 ví dụ cho mỗi loại dữ liệu: số (cân nặng, số bước chân, nhiệt độ ngoài trời), chữ (tên bạn, địa chỉ nhà, tên bài hát đang nghe), hình (ảnh chụp bữa trưa, ảnh tự sướng sáng nay, bản vẽ sơ đồ phòng), âm thanh (ghi âm giọng nói của bạn, tiếng chuông điện thoại, bài hát đang nghe). Lưu vào `portfolio-ai/phan-1/chặng-03-bao-cao-du-lieu/data-types.md`. Tiêu chí đạt: mỗi loại có ít nhất 3 ví dụ cụ thể, không chép ví dụ mẫu.

### Bài 2 ★: Khảo sát mini "Nước uống yêu thích"

Thực hiện 1 khảo sát nhỏ để thu thập dữ liệu thực. Câu hỏi khảo sát: "Trong các loại nước sau, nước lọc, nước cam, trà đào, sữa, bạn thích loại nào nhất?". Quy trình bốn bước. Bước 1, lên kế hoạch: chọn 6 đến 10 người để hỏi (bạn bè, người nhà, đồng nghiệp). Bước 2, hỏi lịch sự: chào hỏi, giới thiệu mục đích ("tôi đang học về dữ liệu, xin phép hỏi 1 câu"), cảm ơn sau. Bước 3, ghi tally (ký hiệu đếm) bằng các vạch gạch, ví dụ 4 vạch cho nước lọc, 2 cho nước cam, 3 cho trà đào, 2 cho sữa. Bước 4, kiểm tra chéo: đếm lại tổng ký hiệu có bằng số người đã hỏi không, nếu không thì đếm lại, không tự thêm bớt.

Lưu ý quan trọng: chỉ hỏi sở thích, không hỏi số điện thoại, địa chỉ nhà, CCCD, quyền riêng tư từ đầu. Nếu người hỏi "không biết" hoặc "thích nhiều loại", ghi theo câu trả lời, không ép chọn 1. Tránh bias, đừng chỉ hỏi người cùng độ tuổi, cùng giới tính, cùng nghề nghiệp.

### Bài 3 ★: Lập bảng dữ liệu từ khảo sát

Từ tally của Bài 2, lập bảng chuẩn. Tiêu đề bảng: "Nước uống yêu thích, khảo sát nhóm tôi". Hai cột: Loại nước và Số người chọn. Bốn hàng dữ liệu: Nước lọc, Nước cam, Trà đào, Sữa (điền số tương ứng). Dòng tổng ở cuối. Lưu vào `data-types.md`. Kiểm tra: tổng cột phải bằng tổng số người đã hỏi.

### Bài 4 ★: Vẽ biểu đồ cột trên giấy kẻ ô vuông

Từ bảng Bài 3, vẽ biểu đồ cột trên giấy kẻ ô vuông (hoặc dùng công cụ online như [Google Sheets](https://sheets.google.com), Excel, Data Studio). Quy trình vẽ 5 bước. Bước 1, vẽ trục ngang, ghi 4 tên loại nước, cách đều nhau. Bước 2, vẽ trục dọc bên trái, đánh số 0, 1, 2, 3, 4... (mỗi ô là 1 người). Bước 3, với mỗi loại nước, tô cột cao bằng số người chọn. Bước 4, viết tiêu đề trên cùng: "Nước uống yêu thích, khảo sát nhóm tôi". Bước 5, ghi "Số người" cạnh trục dọc, "Loại nước" dưới trục ngang.

Trả lời 4 câu hỏi vàng: loại nước nào được chọn nhiều nhất (cột cao nhất). Loại nào ít nhất. Nước lọc hơn trà đào bao nhiêu người. Tổng cộng có bao nhiêu người tham gia (cộng tất cả cột, phải khớp với bảng). Chụp ảnh biểu đồ (nếu vẽ tay) hoặc export PDF (nếu vẽ tool), lưu vào thư mục portfolio.

### Bài 5 ★: Viết 2 nhận xét từ dữ liệu

Từ bảng và biểu đồ, viết 2 nhận xét. Mỗi nhận xét phải có số liệu làm bằng chứng. Ví dụ nhận xét đúng: "Nước lọc được 4 người chọn, nhiều nhất trong nhóm 11 người khảo sát". Hoặc "Trà đào (3 người) gấp 1.5 lần nước cam (2 người)". Hoặc "Tổng có 11 người tham gia khảo sát, trong đó 4 người (36%) chọn nước lọc".

Ví dụ nhận xét sai (vì là ý kiến cá nhân): "Nước lọc ngon nhất" (cảm nhận, không có số liệu). "Trà đào chắc chắn sẽ thắng" (dự đoán, không phải dữ liệu). "Nhóm này thích đồ uống lành mạnh" (suy diễn, không có số liệu). Lưu 2 nhận xét vào `data-types.md`.

### Bài 6 (tùy chọn): Khảo sát câu hỏi thứ 2

Lặp lại Bài 2 đến 5 với câu hỏi khác, ví dụ "Bạn thường xem video trên nền tảng nào nhất" (YouTube, TikTok, Facebook, Instagram), hoặc "Bạn thường đi làm hoặc đi học bằng phương tiện nào" (xe máy, xe buýt, đi bộ, ô tô), hoặc "Bạn uống mấy ly nước mỗi ngày" (1, 2, 3, 4, 5+). So sánh kết quả 2 khảo sát, có mẫu hình gì thú vị không.

### Bài 7 (tùy chọn): Phát hiện bias lấy mẫu

Trong khảo sát Bài 2, trả lời 4 câu: ai bạn đã hỏi (độ tuổi, giới tính, nghề nghiệp, khu vực). Nhóm này đại diện cho ai (toàn dân Việt Nam, thanh niên Hà Nội, người ở nhà bạn). Nếu kết quả khảo sát được tuyên bố là "người Việt thích loại nước X nhất", có bias không. Để tránh bias, bạn cần thay đổi gì trong cách chọn người khảo sát. Đây là nền tảng cho chặng 95 (lấy mẫu và tổng thể) và chặng 69 (thiên vị dữ liệu).

### Bài 8 (tùy chọn): Đọc 1 biểu đồ báo chí

Tìm 1 bài báo tiếng Việt có biểu đồ (VnExpress, Tuổi Trẻ thường có). Trả lời 5 câu: biểu đồ loại gì (cột, đường, tròn, area). Dữ liệu từ đâu. Trục x và y thể hiện gì. 2 nhận xét chính từ biểu đồ. Có gì đáng nghi không (trục bị cắt, tỷ lệ không trung thực, thiếu nguồn). Đây là nền tảng cho chặng 91 (nguyên tắc trực quan hóa trung thực).

### Bài 9 (tùy chọn): Trừu tượng hóa dữ liệu

Bạn có bảng dữ liệu 5 cột: Tên, Tuổi, Cân nặng, Chiều cao, Nghề nghiệp. Trả lời 4 câu: cột nào định lượng, cột nào định tính. Cột nào liên tục, cột nào rời rạc. Nếu chỉ được giữ 2 cột để phân tích "sức khỏe", bạn giữ cột nào, vì sao. Bỏ cột nào trước nếu muốn bảo vệ quyền riêng tư, vì sao. Đây là bài tập về trừu tượng hóa cộng đạo đức dữ liệu, nền tảng cho chặng 08 và 70.

### Bài 10 (tùy chọn): Tự tạo bộ dữ liệu cá nhân

Tạo một tệp CSV (dùng Notepad hoặc VS Code) ghi lại 7 ngày dữ liệu về 1 việc bạn làm hằng ngày, ví dụ số phút tập thể thao mỗi ngày. Mở tệp CSV bằng Excel hoặc Google Sheets, quan sát: dữ liệu có cấu trúc không, có thể vẽ biểu đồ được không, bias có thể có (ngày cuối tuần so với ngày thường). Bạn sẽ làm việc kiểu này mỗi ngày ở Phần 2 với Pandas.

### Câu hỏi tự kiểm tra

Sau khi làm xong bài tập, trả lời 4 câu: dữ liệu là gì, nêu 4 dạng dữ liệu phổ biến kèm ví dụ. Nêu 3 quy tắc thu thập dữ liệu và 1 ví dụ vi phạm mỗi quy tắc. Phân biệt "nhận xét từ dữ liệu" và "ý kiến cá nhân", kèm 1 ví dụ mỗi loại. Vì sao dữ liệu quan trọng cho AI, nêu 2 hệ quả. Nếu trả lời được cả 4 câu mà không cần xem tài liệu, bạn đã sẵn sàng sang chặng 04 (khi phát hành).

## 3. Sản phẩm cuối chặng: "Báo cáo dữ liệu đầu tiên"

Mỗi chặng kết thúc bằng một sản phẩm đưa vào portfolio. Chặng 03 yêu cầu tạo tệp `portfolio-ai/phan-1/chặng-03-bao-cao-du-lieu/README.md` gồm 4 phần.

Phần 1 là câu hỏi khảo sát, viết câu hỏi bạn đã dùng kèm ghi ai được hỏi (nhóm, số người). Điều kiện đạt: câu hỏi rõ, có đối tượng và số người. Phần 2 là bảng dữ liệu, có tiêu đề, tên cột, số liệu, dòng tổng. Điều kiện đạt: đủ cấu phần, tổng khớp số người. Phần 3 là biểu đồ cột, vẽ trên giấy (scan hoặc ảnh) hoặc vẽ trên tool, có tiêu đề, trục, cột đúng tỉ lệ. Điều kiện đạt: cột đúng chiều cao theo số liệu bảng. Phần 4 là hai nhận xét rút ra từ dữ liệu. Điều kiện đạt: mỗi câu có số liệu làm bằng chứng.

Điểm nhấn: nếu bạn ghi sai số rồi sửa, tuyệt vời, đó là gỡ lỗi dữ liệu. Đừng sửa cho "báo cáo đẹp". Sản phẩm mục đích là sự thật, không phải thẩm mỹ. Lưu tệp vào portfolio. Đây là artifact thứ 3 của bạn trong hành trình 170 chặng.

### Gợi ý phân tích thêm

Tại sao không nên so sánh biểu đồ của bạn với người khác: mỗi người khảo sát một nhóm khác nhau, nên số khác là bình thường. So sánh "biểu đồ của tôi đúng hơn của bạn" sai về tư duy, không có "đúng" tuyệt đối, chỉ có "đại diện cho nhóm nào". Nếu muốn khảo sát nghiêm túc hơn, để khảo sát có giá trị thống kê: cỡ mẫu ít nhất 30 (lý tưởng ít nhất 100), chọn mẫu ngẫu nhiên từ dân số mục tiêu, câu hỏi trung lập (không gợi ý đáp án), bảo vệ thông tin cá nhân (không hỏi tên, số điện thoại). Sẽ học kỹ thuật khảo sát nghiêm túc ở Phần 2 (chặng 95, mẫu và tổng thể).

Biểu đồ cột phù hợp dữ liệu phân loại (loại nước, thành phố, giới tính). Các loại dữ liệu khác cần loại biểu đồ khác: tỷ lệ phần trăm dùng biểu đồ tròn (cơ cấu chi tiêu), theo thời gian dùng biểu đồ đường (nhiệt độ 7 ngày), quan hệ 2 biến dùng biểu đồ phân tán (chiều cao so với cân nặng), phân phối dùng histogram (phân bố điểm kiểm tra). Sẽ học các loại biểu đồ này ở chặng 56 (bảng tính) và chặng 88 đến 90 (Matplotlib và Seaborn).

## 4. Tự đánh giá và kết nối về sau

Checklist cuối chặng: tôi hiểu dữ liệu là gì, 4 dạng dữ liệu phổ biến. Tôi phân biệt được dữ liệu định lượng so với định tính, có cấu trúc so với phi cấu trúc. Tôi biết 3 quy tắc thu thập dữ liệu (đúng, đủ, trung thực). Tôi hiểu bias lấy mẫu là gì và vì sao cần tránh. Tôi đã làm xong Bài 1, 2, 3, 4, 5 (có sao). Tôi đã hoàn thành "Báo cáo dữ liệu đầu tiên" và lưu vào portfolio. Tôi phân biệt được "nhận xét từ dữ liệu" và "ý kiến cá nhân". Tôi đã ghi 1 mục vào `learning-journal.md` cho chặng này. Tôi đã trả lời được câu hỏi "Kết nối về sau" ở cuối chặng.

Nếu 9 trên 9 ô được đánh dấu, chúc mừng, bạn đã hoàn thành chặng 03. Phần 1 tiếp tục với chặng 04 (đang hoàn thiện).

### Thuật ngữ cần nhớ

Hai mươi chín thuật ngữ của chặng 03 sẽ xuất hiện lại nhiều lần. **Dữ liệu** (*data*) là thông tin được ghi lại, có thể lưu trữ, truyền tải, xử lý. **Dữ liệu số** (*numerical data*) đo lường bằng số. **Dữ liệu chữ** (*textual data*) dạng ký tự. **Dữ liệu hình** (*image data*) dạng ảnh. **Dữ liệu âm thanh** (*audio data*) dạng sóng âm. **Dữ liệu định lượng** (*quantitative data*) đo lường được bằng số. **Dữ liệu định tính** (*qualitative data*) mô tả đặc tính, không đo lường trực tiếp. **Dữ liệu liên tục** (*continuous data*) có thể lấy mọi giá trị trong khoảng. **Dữ liệu rời rạc** (*discrete data*) chỉ lấy giá trị đếm được. **Dữ liệu có cấu trúc** (*structured data*) sắp xếp theo hàng và cột, có lược đồ rõ. **Dữ liệu bán cấu trúc** (*semi-structured data*) có thẻ hoặc nhãn nhưng không theo bảng. **Dữ liệu phi cấu trúc** (*unstructured data*) không có cấu trúc cố định. **Thu thập dữ liệu** (*data collection*) là quá trình gom dữ liệu từ nguồn. **Mẫu** (*sample*) là tập con của dân số được khảo sát. **Dân số** (*population*) là toàn bộ đối tượng quan tâm. **Bias lấy mẫu** (*sampling bias*) là mẫu không đại diện cho dân số. **Bảng** (*table*) là cách sắp xếp dữ liệu theo hàng và cột. **Hàng** (*row* hay *record*) mỗi hàng là 1 bản ghi. **Cột** (*column* hay *field*) mỗi cột là 1 trường dữ liệu. **Ô** (*cell*) là giao cột và hàng, chứa 1 giá trị. **Biểu đồ cột** (*bar chart*) dùng cột cao để so sánh giá trị. **Trục** (*axis*) là đường đánh giá trị (x ngang, y dọc). **Trực quan hóa** (*data visualization*) là biểu diễn dữ liệu bằng hình ảnh. **Trọng tâm của dữ liệu** (*central tendency*) là giá trị "đại diện" cho dữ liệu. **Tập dữ liệu** (*dataset*) là tập hợp dữ liệu có liên quan. **Tập dữ liệu huấn luyện** (*training set*) là dữ liệu dùng để huấn luyện AI. **Làm sạch dữ liệu** (*data cleaning*) là sửa dữ liệu thiếu, sai, trùng. **Nhận xét từ dữ liệu** (*data-driven observation*) là câu nói có số liệu làm bằng chứng. **Ý kiến cá nhân** (*personal opinion*) là câu nói phản ánh cảm nhận, không số liệu.

Một câu nói nên nhớ: không có dữ liệu, không có AI. Thu thập đúng, đủ, trung thực. Nhận xét phải có số liệu làm bằng chứng, không bịa, không phóng đại. Dữ liệu trong đầu bạn không phải dữ liệu theo nghĩa máy tính, chỉ khi ghi lại mới thành dữ liệu.

### Tài nguyên mở rộng (tùy chọn)

Nếu muốn đi sâu hơn, các tài nguyên sau đều miễn phí hoặc dễ tiếp cận. **Google Data Analytics** trên Coursera (có phần miễn phí) là khóa phân tích dữ liệu cho người mới. **Data Visualization for All** của Trinity College (miễn phí) là khóa trực quan hóa dữ liệu. **SQL for Data Science** trên Coursera (có phần miễn phí) sẽ dùng ở chặng 58.

Sách gợi ý: *Naked Statistics* của Charles Wheelan là sách phổ thông về thống kê, dễ hiểu, hài hước, khuyến nghị đọc trước Phần 2. *The Art of Statistics* của David Spiegelhalter là sách về tư duy thống kê. *Storytelling with Data* của Cole Nussbaumer Knaflic là sách kinh điển về trực quan hóa dữ liệu cho người không chuyên. *Factfulness* của Hans Rosling là sách về cách đọc dữ liệu thế giới không bị cảm xúc lèo lái.

Trên YouTube: *"How to spot a misleading graph"* của Lea Gaslowitz (TED-Ed, 4 phút) trực quan về biểu đồ nói dối. *"The best stats you've ever seen"* của Hans Rosling (TED) là huyền thoại về trực quan hóa dữ liệu. Công cụ trực quan hóa miễn phí: [Google Sheets](https://sheets.google.com), [Data Studio](https://datastudio.google.com), [Flourish](https://flourish.studio), [RawGraphs](https://app.rawgraphs.io).

Tài nguyên tiếng Việt: VnExpress mục Data là blog phân tích dữ liệu tiếng Việt, The Data Story là blog về kể chuyện bằng dữ liệu, Học viện AI Việt Nam (AIO) có tài liệu về phân tích dữ liệu. Bộ dữ liệu miễn phí để thực hành: [Kaggle Datasets](https://www.kaggle.com/datasets), [Google Dataset Search](https://datasetsearch.research.google.com), [UCI ML Repository](https://archive.ics.uci.edu), [Awesome Public Datasets](https://github.com/awesomedata/awesome-public-datasets). Tập dữ liệu Việt Nam: Tổng cục Thống kê tại [gso.gov.vn](https://www.gso.gov.vn) có dữ liệu kinh tế xã hội, Our World in Data tại [ourworldindata.org](https://ourworldindata.org) có dữ liệu Việt Nam so sánh thế giới.

### Kết nối về sau

Các khái niệm của chặng 03 sẽ xuất hiện lại ở: **bảng, cột, hàng** (chặng 53 đến 56) Google Sheets, công thức, pivot table. **Bias lấy mẫu** (chặng 95) phân tích chính thức bằng khái niệm thống kê. **Làm sạch dữ liệu** (chặng 57 và 85) kỹ thuật Pandas. **Trực quan hóa** (chặng 56 và 88 đến 92) Matplotlib, Seaborn, dashboard. **Nhận xét từ dữ liệu** (chặng 93 đến 98) thống kê suy luận, p-value, kiểm định. **Tập dữ liệu huấn luyện** (chặng 64 và 101) ML formal definition. **Thiên vị dữ liệu** (chặng 69) bias mở rộng sang đạo đức AI. **Quyền riêng tư** (chặng 70) đạo đức dữ liệu chuyên sâu.

Không cần học thuộc ngay, cứ gặp lại là nhớ thêm. Lặp xoáy ốc. Cuối cùng, mở tệp `learning-journal.md` và thêm mục cho chặng 03, gồm: hôm nay tôi học được gì (5 đến 6 ý chính), khó khăn lớn nhất, cách vượt qua, sản phẩm đã làm (đường dẫn), câu hỏi mở cho chặng sau, và checklist 6 ô đánh dấu. Nhật ký này là tài sản quý nhất của bạn sau 170 chặng.
