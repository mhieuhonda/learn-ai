# Chặng 01 — Làm quen với thế giới AI xung quanh ta

Đây là chặng đầu tiên của lộ trình tự học. Mục tiêu không phải là nhồi nhét thuật ngữ, mà là giúp bạn nhìn ra AI đang ở quanh mình thế nào, hiểu được giới hạn thực sự của công nghệ này, và biết vì sao người ta nói "AI học từ dữ liệu" thay vì "AI được lập trình". Sau chặng này, bạn sẽ không còn nhầm ChatGPT với một "phần mềm tự động" hay đồng nhất AI với robot thông minh trong phim. Bạn sẽ có một khung khái niệm đủ vững để bước vào 169 chặng tiếp theo mà không bị ngợp.

Cách đọc chặng này: đi từ đầu đến cuối, không nhảy. Mỗi mục lớn xây trên mục trước. Khi gặp thuật ngữ mới, định nghĩa sẽ ở ngay tại chỗ, kèm một ví dụ cụ thể trước khi đi vào lý thuyết. Nếu bạn tò mò muốn mở rộng, cuối chặng có phần tài nguyên. Bạn không cần thuộc lòng ngay, chỉ cần đọc cho trôi ý.

## 1. Kiến thức

### AI là gì

Hãy bắt đầu từ một ví dụ đời thường: bạn nói "biết gì, mở YouTube giúp tôi". Điện thoại nghe giọng bạn, nhận ra đó là tiếng Việt, hiểu ý bạn muốn mở ứng dụng YouTube, rồi mở nó ra. Việc này từng cần một người: nghe, hiểu, ra quyết định, hành động. Nay máy tính làm được. Đó chính là **trí tuệ nhân tạo** (*Artificial Intelligence*, viết tắt **AI**) theo nghĩa thông dụng: ngành khoa học máy tính xây dựng các hệ thống có thể thực hiện những việc từng cần trí tuệ người, như nhận dạng hình ảnh, hiểu ngôn ngữ nói, chơi cờ, dịch văn bản, hay ra quyết định khi thông tin không chắc chắn.

Có nhiều cách định nghĩa chính thức hơn. Một định nghĩa phổ biến trong giáo trình chuẩn của Russell và Norvig (cuốn *Artificial Intelligence: A Modern Approach*, 2020) nói rằng AI là nghiên cứu về **agent** (tác tử), nghĩa là các hệ thống nhận thông tin từ môi trường qua cảm biến, rồi hành động qua cơ cấu tác động để đạt mục tiêu. Hai ý trong định nghĩa này quan trọng để nhớ: thứ nhất, AI là một agent, nghĩa là nó nhận input và tạo ra output có mục đích chứ không ngẫu nhiên; thứ hai, AI tương tác với môi trường, nó không tồn tại trong chân không mà vừa chịu ảnh hưởng vừa tác động trở lại. Khi bạn thấy xe tự lái dừng lại trước đèn đỏ, đó là một agent: camera thu hình ảnh đèn đỏ, hệ thống quyết định phanh, phanh tác động lên xe, xe dừng lại, môi trường xung quanh phản ứng theo.

Một định nghĩa khác phổ biến trong công nghiệp nói AI là tập hợp các kỹ thuật cho phép máy tính học từ dữ liệu để thực hiện việc cần trí tuệ người. Khác biệt then chốt với phần mềm truyền thống nằm ở chữ "học": phần mềm thường làm theo quy tắc do người viết tay, còn AI tự rút ra quy tắc từ rất nhiều dữ liệu ví dụ. Câu nói rút gọn cần nhớ là: AI là ngành xây agent thông minh, cách tiếp cận phổ biến nhất là cho máy học quy tắc từ rất nhiều dữ liệu thay vì viết tay quy tắc.

### Ba cấp độ AI theo năng lực

Khi đọc báo, bạn sẽ thấy nhiều cách phân loại AI. Cách chuẩn nhất phân theo năng lực. **AI hẹp** (*Narrow AI* hay *Weak AI*) là loại chỉ giỏi một việc cụ thể, ví dụ nhận dạng ảnh, dịch văn bản, chơi cờ vua. Mọi AI bạn dùng hằng ngày, từ ChatGPT đến hệ thống tự lái Tesla, đều là AI hẹp. Chúng rất giỏi việc của mình nhưng hoàn toàn không thể chuyển sang việc khác: ChatGPT không tự lái xe được, và hệ thống tự lái Tesla không viết thơ được. **AI tổng quát** (*Artificial General Intelligence*, viết tắt **AGI**) là cấp cao hơn, giả thuyết về một AI học được mọi việc mà trí tuệ người có thể học, có thể chuyển kiến thức giữa các lĩnh vực khác nhau. Cấp cao nhất là **siêu trí tuệ** (*Superintelligence*), vượt người trên mọi mặt trí tuệ.

Quan trọng phải rõ: hiện nay chưa có AGI hay siêu trí tuệ tồn tại, dù một số công ty như OpenAI, DeepMind, Anthropic tuyên bố hướng tới. Khi báo chí nói "AI sắp có ý thức" hay "AI sắp vượt người", đó thường là văn hóa pop hoặc strategic positioning, không phải tình trạng kỹ thuật thực. Bạn đọc tin như vậy, hãy luôn đặt câu hỏi: "Họ đang nói về AI hẹp (tồn tại) hay AGI (chưa tồn)?". Nếu không rõ, tin đó không đáng tin cậy tuyệt đối.

### Bốn lĩnh vực con chính

AI không phải khối thống nhất, mà là một ngành gồm nhiều lĩnh vực con. Bốn lĩnh vực phổ biến nhất, và là trọng tâm lộ trình này, có thể giới thiệu qua ví dụ đời thường.

**Học máy** (*Machine Learning*, viết tắt **ML**) là nhánh AI trong đó máy tự học quy tắc từ dữ liệu thay vì được người lập trình từng quy tắc. Để máy nhận dạng mèo, không ai viết quy tắc "tai nhọn cộng ria cộng bốn chân bằng mèo", vì có vô số ngoại lệ. Thay vào đó, người ta cho máy xem khoảng 10.000 ảnh mèo và 10.000 ảnh không phải mèo, máy tự tìm quy luật phân biệt. ML lại chia thành ba nhánh con thường gặp: **học có giám sát** (*supervised learning*) khi dữ liệu có nhãn rõ (ảnh mèo có nhãn "mèo", ảnh chó có nhãn "chó", máy học ánh xạ từ ảnh sang nhãn), **học không giám sát** (*unsupervised learning*) khi dữ liệu không nhãn và máy tự tìm cấu trúc ẩn (ví dụ phân cụm khách hàng theo hành vi mua sắm), và **học tăng cường** (*reinforcement learning*) khi máy học qua thử và sai kèm thưởng phạt (chơi cờ, đi xe, robot hút bụi). Bạn sẽ học sâu về ML ở Phần 3 (chặng 101 đến 120).

**Học sâu** (*Deep Learning*, viết tắt **DL**) là nhánh con của ML, dùng **mạng nơ-ron nhân tạo nhiều lớp** (*deep neural networks*). Chữ "sâu" ở đây không phải trí tuệ sâu, mà chỉ số lớp của mạng. DL đặc biệt mạnh với dữ liệu phi cấu trúc như ảnh, âm thanh, văn bản. ChatGPT, Midjourney, hệ thống tự lái, FaceID, tất cả đều dùng DL. Sẽ học sâu ở Phần 3 (chặng 121 đến 140).

**Thị giác máy tính** (*Computer Vision*, viết tắt **CV**) là nhánh AI xử lý ảnh và video: nhận dạng đối tượng, phát hiện khuôn mặt, phân đoạn ảnh, mô tả ảnh bằng văn bản. Khi bạn chụp ảnh điện thoại tự vẽ khung vàng quanh mặt người, đó là CV. Khi xe tự lái nhận ra người đi bộ qua đường, đó cũng là CV. CV thường kết hợp DL (đặc biệt một kiến trúc gọi là CNN) với xử lý ảnh số học. Sẽ gặp lại CV ở chặng 19, 66 và chuyên sâu ở chặng 127 đến 132.

**Xử lý ngôn ngữ tự nhiên** (*Natural Language Processing*, viết tắt **NLP**) là nhánh AI xử lý ngôn ngữ người, gồm văn bản và lời nói. Dịch máy, tóm tắt, phân loại cảm xúc, chatbot, hệ thống hỏi đáp đều thuộc NLP. Khi bạn nói với Google Assistant "Bây giờ mấy giờ?", máy nghe giọng (NLP), chuyển thành chữ, hiểu ý định, tra dữ liệu, nói lại câu trả lời. Đó là một pipeline NLP đầu cuối. Sẽ gặp lại NLP ở chặng 20, 67 và chuyên sâu ở chặng 133 đến 140.

Ngoài bốn lĩnh vực trên, AI còn có các nhánh khác như robot học, hệ chuyên gia, lập luận tự động, tìm kiếm và tối ưu. Các nhánh này ít phổ biến hơn trong ứng dụng thương mại hiện nay, nhưng quan trọng về mặt lịch sử và lý thuyết. Lộ trình này không đi sâu vào chúng, nhưng bạn sẽ gặp tên khi đọc tài liệu chuyên ngành.

### AI quanh bạn, sáu dấu chân trong đời sống

Để hiểu AI không phải thứ viễn tưởng, hãy xem sáu hệ thống AI mà bạn có thể đã dùng hôm nay.

**Trợ lý ảo** như Google Assistant, Siri, Alexa. Bạn nói "Bây giờ mấy giờ?", máy nghe giọng bạn, chuyển thành chữ, hiểu ý định, tra dữ liệu, nói lại câu trả lời. Đây là pipeline NLP đầu cuối, kết hợp nghe tiếng nói, dịch sang chữ, hiểu ý, truy xuất dữ liệu, và tạo giọng nói phản hồi.

**Hệ thống gợi ý video** trên YouTube, TikTok, Netflix. Khi bạn xem xong một video, hệ thống dùng lịch sử xem của bạn và hàng triệu người dùng tương tự để dự đoán video tiếp theo bạn có thể thích. Đây là ML, kết hợp học có giám sát (dự đoán tỷ lệ click) và học không giám sát (phân cụm người dùng theo hành vi).

**Dịch máy** như Google Dịch, DeepL. Bạn gõ câu tiếng Việt, hệ thống mã hóa câu thành chuỗi số, dịch chuyển ngữ nghĩa qua không gian số, rồi giải mã ra tiếng Anh. Đây là DL với một kiến trúc gọi là Transformer, sẽ học ở chặng 137.

**Mở khóa bằng khuôn mặt** (*FaceID*). Điện thoại nhìn mặt bạn, so với khuôn mặt đã đăng ký. Hệ thống dùng CV để trích đặc trưng khuôn mặt thành một chuỗi số, so khoảng cách giữa chuỗi mới với chuỗi đã lưu. Nếu gần đủ, mở khóa. Đây là DL cộng CV.

**Camera tự tìm mặt** khi chụp ảnh, vẽ khung vàng quanh mặt. Hệ thống quét ảnh theo cửa sổ trượt, mỗi cửa sổ đưa qua mạng nơ-ron đã huấn luyện để trả lời câu hỏi "đây có phải mặt người không". Đây cũng là CV cộng DL.

**Chatbot** như ChatGPT, Claude, Gemini. Bạn hỏi bằng văn bản, hệ thống dự đoán token (đơn vị chữ) tiếp theo có xác suất cao nhất dựa trên văn bản đã có, lặp lại nhiều lần để tạo câu trả lời. Đây là DL cộng NLP, dùng **mô hình ngôn ngữ lớn** (*Large Language Model*, viết tắt **LLM**).

Điểm chung của sáu hệ thống: mỗi cái đều "học" từ lượng dữ liệu khổng lồ trước khi hoạt động. Không có hệ thống nào được lập trình từng quy tắc tay. Đây là đặc trưng của AI hiện đại, và là sợi đỏ xuyên suốt lộ trình.

### AI giỏi việc gì, chưa giỏi việc gì

Hiểu giới hạn AI quan trọng không kém hiểu năng lực. AI hiện nay rất giỏi tính toán số học trên lượng lớn dữ liệu, tìm mẫu hình trong dữ liệu lớn, nhận dạng ảnh và âm thanh ở quy mô lớn, dịch văn bản giữa các ngôn ngữ phổ biến. AI hiện nay kém khi phải hiểu cảm xúc người khác, đưa ra quyết định đạo đức, sáng tạo kiến thức mới, học một việc mới chỉ từ một hai ví dụ, hay chuyển kiến thức giữa các lĩnh vực khác nhau.

Nguyên lý sâu xa: AI hiện nay giỏi việc lặp lại quy luật đã có trong dữ liệu, kém việc hiểu ngữ cảnh và chuyển ý nghĩa. Khi đọc tin "AI sắp thay thế X", hãy hỏi: "X có phải việc lặp quy luật dữ liệu, hay việc hiểu ngữ cảnh?". Câu trả lời cho biết mức độ đáng tin của tin. Ví dụ "AI thay thế nhân viên nhập liệu" khá đáng tin, vì nhập liệu là việc lặp quy luật. Còn "AI thay thế bác sĩ tâm lý" không đáng tin, vì bác sĩ tâm lý cần hiểu ngữ cảnh sâu, một việc AI chưa làm tốt.

### Học máy khác lập trình truyền thống ở đâu

Để thực sự hiểu AI, phải hiểu sự khác biệt với lập trình truyền thống. Trong **lập trình truyền thống**, người lập trình viết quy tắc rõ ràng. Ví dụ phần mềm tính thuế: mỗi trường hợp một dòng code kiểu "nếu thu nhập trên 11 triệu thì thuế bằng bao nhiêu". Ưu điểm là rõ ràng, kiểm chứng được. Nhược điểm là không khả thi với việc phức tạp: để máy nhận dạng mèo bằng quy tắc tay, bạn phải viết bao nhiêu dòng? Vô số, và vẫn sai.

Trong **học máy**, người lập trình không viết quy tắc. Họ viết một **thuật toán học** (sẽ học kỹ ở chặng 02), cung cấp **dữ liệu** gồm input và nhãn, thuật toán tự tìm ra quy tắc. Ưu điểm là mở rộng được cho việc phức tạp. Nhược điểm là quy tắc tìm được không dễ giải thích: khi ai hỏi "tại sao máy đoán đây là mèo?", câu trả lời thường là "vì mạng nơ-ron nói vậy", không trực diện như đọc code.

Lộ trình này bắt đầu bằng lập trình truyền thống (Phần 1, chặng 25 trở đi) trước khi sang ML (Phần 3), vì hiểu lập trình là nền cho hiểu ML. Nếu bạn vội vào ML mà chưa biết đọc code, sẽ bị ngợp.

### Một câu thần chú để nhớ

Sau khi đọc phần Kiến thức, hãy nhẩm một câu tóm tắt: AI là ngành xây dựng agent thông minh, cách tiếp cận phổ biến nhất là cho máy học quy tắc từ rất nhiều dữ liệu thay vì viết tay quy tắc, AI hiện nay đều là AI hẹp, giỏi việc lặp quy luật dữ liệu, kém việc hiểu ngữ cảnh. Nếu bạn có thể viết lại câu này bằng lời của mình mà không xem tài liệu, bạn đã hiểu phần Kiến thức. Nếu không, hãy đọc lại các mục trên trước khi sang phần Thực hành.

## 2. Thực hành

Để biến kiến thức thành trực giác, bạn cần tự tay quan sát và phản xạ. Bài tập sau xếp từ dễ đến khó, bài có dấu sao (★) là bắt buộc, bài không sao là tùy chọn mở rộng. Bạn có thể làm trực tiếp trong portfolio của mình, không cần ai đồng hành.

### Bài 1 ★: Săn tìm 6 dấu chân AI trong 3 ngày

Mở một tệp markdown `portfolio-ai/phan-1/chặng-01-nhat-ky-ai/observations.md`. Trong 3 ngày tiếp theo, mỗi ngày quan sát ít nhất 2 hệ thống AI bạn dùng hoặc gặp. Mỗi lần quan sát, ghi vào bảng có các cột: Ngày, Hệ thống, Input của nó, Output của nó, Dữ liệu nó đã học từ đâu, Lĩnh vực AI (ML, DL, CV, NLP hoặc tổ hợp).

Ví dụ để bạn hình dung: ngày 15/09, hệ thống "Gợi ý video YouTube", input là lịch sử xem của bạn, output là danh sách 10 video gợi ý, dữ liệu học từ lịch sử xem của hàng tỷ người, lĩnh vực là ML học có giám sát. Hoặc ngày 15/09, hệ thống "Mở khóa FaceID", input là ảnh khuôn mặt bạn hiện tại, output là quyết định mở hay không mở, dữ liệu học từ ảnh khuôn mặt bạn khi đăng ký cộng các biến đổi, lĩnh vực là DL cộng CV.

Cố gắng đa dạng: đừng chỉ lấy 6 ứng dụng điện thoại. Hãy để ý cả xe nhà bạn có camera lùi cảnh báo người không, chợ online có gợi ý "sản phẩm tương tự", tìm kiếm Google có tự hoàn thành câu. Sau 3 ngày, đánh dấu 1 hệ thống bạn thấy "ngạc nhiên nhất" và giải thích vì sao bằng 1 đến 2 câu. Tiêu chí đạt: đủ 6 hệ thống, mỗi hàng có 6 cột điền đủ, có ít nhất 1 hệ thống ngoài điện thoại.

### Bài 2 ★: Phân biệt AI với không-AI

Đánh dấu X vào cột phù hợp cho mỗi tình huống dưới đây. Cố gắng suy nghĩ trước khi xem đáp án ở cuối phần Thực hành.

| # | Tình huống | Có AI | Không AI |
|---|---|---|---|
| 1 | Máy tính thường cộng 25 + 75 | | |
| 2 | Điện thoại gợi ý từ tiếp theo khi bạn nhắn tin | | |
| 3 | Quạt quay theo nút bấm cấp 1, 2, 3 | | |
| 4 | Ứng dụng bản đồ vẽ lộ trình tránh đường kẹt | | |
| 5 | Đồng hồ báo thức reo đúng 6 giờ sáng mỗi ngày | | |
| 6 | Ứng dụng học tiếng Anh chấm giọng đọc của bạn | | |
| 7 | Máy lạnh tự tăng giảm theo nhiệt độ phòng và thói quen nhà | | |
| 8 | Cái kéo cắt giấy | | |
| 9 | ChatGPT trả lời câu hỏi của bạn | | |
| 10 | Email được tự động phân vào "Spam" | | |
| 11 | Viva Insights gợi ý "Bạn có 2 cuộc họp trùng lịch" | | |
| 12 | Bộ lọc Instagram thêm hiệu ứng mèo lên mặt bạn | | |
| 13 | Excel tính `=SUM(A1:A10)` | | |
| 14 | Google Photos nhóm ảnh theo người trong ảnh | | |
| 15 | Tivi tự tăng brightness khi phòng sáng | | |

Sau khi đánh dấu, viết 1 đoạn khoảng 100 chữ giải thích: điểm khác cốt lõi giữa hệ thống có AI và không AI là gì. Gợi ý: AI phải "học" từ dữ liệu, không AI thì làm theo quy tắc cố định.

### Bài 3 (tùy chọn): Phân tích 1 hệ thống AI sâu hơn

Chọn 1 hệ thống AI bạn dùng nhiều, ví dụ ChatGPT, gợi ý YouTube, Google Dịch. Tránh ChatGPT nếu bạn chỉ mới dùng vài lần, hãy chọn hệ thống bạn thực sự quen. Viết 1 bài 300 đến 500 chữ trả lời sáu câu: input chính của hệ thống là gì, output chính là gì, dữ liệu huấn luyện bạn đoán đến từ đâu (nguồn, loại, lượng ước lượng), một việc hệ thống làm tốt và vì sao, một việc hệ thống làm kém và vì sao, nếu bạn là kỹ sư của hệ thống bạn sẽ thu thập thêm dữ liệu gì để cải thiện.

Bài này không có đáp án đúng. Mục đích là tập tư duy ngược: từ trải nghiệm người dùng ngược đoán thiết kế bên trong. Đây là kỹ năng quan trọng của mọi kỹ sư AI sau này.

### Bài 4 (tùy chọn): Trò chơi "Huấn luyện máy từ thẻ hình"

Trò chơi này giúp bạn trải nghiệm trực giác về học máy mà không cần máy tính. Chuẩn bị 10 tấm thẻ giấy cắt vuông 5x5 cm, bút. Vẽ 6 tấm hình đồ vật: quả cam, quả bóng, cuốn sách, cái ly, viên gạch, quả bầu dục. Còn 4 tấm để trống, bạn sẽ tự điền sau.

Cách chơi: bạn đóng vai "máy", chỉ nhận biết bằng 2 tính chất bạn chọn, ví dụ "tròn" và "không tròn". Sau đó bạn đóng vai "người dạy máy", xem 3 đến 4 ví dụ quả tròn (cam, bóng, bầu dục) và tự phát hiện quy tắc: tròn là quả tròn. Đưa thẻ "viên gạch" cho "máy", bạn phải hỏi "đây là quả tròn không" và trả lời kèm lý do dựa trên quy tắc đã học.

Bước quan trọng nhất: thử dữ liệu xấu. Nếu ban đầu chỉ cho "máy" xem quả cam và quả bóng to, máy sẽ học quy tắc "to và tròn mới là quả tròn", rồi chối quả bầu dục nhỏ. Đây là hiện tượng **overfitting** (quá khít), máy học quá sát vào ví dụ cụ thể, không khái quát được. Sau khi chơi, viết 2 đến 3 dòng vào `observations.md` rút ra về mối quan hệ giữa dữ liệu huấn luyện và hành vi của máy. Đây là nền tảng trực giác cho chặng 105 (Overfitting và Underfitting) sau này.

### Bài 5 (tùy chọn): Báo cáo "Ví dụ xấu"

Nghĩ tình huống sau: bạn được giao huấn luyện AI nhận biết "cán bộ nhà nước" qua ảnh, nhưng chỉ có dữ liệu 1000 cán bộ, tất cả đều đeo kính. Viết 2 câu trả lời: máy học sai khi nào, và để máy học đúng hơn ta cần cho nó xem thêm gì.

Mở rộng (tùy chọn): tự đặt 1 tình huống "ví dụ xấu" tương tự trong lĩnh vực bạn quan tâm, như y tế, giáo dục, nông nghiệp. Viết câu hỏi và câu trả lời theo mẫu trên. Bài này là lần đầu bạn chạm vào ý tưởng quan trọng: dữ liệu không tốt làm máy đối xử không công bằng. Lộ trình sẽ quay lại ý tưởng này ở chặng 69 (thiên vị dữ liệu) khi bạn đã có đủ công cụ để phân tích sâu.

### Bài 6 (tùy chọn): AI mơ ước của tôi

Vẽ hoặc mô tả bằng văn bản một hệ thống AI bạn mong có trong tương lai, kèm 5 mục: tên hệ thống, giúp ai (người khiếm thị, bác nông dân, học sinh vùng sâu, chính bạn), làm được điều gì mà ngày nay chưa có, dữ liệu nào cần có để huấn luyện, rủi ro đạo đức gì có thể xảy ra. Bạn sẽ học cách phân tích rủi ro ở chặng 69 đến 74.

### Đáp án Bài 2

| # | Tình huống | Có AI | Không AI | Lý do |
|---|---|---|---|---|
| 1 | Máy tính cộng 25 + 75 | | X | Tính toán cố định, không học |
| 2 | Gợi ý từ nhắn tin | X | | Học từ lịch sử nhắn của hàng triệu người |
| 3 | Quạt quay theo nút | | X | Quy tắc cơ học |
| 4 | Bản đồ tránh kẹt | X | | Học từ dữ liệu giao thông thời gian thực |
| 5 | Đồng hồ báo thức | | X | Quy tắc cố định |
| 6 | Chấm giọng đọc tiếng Anh | X | | Học từ hàng triệu mẫu giọng |
| 7 | Máy lạnh theo thói quen | X | | Học từ dữ liệu sử dụng |
| 8 | Kéo cắt giấy | | X | Vật lý, không phải máy tính |
| 9 | ChatGPT | X | | LLM dự đoán token từ dữ liệu huấn luyện |
| 10 | Email vào Spam | X | | Học từ hàng triệu email đã được đánh dấu |
| 11 | Viva Insights báo trùng lịch | X | | Học từ dữ liệu lịch của tổ chức |
| 12 | Bộ lọc Instagram thêm mèo | X | | CV cộng DL theo dõi điểm mặt |
| 13 | Excel tính SUM | | X | Hàm cố định |
| 14 | Google Photos nhóm theo người | X | | CV cộng DL nhận diện khuôn mặt |
| 15 | Tivi tăng brightness | | X | Cảm biến ánh sáng cố định |

Điểm cốt lõi: hệ thống có AI học từ dữ liệu để đưa ra quyết định, hệ thống không AI làm theo quy tắc cố định do người viết. Câu hỏi phân biệt nhanh: hệ thống có cần học từ lượng dữ liệu lớn mới làm được việc đó không. Nếu có, là AI. Nếu không, chỉ cần quy tắc if-else, không phải AI.

## 3. Sản phẩm cuối chặng: "Nhật ký AI" 5 phần

Mỗi chặng kết thúc bằng một sản phẩm cụ thể để đưa vào portfolio. Chặng 01 yêu cầu bạn tạo một tệp markdown tại `portfolio-ai/phan-1/chặng-01-nhat-ky-ai/README.md` gồm 5 phần.

Phần 1 là định nghĩa AI, 1 đến 2 câu viết bằng lời bạn, không chép tài liệu. Điều kiện đạt: có nhắc "học từ dữ liệu" và "làm việc cần trí tuệ người". Phần 2 là bảng phân loại AI với 3 cấp độ (hẹp, tổng quát, siêu trí tuệ) kèm tình trạng hiện tại, đúng theo như đã học. Phần 3 là bảng 4 lĩnh vực con (ML, DL, CV, NLP), mỗi lĩnh vực 1 dòng mô tả. Phần 4 là bảng 6 hệ thống AI bạn quan sát được trong 3 ngày theo mẫu của Bài 1, đủ 6 ví dụ với 5 cột điền đủ. Phần 5 là 1 câu hỏi mở về AI bạn muốn tìm hiểu tiếp, ví dụ "làm sao máy học được ngữ cảnh". Câu hỏi phải cụ thể và có thể trả lời dần qua lộ trình.

Lưu tệp vào portfolio. Đây là artifact đầu tiên trong hành trình 170 chặng. Đừng bỏ qua chỉ vì "đơn giản": thói quen tạo sản phẩm sau mỗi chặng là sợi dây giữ bạn đi đến hết lộ trình.

## 4. Tự đánh giá và kết nối về sau

Checklist cuối chặng, đánh dấu X vào mỗi ô khi đạt. Tôi đã đọc toàn bộ phần Kiến thức. Tôi có thể giải thích AI bằng lời của mình (test Feynman). Tôi có thể phân biệt AI hẹp, tổng quát, siêu trí tuệ. Tôi có thể liệt kê 4 lĩnh vực con của AI kèm ví dụ. Tôi đã làm xong Bài 1 và Bài 2 (có sao). Tôi đã hoàn thành "Nhật ký AI" và lưu vào portfolio. Tôi đã ghi 1 mục vào `learning-journal.md` cho chặng này. Tôi đã trả lời được câu hỏi "Kết nối về sau" ở cuối chặng.

Nếu 8 trên 8 ô được đánh dấu, chúc mừng, bạn đã hoàn thành chặng 01, sang [chặng 02](../giai-doan-02-tu-duy-giai-quyet-van-de/README.md). Nếu có ô chưa đánh dấu, đừng sang chặng sau, trở lại phần tương ứng.

### Thuật ngữ cần nhớ

Mười thuật ngữ đầu tiên trong lộ trình sẽ xuất hiện lại nhiều lần, không cần học thuộc ngay, cứ gặp lại là nhớ thêm. **Trí tuệ nhân tạo** (*Artificial Intelligence*, AI) là ngành khoa học máy tính xây hệ thống làm được việc cần trí tuệ người, ví dụ ChatGPT, hệ thống tự lái, FaceID. **AI hẹp** (*Narrow AI*) xử lý một việc cụ thể rất giỏi, không chuyển lĩnh vực, mọi AI hiện nay đều thuộc loại này. **AI tổng quát** (*AGI*) học được mọi việc trí tuệ người học được, chưa tồn tại. **Học máy** (*Machine Learning*, ML) là nhánh AI trong đó máy tự học quy tắc từ dữ liệu, ví dụ gợi ý YouTube, lọc email spam. **Học sâu** (*Deep Learning*, DL) là nhánh ML dùng mạng nơ-ron nhiều lớp, ví dụ ChatGPT, Midjourney, FaceID. **Thị giác máy tính** (*Computer Vision*, CV) xử lý ảnh và video, ví dụ nhận diện khuôn mặt. **Xử lý ngôn ngữ tự nhiên** (*Natural Language Processing*, NLP) xử lý ngôn ngữ người, ví dụ dịch máy, chatbot. **Dữ liệu** (*data*) là thông tin được ghi lại: số, chữ, hình, âm. **Tập dữ liệu huấn luyện** (*training dataset*) là dữ liệu dùng để huấn luyện mô hình AI, ví dụ 10.000 ảnh mèo để máy nhận mèo. **Agent** là hệ thống nhận input, ra quyết định, hành động để đạt mục tiêu, ví dụ robot hút bụi, AI chơi cờ.

Một câu nói nên nhớ: AI hiện nay đều là AI hẹp, cách tiếp cận phổ biến nhất là cho máy học quy tắc từ rất nhiều dữ liệu thay vì viết tay quy tắc, AI giỏi việc lặp quy luật dữ liệu, kém việc hiểu ngữ cảnh.

### Tài nguyên mở rộng (tùy chọn)

Nếu muốn đi sâu hơn ngoài chặng, các tài nguyên sau đều miễn phí hoặc dễ tiếp cận. **Elements of AI** của Đại học Helsinki (có bản tiếng Việt) là khóa 6 chương về AI cho người không chuyên kỹ thuật, khuyến nghị làm xong sau chặng 03. **Google AI Education: Introduction to AI** là khóa ngắn giới thiệu AI. **AI for Everyone** của Andrew Ng trên Coursera tập trung hiểu AI ở cấp quản lý, không mã hóa. Trên YouTube, video *"How AI works"* của Code.org (tiếng Anh có phụ đề) giới thiệu AI trong 5 phút, và *"3Blue1Brown: But what is a neural network?"* giải thích mạng nơ-ron trực quan (xem trước chặng 121).

Nếu muốn đọc sách, *Life 3.0* của Max Tegmark (2017) là sách phổ thông về tương lai AI, *Weapons of Math Destruction* của Cathy O'Neil (2016) là sách kinh điển về thiên vị dữ liệu (sẽ đọc sâu hơn ở chặng 69), *AI Superpowers* của Kai-Fu Lee (2018) nhìn AI từ góc địa chính trị. Công cụ để thử nghiệm trực tiếp gồm [Teachable Machine](https://teachablemachine.withgoogle.com) để huấn luyện mô hình CV không cần code (chặng 19), [ChatGPT](https://chat.openai.com), [Claude](https://claude.ai), [Gemini](https://gemini.google.com) để thử các LLM, [Scratch](https://scratch.mit.edu) sẽ dùng để lập trình từ chặng 09.

Khi đọc tài liệu AI, ba lưu ý quan trọng: phân biệt tin quảng cáo và tin kỹ thuật, báo chí phổ thông thường nói "AI sắp thay thế X" kiểu phóng đại, tin kỹ thuật (arxiv blog, MIT Tech Review) khiêm tốn hơn; cẩn thận với "AI có ý thức" hay "AI sợ con người", đây là văn hóa pop, không phải khoa học, AI hiện nay không có ý thức, cảm xúc, hay ý định; cẩn thận với "AI 100% chính xác", không có hệ thống AI nào 100% chính xác, câu hỏi quan trọng là "sai bao nhiêu, sai kiểu gì".

### Kết nối về sau

Các thuật ngữ và khái niệm của chặng 01 sẽ xuất hiện lại ở các chặng sau: **thuật toán** (chặng 02) bạn sẽ học cách viết thuật toán chính xác, nền tảng của lập trình. **Dữ liệu** (chặng 03) bạn sẽ học cách thu thập, sắp xếp, trực quan hóa dữ liệu. **Overfitting** (chặng 18 và 105) quay lại dưới góc kỹ thuật, có công cụ đo lường. **Mô hình, inference, training** (chặng 62 và 101) được định nghĩa chính thức khi bạn vào Phần 3. **Thiên vị dữ liệu** (chặng 69), "ví dụ xấu" của Bài 5 sẽ được phân tích bằng khái niệm bias. **AGI** (chặng 17 và 161) quay lại câu hỏi "máy có suy nghĩ không" với nền tảng kỹ thuật sâu hơn.

Không cần học thuộc ngay, cứ gặp lại là nhớ thêm một tầng ý nghĩa mới. Lộ trình áp dụng nguyên lý lặp xoáy ốc: cùng một khái niệm quay lại nhiều lần ở mức sâu hơn. Cuối cùng, mở tệp `learning-journal.md` (tạo nếu chưa có) và thêm mục cho chặng này, gồm: hôm nay tôi học được gì (4 đến 5 ý chính), khó khăn lớn nhất của tôi, cách tôi vượt qua, sản phẩm đã làm (đường dẫn đến portfolio), câu hỏi mở cho chặng sau, và checklist 6 ô đánh dấu. Nhật ký này sẽ là tài sản quý nhất của bạn sau 170 chặng, đừng bỏ qua.
