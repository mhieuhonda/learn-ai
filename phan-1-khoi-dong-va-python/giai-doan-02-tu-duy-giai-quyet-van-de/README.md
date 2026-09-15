# Chặng 02 — Tư duy giải quyết vấn đề: các bước nhỏ dẫn đến thành công

Đây là chặng nền tảng quan trọng nhất của Phần 1. Bạn sẽ học **tư duy máy tính** (*computational thinking*), kỹ năng mà mọi lập trình viên, kỹ sư AI, nhà nghiên cứu đều dùng hằng ngày. Không cần máy tính, không cần biết gõ lệnh, chỉ cần sự kiên nhẫn để phân rã việc lớn thành các bước nhỏ rõ ràng. Sau chặng này, bạn sẽ hiểu vì sao máy tính chỉ làm đúng khi được chỉ dẫn chính xác, vì sao "đoán ý" là đặc quyền của người chứ không phải máy, và vì sao "gỡ lỗi" quan trọng hơn "viết đúng ngay lần đầu".

Cách đọc chặng này giống chặng 01: đi từ đầu đến cuối, không nhảy. Khi gặp khái niệm mới, định nghĩa sẽ ở ngay tại chỗ, kèm một ví dụ cụ thể trước khi đi vào lý thuyết. Cuối chặng có phần tài nguyên mở rộng cho ai muốn đi sâu.

## 1. Kiến thức

### Tư duy máy tính là gì và gồm bốn kỹ năng nào

Hãy bắt đầu từ một câu hỏi tưởng đơn giản: nếu bạn nhờ em trai 8 tuổi "đi mua cho anh một tô phở", bạn sẽ phải dặn những gì? Có lẽ: "đi qua đường cẩn thận, đến tiệm ông Ba đầu ngõ, nói ông cho một tô tái, nhiều hành, không hành lá, lấy thêm tương đen, rồi cầm về cẩn thận không đổ". Bạn vừa làm tư duy máy tính mà không biết. Bạn đã chia một việc lớn (mua phở) thành các bước nhỏ theo trật tự, bạn đã nêu điều kiện (nhiều hành, không hành lá), bạn đã dùng ngôn ngữ cụ thể để người nghe làm đúng. Đó chính là **tư duy máy tính**, quá trình tư duy để giải quyết vấn đề theo cách mà máy tính có thể thực hiện.

Tư duy máy tính gồm bốn thành phần. **Phân rã** (*decomposition*) là chia vấn đề lớn thành các phần nhỏ dễ giải quyết, ví dụ chia "tổ chức sinh nhật" thành mời khách, đặt bánh, trang trí, đón bạn, cắt bánh. **Nhận dạng mẫu hình** (*pattern recognition*) là tìm quy luật lặp lại trong vấn đề hoặc giữa các vấn đề, ví dụ nhận ra rằng đánh răng, rửa mặt, tắm đều bắt đầu bằng "chuẩn bị nước" và kết thúc bằng "lau khô", nên có thể viết một quy trình mẫu chung rồi điền chi tiết. **Trừu tượng hóa** (*abstraction*) là lọc thông tin quan trọng, bỏ chi tiết thừa, ví dụ bản đồ bỏ qua màu nhà, chỉ giữ tên đường và hình tuyến đường. **Thiết kế thuật toán** (*algorithm design*) là viết dãy bước rõ ràng, đúng thứ tự để giải quyết vấn đề. Bốn kỹ năng này không tách rời, chúng đan xen: phân rã xong mới nhận mẫu hình, nhận được mới trừu tượng hóa, trừu tượng xong mới viết thuật toán.

Điểm quan trọng cần rõ: tư duy máy tính không phải "tư duy như máy", mà là "tư duy để giao tiếp với máy". Máy không có trực giác, không có ngữ cảnh, không "đoán ý" được. Khi bạn giải thích một việc cho máy, bạn phải làm theo bốn bước trên, vì máy không có cách nào khác để hiểu. Lộ trình 170 chặng xây toàn bộ kỹ năng AI trên nền tư duy máy tính, bạn sẽ gặp lại bốn thành phần này ở mọi chặng.

### Thuật toán, trật tự và điều kiện: ba khái niệm để giao tiếp với máy

Từ bốn kỹ năng trên, **thiết kế thuật toán** là kỹ năng thực hành nhiều nhất, nên cần hiểu rõ. **Thuật toán** (*algorithm*) là dãy các bước rõ ràng, đúng thứ tự, có thể thực hiện được, để giải quyết một vấn đề hoặc hoàn thành một việc. Một dãy bước được gọi là thuật toán khi thỏa bốn điều kiện: đầu vào rõ (biết trước dữ liệu gì cần có, ví dụ nguyên liệu nấu mì), đầu ra rõ (biết trước kết quả mong đợi, ví dụ tô mì ăn được), mỗi bước thực hiện được (mỗi bước là hành động cụ thể, không mơ hồ), và dừng được (sau hữu hạn bước, thuật toán kết thúc, không lặp vô hạn).

Ví dụ kinh điển: thuật toán nấu mì gói. Bước 1, đun 500ml nước trong nồi đến khi sôi. Bước 2, mở gói mì và gói gia vị. Bước 3, khi nước sôi, thả mì vào nồi. Bước 4, đun thêm 3 phút, khuấy nhẹ. Bước 5, tắt bếp, đổ mì ra tô. Bước 6, cho gói gia vị vào tô, trộn đều. Bước 7, thưởng thức. Bảy bước trên thỏa cả bốn điều kiện: đầu vào là 1 gói mì và 500ml nước, đầu ra là tô mì ăn được, mỗi bước là hành động cụ thể, và thuật toán dừng sau 7 bước.

Thuật toán không phải duy nhất: cùng một việc có nhiều thuật toán. Nấu mì có thể cho gia vị vào nồi trước khi tắt bếp, hoặc cho vào tô sau, cả hai đều đúng. Điểm khác biệt nằm ở **trật tự** (*sequence*), thứ tự thực hiện các lệnh. Máy tính thực hiện lệnh theo trật tự chính xác như đã viết, đổi trật tự là đổi kết quả. Đây là khác biệt cốt lõi giữa giao tiếp với máy và giao tiếp với người. Người có thể hiểu "nấu mì rồi ăn" dù bạn nói ngược "ăn rồi nấu mì", vì người có ngữ cảnh và biết bạn nói nhầm. Máy tính thì thực hiện đúng như bạn nói, nếu bạn bảo "ăn mì" trước "nấu mì", máy sẽ cố ăn khi chưa có mì, lỗi.

Ví dụ trật tự quan trọng: thuật toán "sai trật tự" nấu mì: bước 1 ăn mì, bước 2 nấu mì, bước 3 đun nước. Hiển nhiên vô lý, nhưng máy tính sẽ làm đúng theo thứ tự này nếu bạn ra lệnh vậy. Bài học rút ra: khi viết thuật toán cho máy, luôn tự hỏi "trật tự này có ý nghĩa không, đổi trật tự có ảnh hưởng kết quả không". Đây là phản xạ bạn cần rèn.

Nhiều việc thực tế không phải lúc nào cũng giống nhau. Có lúc cần quyết định: "nếu A thì làm X, nếu B thì làm Y". Đó là **điều kiện** (*condition*), bước chỉ thực hiện khi thoả một điều kiện nào đó. Cấu trúc điều kiện phổ biến là "NẾU điều kiện THÌ hành động", có thể thêm "NẾU KHÔNG THÌ hành động khác". Ví dụ trong thuật toán nấu mì: nếu nước chưa sôi thì đợi thêm 1 phút rồi kiểm tra lại, nếu nước đã sôi thì thả mì vào. Điều kiện cho phép thuật toán thích ứng với tình huống thay vì chạy cứng theo một đường, đây là nền tảng của mọi chương trình có logic phức tạp. Bạn sẽ viết điều kiện bằng Scratch ở chặng 12, bằng Python ở chặng 29.

### Lệnh chính xác, máy không đoán ý

Máy tính thực hiện lệnh đúng theo nghĩa đen (*literal interpretation*). Nếu bạn nói "tiến đến gần cái bàn", máy sẽ hỏi: "gần là bao nhiêu cm?". Nếu bạn nói "đi quanh phòng", máy sẽ hỏi: "quanh theo chiều nào, mấy bước?". Khác với người có thể "đoán ý" từ ngữ cảnh, máy cần mọi lệnh đều cụ thể, đo lường được, không mơ hồ.

Ví dụ: bạn nói với trợ lý ảo "đặt báo thức sáng mai". Trợ lý sẽ hỏi: "mấy giờ, báo thức loại gì (chuông, nhạc, rung), lặp lại không". Đây không phải vì trợ lý "ngu", mà vì nó cần thông tin cụ thể để thực hiện. Người thì tự đoán "sáng mai chắc là 6 giờ", nhưng đoán có thể sai, và máy không được phép đoán. Nguyên lý giao tiếp với máy: lệnh cụ thể không mơ hồ, số liệu rõ (khoảng cách, thời gian, số lượng), điều kiện rõ (nếu X thì làm Y, ngược lại làm Z), không kỳ vọng máy "hiểu ý" khi bạn nói chung chung. Kỹ năng này trở thành phản xạ khi bạn lập trình từ Phần 1 trở đi, nhưng rèn ngay từ bây giờ bằng bài tập phần 2.

### Gỡ lỗi và mã giả: quy trình hằng ngày của người viết code

Khi viết thuật toán hoặc viết code, lỗi là điều tất yếu. **Gỡ lỗi** (*debugging* hay *debug*) là quá trình tìm và sửa lỗi. Đây không phải việc xui xẻo, mà là việc hằng ngày của mọi lập trình viên. Có ước tính: lập trình viên dành 50 đến 80% thời gian gỡ lỗi, không phải viết code mới. Nếu bạn học được cách gỡ lỗi có kỷ luật, bạn đã có được một nửa kỹ năng của người làm công nghệ.

Quy trình gỡ lỗi bốn bước. Bước 1, xác định triệu chứng: kết quả sai kiểu gì, khác mong đợi ở điểm nào. Bước 2, cô lập vị trí lỗi: bước nào trong thuật toán gây ra sai, chạy từng bước và kiểm tra kết quả trung gian. Bước 3, tìm nguyên nhân gốc: vì sao bước đó sai, do nhập sai dữ liệu, trật tự sai, hay điều kiện sai. Bước 4, sửa và kiểm tra lại: sửa lỗi, chạy lại toàn bộ, xác nhận kết quả đúng, nếu vẫn sai thì lặp lại quy trình.

Ví dụ: thuật toán nấu mì bị sai, mì nhão. Triệu chứng: mì nhão, không săn. Cô lập: bước 4 "đun thêm 3 phút" có thể quá lâu. Nguyên nhân: mì gói thường chỉ cần 2 phút, 3 phút làm mì nhũn. Sửa: đổi 3 phút thành 2 phút, nếm thử trước khi tắt bếp. Tư duy quan trọng cần giữ: lỗi không phải thất bại, lỗi là **dữ liệu**. Mỗi lần gặp lỗi và sửa được, bạn học thêm một "cái bẫy" để tránh sau này. Ghi lại vào `lessons-learned.md`, vài tháng sau bạn có một kho "những cái bẫy đã qua", tài sản quý nhất của người tự học.

Trước khi viết code thật (Python, Scratch), người ta thường viết **mã giả** (*pseudocode*), dạng văn bản gần ngôn ngữ người, có cấu trúc gần ngôn ngữ máy. Mã giả không có cú pháp cố định, mục đích là làm rõ thuật toán trước khi hiện thực. Ví dụ mã giả cho "tìm số lớn nhất trong 3 số":

```
INPUT: a, b, c (3 số)
OUTPUT: số lớn nhất

largest = a
IF b > largest THEN
    largest = b
IF c > largest THEN
    largest = c
RETURN largest
```

Mã giả giúp bạn suy nghĩ thuật toán mà không vướng cú pháp ngôn ngữ, trao đổi thuật toán với người khác không phụ thuộc ngôn ngữ lập trình, và chuyển sang code thật dễ hơn (mỗi dòng mã giả thường tương ứng 1 đến 2 dòng code). Từ chặng 25 (Python) trở đi, bạn sẽ viết mã giả trước khi code, đây là thói quen quan trọng.

### Một câu thần chú để nhớ

Tư duy máy tính bằng bốn kỹ năng: phân rã, nhận dạng mẫu hình, trừu tượng hóa, thiết kế thuật toán. Máy chỉ hiểu lệnh cụ thể, không đoán ý. Lỗi là dữ liệu quý, gỡ lỗi là kỹ năng hằng ngày. Nếu bạn viết lại được câu này bằng lời của mình mà không xem tài liệu, bạn đã hiểu phần Kiến thức.

## 2. Thực hành

Bài tập cho chặng 02 xếp từ dễ đến khó. Bài có dấu sao (★) là bắt buộc, bài không sao là tùy chọn mở rộng. Tất cả tự làm một mình.

### Bài 1 ★: Phân rã 3 việc hằng ngày

Chọn 3 việc từ danh sách dưới hoặc tự chọn: tổ chức sinh nhật cho bạn, đi học đúng giờ (từ lúc ngủ dậy đến lúc vào lớp), làm sạch bàn học, nấu một món bạn biết, mua sắm ở siêu thị, lập kế hoạch đi du lịch 2 ngày, soạn cặp sách cho ngày hôm sau, trả lời một email quan trọng. Mỗi việc, phân rã thành 5 đến 8 bước nhỏ rõ ràng, đúng trật tự.

Format trả lời đơn giản: ghi tên việc, rồi "Bước 1: [hành động cụ thể]", "Bước 2: [hành động cụ thể]", cho đến bước N. Lưu vào `portfolio-ai/phan-1/chặng-02-sach-thuat-toan/decomposition.md`. Tiêu chí đạt: mỗi việc có 5 đến 8 bước (không quá ngắn, không quá dài), mỗi bước là hành động cụ thể có động từ rõ, trật tự đúng logic, không có bước mơ hồ như "chuẩn bị xong" hay "làm tốt".

### Bài 2 ★: Sửa thuật toán "nấu mì bị hỏng"

Thuật toán sau có 3 lỗi cài sẵn, tìm và sửa.

```
Thuật toán nấu mì gói:
1. Đun 500ml nước trong nồi.
2. Thả mì vào nước lạnh ngay.
3. Đợi 5 phút, tắt bếp.
4. Sau đó mới mở gói gia vị bỏ vào.
5. Đổ mì ra tô và thưởng thức.
```

Yêu cầu: gạch chân mỗi bước sai, viết lý do sai, viết lại toàn bộ thuật toán đúng, có thể thêm bước thiếu nếu cần. Gợi ý: ít nhất 3 lỗi về trật tự, về điều kiện thiếu, và về bước thiếu. Xem đáp án ở cuối phần Thực hành, nhưng đừng xem trước khi đã thử 30 phút.

### Bài 3 ★: Trò chơi "Chỉ lệnh cho máy" phiên bản lưới ô vuông

Trò chơi giúp bạn trải nghiệm trực tiếp việc giao tiếp với máy không đoán ý. Chuẩn bị 2 tờ giấy kẻ ô vuông (lưới 5x5 hoặc 8x8), 1 vật nhỏ làm "mục tiêu" (đồng xu, cục tẩy), 1 vật nhỏ làm "robot" (hòn đá, cục tẩy khác).

Cách chơi chia hai lần. Lần 1, bạn đóng vai "người ra lệnh": đặt "robot" ở ô góc dưới trái của tờ 1, đặt "mục tiêu" ở một ô khác (bạn chọn). Bạn giữ tờ 1 (có robot và mục tiêu), tờ 2 để trống đặt cạnh. Bạn sẽ chỉ lệnh cho "máy" (chính bạn, đóng vai máy) di chuyển robot đến mục tiêu, nhưng đóng vai máy không được nhìn tờ 1, chỉ dùng tờ 2 để vẽ lại vị trí robot sau mỗi lệnh. Lệnh phải rất cụ thể: "tiến 1 ô lên trên" là cụ thể (đạt), "tiến đến gần mục tiêu" là mơ hồ (không đạt, gần là bao nhiêu ô), "rẽ phải" là cụ thể (đạt), "đi quanh phòng" là mơ hồ (không đạt, quanh theo chiều nào, mấy bước).

Lần 2, bẫy lệnh: bạn cố tình ra lệnh mơ hồ và quan sát "máy" hỏi lại. Ví dụ "đi chậm thôi" thì máy hỏi "chậm là bao nhiêu ô mỗi lượt", "đi vòng qua cái bàn" thì máy hỏi "vòng qua bên nào, mấy bước", "đến gần mục tiêu" thì máy hỏi "gần là bao nhiêu ô". Sau khi chơi, viết 2 đến 3 dòng vào `decomposition.md`: việc gì khiến bạn nhận ra lệnh cần cụ thể, và một loại lệnh mơ hồ bạn thường vô tình dùng là gì.

### Bài 4 ★: Viết thuật toán có điều kiện

Chọn 1 việc từ Bài 1. Viết lại thuật toán thêm ít nhất 2 bước có điều kiện "NẾU... THÌ...". Ví dụ thuật toán "đi học đúng giờ" có thể thêm: nếu trời mưa thì mang theo ô, nếu đồng hồ báo 6:45 mà chưa ăn sáng thì ăn nhanh bánh mì thay vì bún, nếu quên sách thì gọi điện cho mẹ nhờ mang tới. Mục đích: tập viết điều kiện, nền tảng của lập trình rẽ nhánh ở chặng 12 (Scratch) và chặng 29 (Python).

### Bài 5 (tùy chọn): Mã giả cho "tìm số lớn nhất trong 4 số"

Viết mã giả (theo mẫu ở phần Kiến thức) cho thuật toán tìm số lớn nhất trong **4 số** a, b, c, d. Đừng xem gợi ý mẫu cho 3 số cho đến khi bạn đã thử 15 phút. Format gợi ý: ghi INPUT và OUTPUT, sau đó là các dòng `largest = a`, `IF b > largest THEN largest = b`, cứ thế cho c và d, kết thúc bằng `RETURN largest`.

### Bài 6 (tùy chọn): Trò chơi tháp Hà Nội với 3 đĩa

Nếu có 3 đĩa kích thước khác nhau (dùng 3 đồng xu kích cỡ khác, hoặc 3 cuốn sách) và 3 cọc, thử giải bài toán tháp Hà Nội 3 đĩa. Quy tắc: đưa 3 đĩa từ cọc A sang cọc C, dùng cọc B làm trung gian, mỗi lần chỉ di chuyển 1 đĩa, không đặt đĩa lớn lên đĩa nhỏ. Ghi lại các bước bạn làm theo format "Bước 1: chuyển đĩa nhỏ từ A sang C", "Bước 2: chuyển đĩa trung từ A sang B", v.v. Thử với 3 đĩa (cần 7 bước). Nếu thấy dễ, thử 4 đĩa (cần 15 bước). Đây là bài toán đệ quy kinh điển, sẽ học phân tích sâu ở chặng 39.

### Bài 7 (tùy chọn): Gỡ lỗi thuật toán "đi siêu thị"

Thuật toán sau có nhiều lỗi tiềm năng, tìm và sửa.

```
Thuật toán đi siêu thị:
1. Lên danh sách cần mua.
2. Ra siêu thị, vào cửa.
3. Bỏ tất cả đồ vào giỏ mà không nhìn giá.
4. Đến quầy tính tiền, thanh toán.
5. Về nhà, cất đồ vào tủ lạnh.
```

Lỗi tiềm năng: thiếu bước so sánh giá và chọn hàng, thiếu bước kiểm tra hạn sử dụng, thiếu bước xử lý khi hết hàng, thiếu bước kiểm tra túi tiền trước khi đi, thiếu bước xếp đồ vào túi mang về. Viết lại thuật toán đầy đủ, gồm ít nhất 1 điều kiện "NẾU... THÌ...".

### Bài 8 (tùy chọn): Trừu tượng hóa, vẽ sơ đồ quy trình

Chọn 1 trong 3 thuật toán bạn viết ở Bài 1, vẽ lại thành **sơ đồ quy trình** (*flowchart*). Hình chữ nhật là bước hành động, hình thoi là điều kiện rẽ nhánh (NẾU... THÌ... / NẾU KHÔNG THÌ...), mũi tên là trật tự thực hiện. Vẽ trên giấy hoặc dùng công cụ online miễn phí như [draw.io](https://draw.io), [mermaid.live](https://mermaid.live). Sơ đồ quy trình là cách giao tiếp thuật toán phổ biến trong tài liệu kỹ thuật, bạn sẽ gặp lại ở mọi chặng sau.

### Bài 9 (tùy chọn): Tìm mẫu hình trong 3 quy trình

So sánh 3 quy trình hằng ngày: đánh răng, rửa mặt, tắm. Tìm các bước giống nhau giữa 3 quy trình, đó là mẫu hình lặp lại. Ví dụ: đều bắt đầu bằng "chuẩn bị nước", đều kết thúc bằng "lau khô". Ghi lại các mẫu hình bạn tìm được. Đây là bước đầu của trừu tượng hóa, sẽ học sâu hơn ở chặng 08.

### Đáp án Bài 2

Thuật toán gốc:

```
1. Đun 500ml nước trong nồi.
2. Thả mì vào nước lạnh ngay.
3. Đợi 5 phút, tắt bếp.
4. Sau đó mới mở gói gia vị bỏ vào.
5. Đổ mì ra tô và thưởng thức.
```

Ba lỗi cần sửa: bước 2 thả mì vào nước lạnh sẽ làm mì nhũn, không săn, sửa thành "đợi nước sôi mới thả mì". Bước 3 đợi 5 phút là quá lâu, mì thường chỉ cần 2 đến 3 phút, sửa thành "đợi 2 đến 3 phút, khuấy nhẹ, nếm thử trước khi tắt bếp". Còn thiếu bước "chuẩn bị tô, đũa" trước khi đổ mì ra, thêm vào đầu. Bản sửa gợi ý:

```
0. Chuẩn bị: nồi, 500ml nước, tô, đũa, gói mì, gói gia vị.
1. Đun 500ml nước trong nồi đến khi sôi. NẾU chưa sôi THÌ đợi thêm.
2. Khi nước sôi, mở gói mì, thả mì vào nồi.
3. Đun thêm 2 đến 3 phút, khuấy nhẹ. NẾU mì đã mềm THÌ tắt bếp.
4. Đổ mì ra tô (đã chuẩn bị ở bước 0).
5. Cho gói gia vị vào tô, trộn đều.
6. Thưởng thức.
```

Lưu ý: có nhiều cách nấu mì đúng, đây chỉ là một. Quan trọng là đủ 4 điều kiện thuật toán: đầu vào rõ, đầu ra rõ, mỗi bước cụ thể, dừng được.

### Câu hỏi tự kiểm tra

Sau khi làm xong bài tập, trả lời 4 câu: tư duy máy tính gồm 4 thành phần nào, nêu 1 ví dụ cho mỗi thành phần. Vì sao máy tính cần lệnh chính xác, không đoán ý. Nêu 4 điều kiện để một dãy bước được gọi là thuật toán. Bạn đang gỡ lỗi 1 thuật toán, quy trình 4 bước là gì. Nếu trả lời được cả 4 câu mà không cần xem tài liệu, bạn đã sẵn sàng sang chặng 03.

## 3. Sản phẩm cuối chặng: "Sách thuật toán"

Mỗi chặng kết thúc bằng một sản phẩm đưa vào portfolio. Chặng 02 yêu cầu tạo tệp `portfolio-ai/phan-1/chặng-02-sach-thuat-toan/README.md` gồm 3 thuật toán bạn tự viết.

Trang 1 là một việc hằng ngày ở nhà (đánh răng, gấp chăn, tưới cây), 5 đến 7 bước, đúng trật tự, mỗi bước có động từ cụ thể. Trang 2 là một việc phức tạp hơn (lập kế hoạch tuần, đi siêu thị, dọn nhà), 6 đến 10 bước kèm ít nhất 2 bước điều kiện "NẾU... THÌ...". Trang 3 là một việc bạn thực sự làm theo thuật toán của mình (nấu 1 món đơn giản, gấp máy bay giấy, lắp đồ chơi), 6 đến 10 bước, đã thực sự làm theo, kèm ghi chú ít nhất 1 chỗ bạn phải sửa (gỡ lỗi).

Điểm nhấn trang 3: bạn phải **thực sự chạy thử** thuật toán của chính mình, như chạy thử chương trình, và ghi chú lại chỗ cần sửa. Đây là vòng đời "viết, chạy, gỡ lỗi" trong thực tế. Nếu bạn ghi sai số rồi sửa, tuyệt vời, đó là gỡ lỗi dữ liệu, đừng sửa cho "báo cáo đẹp". Sản phẩm mục đích là sự thật, không phải thẩm mỹ.

Format gợi ý: viết tiêu đề "Sách thuật toán của tôi", rồi 3 mục con tương ứng 3 thuật toán. Mỗi mục ghi rõ tên việc, các bước theo trật tự, và (riêng thuật toán 3) phần "Lỗi phát hiện khi chạy thử" kèm "Bản sửa" và "Bài học rút ra" 1 đến 2 dòng. Lưu tệp vào portfolio. Đây là artifact thứ 2 của bạn trong hành trình 170 chặng.

## 4. Tự đánh giá và kết nối về sau

Checklist cuối chặng: tôi hiểu 4 thành phần của tư duy máy tính (phân rã, nhận dạng mẫu hình, trừu tượng hóa, thuật toán). Tôi có thể giải thích thuật toán là gì kèm 4 điều kiện. Tôi hiểu vì sao máy cần lệnh chính xác, không đoán ý. Tôi đã làm xong Bài 1, 2, 3, 4 (có sao). Tôi đã hoàn thành "Sách thuật toán" và lưu vào portfolio. Tôi đã thực sự "chạy thử" thuật toán trang 3 và ghi chú lỗi. Tôi đã ghi 1 mục vào `learning-journal.md` cho chặng này. Tôi đã trả lời được câu hỏi "Kết nối về sau" ở cuối chặng.

Nếu 8 trên 8 ô được đánh dấu, chúc mừng, bạn đã hoàn thành chặng 02, sang [chặng 03](../giai-doan-03-du-lieu-va-thong-tin/README.md). Nếu có ô chưa đánh dấu, đừng sang chặng sau, trở lại phần tương ứng.

### Thuật ngữ cần nhớ

Hai mươi thuật ngữ của chặng 02 sẽ xuất hiện lại nhiều lần. **Tư duy máy tính** (*Computational Thinking*, CT) là tư duy để giải quyết vấn đề theo cách máy có thể thực hiện. **Phân rã** (*decomposition*) là chia việc lớn thành các phần nhỏ. **Mẫu hình** (*pattern*) là quy luật lặp lại trong dữ liệu hoặc vấn đề. **Trừu tượng hóa** (*abstraction*) là lọc thông tin quan trọng, bỏ chi tiết thừa. **Thuật toán** (*algorithm*) là dãy bước rõ ràng, đúng trật tự, để giải quyết 1 việc. **Lệnh** (*command* hay *instruction*) là chỉ dẫn 1 hành động cụ thể. **Trật tự** (*sequence*) là thứ tự thực hiện các lệnh, đổi trật tự là đổi kết quả. **Điều kiện** (*condition*) là bước chỉ thực hiện khi thoả "NẾU...". **Câu điều kiện** (*conditional statement*) là cấu trúc NẾU... THÌ... NẾU KHÔNG THÌ.... **Gỡ lỗi** (*debugging* hay *debug*) là tìm và sửa lỗi trong thuật toán hoặc chương trình. **Lỗi** (*bug*) là sai trong thuật toán hoặc code khiến kết quả sai. **Triệu chứng** (*symptom*) là dấu hiệu bên ngoài cho thấy có lỗi. **Nguyên nhân gốc** (*root cause*) là nguyên nhân sâu xa gây ra triệu chứng. **Mã giả** (*pseudocode*) là văn bản gần ngôn ngữ người, có cấu trúc gần ngôn ngữ máy. **Sơ đồ quy trình** (*flowchart*) là sơ đồ hình ảnh của thuật toán. **Đầu vào** (*input*) là dữ liệu đi vào thuật toán. **Đầu ra** (*output*) là kết quả thuật toán trả về. **Vòng lặp** (*loop*) là bước lặp lại nhiều lần. **Độ phức tạp** (*complexity*) là số bước hoặc thời gian thuật toán cần. **Hằng số** (*constant*) là giá trị không đổi trong thuật toán.

Một câu nói nên nhớ: người giỏi máy tính không phải người trả lời nhanh nhất, mà là người nói rõ từng bước nhất. Lỗi không phải thất bại, lỗi là dữ liệu quý.

### Tài nguyên mở rộng (tùy chọn)

Nếu muốn đi sâu hơn, các tài nguyên sau đều miễn phí hoặc dễ tiếp cận. **CS50's Understanding Technology** của Harvard (miễn phí trên edX) là khóa giới thiệu khoa học máy tính cho người không chuyên. **Computational Thinking for Everyone** của Google là bài giảng ngắn về CT. **CS Unplugged** tại [csunplugged.org](https://csunplugged.org) là tài liệu kinh điển dạy khoa học máy tính không cần máy tính, rất phù hợp với Phần 1.

Sách gợi ý: *Grokking Algorithms* của Aditya Bhargava, mỏng, có hình minh họa, giới thiệu thuật toán cho người mới bắt đầu, khuyến nghị đọc sau chặng 03. *Algorithms to Live By* của Brian Christian và Tom Griffiths là sách phổ thông về thuật toán trong đời sống. *Computational Thinking* của Peter J. Denning và Matti Tedre (2020) là sách chuyên sâu cho người muốn hiểu gốc rễ khái niệm.

Trên YouTube: video *"How to think like a programmer"* dễ hiểu, *"CS50 Week 0: Scratch"* của David Malan giới thiệu tư duy thuật toán qua Scratch. Công cụ vẽ sơ đồ quy trình miễn phí: [mermaid.live](https://mermaid.live) vẽ flowchart bằng text rồi render hình, [draw.io](https://app.diagrams.net) vẽ kéo thả, [Excalidraw](https://excalidraw.com) vẽ tay phong cách.

### Kết nối về sau

Các khái niệm của chặng 02 sẽ xuất hiện lại ở: **thuật toán, điều kiện, vòng lặp** (chặng 09 đến 16, Scratch) bạn viết các khái niệm này bằng khối lệnh. **Lệnh, trật tự, gỡ lỗi** (chặng 25 đến 43, Python) viết bằng văn bản, thông báo lỗi Python là "máy nói chuyện với mình". **Độ phức tạp thuật toán** (chặng 37 và 38) phân tích chính thức bằng ký hiệu O(). **Đệ quy** (chặng 39) dạng đặc biệt của thuật toán, tháp Hà Nội là ví dụ kinh điển. **Mã giả** (chặng 35 và 101) viết mã giả trước khi code trở thành thói quen. **Sơ đồ quy trình** (chặng 102 và 141) vẽ pipeline ML bằng flowchart. **Gỡ lỗi ML** (chặng 105, 126, 144) debug không phải code bug, mà là mô hình không học đúng.

Không cần học thuộc ngay, cứ gặp lại là nhớ thêm. Lặp xoáy ốc. Cuối cùng, mở tệp `learning-journal.md` và thêm mục cho chặng 02, gồm: hôm nay tôi học được gì (4 đến 5 ý chính), khó khăn lớn nhất, cách vượt qua, sản phẩm đã làm (đường dẫn), câu hỏi mở cho chặng sau, và checklist 6 ô đánh dấu. Nhật ký này là tài sản quý nhất của bạn sau 170 chặng.
