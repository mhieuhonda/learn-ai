# 06. Học máy ở mức lý thuyết

Bài này trình bày các hình thức học và nguyên lý khái quát hóa làm nền chung cho toàn bộ AI hiện nay. Thời lượng đọc khoảng 30 phút. Nội dung thuần lý thuyết, không yêu cầu viết mã hay chạy mô hình.

## 1. Các hình thức học và khái niệm mô hình

Học máy (machine learning) là hướng nghiên cứu giúp máy tự rút quy luật từ dữ liệu thay vì tuân thủ toàn bộ quy tắc viết tay. Bốn hình thức chuẩn là học có giám sát, học không giám sát, học tự giám sát và học tăng cường.

1. Học có giám sát (supervised learning) học từ ví dụ đã có đáp án. Đầu vào là ảnh kèm nhãn mèo hay chó, câu kèm nhãn khen hay chê. Nhiệm vụ là đoán đúng nhãn cho ví dụ mới.
2. Học không giám sát (unsupervised learning) học từ dữ liệu chưa có đáp án. Nhiệm vụ là tự nhóm các điểm giống nhau lại gần nhau để phát hiện cấu trúc ẩn như phân khúc khách hàng.
3. Học tự giám sát (self supervised learning) tự tạo đáp án từ chính dữ liệu bằng cách che một phần và đoán phần bị che. Đây là nguyên lý nền của nhiều mô hình ngôn ngữ và thị giác quy mô lớn.
4. Học tăng cường (reinforcement learning) học qua thử và nhận phản hồi dưới dạng phần thưởng. Tác tử (agent) chọn hành động trong môi trường, nhận điểm thưởng hay phạt, dần điều chỉnh chiến lược để tối đa tổng thưởng về lâu dài.

Mô hình (model) là nơi chứa quy luật đã học dưới dạng tham số có thể điều chỉnh. Hàm mất mát (loss function) đo mức sai lệch giữa đoán nhận và đáp án mong muốn. Quá trình học là điều chỉnh tham số để giảm sai lệch trên dữ liệu đã thấy, đồng thời giữ khả năng đoán đúng cho dữ liệu mới.

## 2. Vì sao học tốt trên dữ liệu cũ chưa đủ

Khái quát hóa (generalization) là khả năng đoán đúng cho tình huống mới chưa từng gặp. Đây là thước đo duy nhất có ý nghĩa thực tế. Hai thất bại điển hình là thiếu khớp và quá khớp. Thiếu khớp (underfitting) nghĩa là mô hình quá đơn giản nên không nắm được quy luật chính, sai cả trên dữ liệu cũ lẫn dữ liệu mới. Quá khớp (overfitting) nghĩa là mô hình nhớ cả nhiễu và chi tiết ngẫu nhiên nên đúng cao trên dữ liệu cũ nhưng sai nhiều trên dữ liệu mới.

Ba thực hành khái niệm để đánh giá trung thực là tách tập huấn luyện, tập kiểm định và tập kiểm tra, theo dõi đồng thời sai số trên cả ba tập, và ưu tiên mô hình đơn giản vừa đủ có khả năng giải thích. Cặp khái niệm sai lệch và phương sai tóm tắt đánh đổi cốt lõi. Mô hình quá đơn giản thì sai lệch cao, mô hình quá phức tạp thì phương sai cao. Điểm tốt nằm ở sự cân bằng phù hợp với lượng dữ liệu và độ phức tạp của nhiệm vụ.

## 3. Tóm lược và chuyển tiếp

Học máy gồm bốn hình thức là có giám sát, không giám sát, tự giám sát và tăng cường, vận hành trên mô hình chứa tham số được điều chỉnh theo hàm mất mát. Giá trị thực tế nằm ở khái quát hóa cho dữ liệu mới, với hai rủi ro chính là thiếu khớp và quá khớp cùng nguyên tắc đánh giá trên tập dữ liệu tách biệt.

Để tự kiểm tra, hãy phân loại một ứng dụng quen thuộc vào một trong bốn hình thức học và giải thích vì sao. Hãy nêu một dấu hiệu cho thấy hệ thống có thể đang quá khớp với dữ liệu cũ.

Bài tiếp theo trình bày học sâu ở mức lý thuyết gồm nơ ron nhân tạo, các kiến trúc chính và ý tưởng biểu diễn nhiều lớp.

<p align="center">
  <a href="../05_du_lieu_khai_niem/README.md">Về bài 05</a> | <a href="../README.md">Về mục lục</a>
</p>
