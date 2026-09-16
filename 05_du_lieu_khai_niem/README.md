# 05. Dữ liệu ở mức khái niệm

Bài này trình bày bản chất, phân loại, chất lượng và vòng đời của dữ liệu dưới góc nhìn khái niệm. Thời lượng đọc khoảng 25 phút. Nội dung thuần lý thuyết, không yêu cầu thu thập hay xử lý trên máy.

## 1. Dữ liệu là gì và có những loại nào

Dữ liệu (data) là các quan sát đời sống đã được ghi lại dưới dạng máy có thể đọc. Ảnh chụp, đoạn chat, bản ghi giọng nói, đơn hàng, nhật ký hệ thống đều là dữ liệu. Máy không trực tiếp sống trong đời sống, máy chỉ tiếp cận đời sống thông qua lớp ghi nhận này nên mọi hiểu biết của máy đều bị giới hạn bởi chất lượng ghi nhận.

Ba phân loại nền tảng cần nắm là dữ liệu có cấu trúc, dữ liệu phi cấu trúc và dữ liệu gán nhãn. Dữ liệu có cấu trúc nằm trong bảng biểu rõ ràng như đơn hàng gồm mã, số lượng và giá. Dữ liệu phi cấu trúc là nội dung tự do như ảnh, âm thanh và văn bản dài. Dữ liệu gán nhãn là dữ liệu đã có đáp án kèm theo như ảnh đã ghi rõ đây là mèo, câu đã ghi rõ ý khen hay chê. Nhãn là cầu nối giữa ví dụ và quy luật cần học.

Vòng đời khái niệm của dữ liệu gồm thu thập, làm sạch, lưu trữ, sử dụng để học và giám sát sau triển khai. Thu thập quyết định phạm vi thế giới mà máy được thấy. Làm sạch quyết định mức nhiễu còn lại. Lưu trữ liên quan tới quyền riêng tư và thời hạn giữ lại. Sử dụng để học quyết định quy luật hình thành. Giám sát sau triển khai phát hiện khi thế giới thay đổi khiến dữ liệu cũ không còn đại diện.

## 2. Vì sao dữ liệu quyết định mọi kết quả

Chất lượng suy luận không bao giờ vượt quá chất lượng dữ liệu ở mức khái niệm. Bốn sai lệch phổ biến là thiếu đại diện, lệch đo lường, lệch lịch sử và lệch phản hồi. Thiếu đại diện nghĩa là một nhóm đối tượng vắng mặt trong dữ liệu nên máy đoán kém cho nhóm đó. Lệch đo lường nghĩa là cách ghi nhận đã méo ngay từ đầu như ảnh luôn chụp trong điều kiện đẹp. Lệch lịch sử nghĩa là dữ liệu mang định kiến xã hội có sẵn và máy học lại nguyên định kiến đó. Lệch phản hồi nghĩa là kết quả của máy ảnh hưởng ngược tới dữ liệu mới tạo vòng xoáy khép kín.

Nguồn gốc và sự đồng thuận là hai câu hỏi pháp lý và đạo đức đi kèm mọi tập dữ liệu. Dữ liệu của ai, thu trong bối cảnh nào, có được cho phép dùng cho mục đích học hay không, thời hạn lưu giữ bao lâu. Đây là lý do các tổ chức nghiêm túc đều yêu cầu truy vết nguồn gốc và đánh giá tác động trước khi huấn luyện.

## 3. Tóm lược và chuyển tiếp

Dữ liệu là thế giới qua lăng kính ghi nhận, gồm ba dạng chính là có cấu trúc, phi cấu trúc và gán nhãn, vận hành theo vòng đời từ thu thập tới giám sát. Mọi sai lệch trong dữ liệu đều lan truyền thành sai lệch trong kết quả theo bốn cơ chế phổ biến. Nắm được bản chất này giúp bạn đọc mọi tuyên bố về độ chính xác với con mắt kiểm chứng về nguồn dữ liệu.

Để tự kiểm tra, hãy lấy một ứng dụng quen thuộc và liệt kê dữ liệu đầu vào của nó thuộc loại nào, vòng đời ra sao, rủi ro lệch nào dễ gặp nhất.

Bài tiếp theo trình bày các nguyên lý học máy gồm các hình thức học, khái niệm mô hình và hiện tượng khái quát hóa, là nền chung cho toàn bộ AI hiện nay.

<p align="center">
  <a href="../04_toan_y_tuong/README.md">Về bài 04</a> | <a href="../README.md">Về mục lục</a> | <a href="../06_hoc_may_ly_thuyet/README.md">Sang bài 06</a>
</p>
