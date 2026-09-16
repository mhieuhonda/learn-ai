# 01. AI là gì và AI làm gì

Bài này trình bày định nghĩa nền tảng và phạm vi ứng dụng của Trí tuệ Nhân tạo ở mức khái niệm. Thời lượng đọc khoảng 25 phút. Nội dung thuần lý thuyết, không yêu cầu cài đặt hay thực hành.

## 1. AI là gì

Trí tuệ nhân tạo (artificial intelligence) là lĩnh vực nghiên cứu và hệ thống công nghệ giúp máy thực hiện các nhiệm vụ vốn cần năng lực trí tuệ của con người như nhận biết hình ảnh, hiểu ngôn ngữ, dự đoán số liệu, hỗ trợ quyết định và tạo nội dung mới ở mức dùng được.

Điểm phân biệt với tự động hóa truyền thống (automation) nằm ở phương thức hình thành năng lực. Tự động hóa truyền thống vận hành theo quy tắc do con người viết sẵn, gặp tình huống ngoài quy tắc thì dừng hoặc báo lỗi. AI hình thành năng lực bằng cách học quy luật từ dữ liệu, vì vậy vẫn đưa ra kết quả hợp lý cho tình huống chưa từng gặp nguyên văn. Ví dụ đối chiếu là máy chấm vân tay theo ngưỡng cố định và hệ nhận diện khuôn mặt trong điều kiện thiếu sáng. Hệ thứ nhất là tự động hóa, hệ thứ hai là AI vì đã khái quát từ hàng triệu khuôn mặt khác nhau.

Ba thành phần cấu thành mọi hệ AI hoàn chỉnh là dữ liệu (data), quy luật trong mô hình (model) và mục tiêu đánh giá (objective). Dữ liệu là các quan sát đã ghi nhận như hình ảnh, văn bản trao đổi, tín hiệu giọng nói, đơn hàng và nhật ký hệ thống. Quy luật là cấu trúc mà máy trích xuất từ dữ liệu như mối liên hệ giữa đặc điểm và nhãn, giữa ngữ cảnh và ý định, giữa chuỗi quá khứ và xu hướng tiếp theo. Mục tiêu đánh giá xác định thế nào là tốt như độ chính xác nhận diện, độ phù hợp của bản dịch, sai số dự báo tồn kho. Ba thành phần này ràng buộc lẫn nhau. Dữ liệu lệch dẫn tới quy luật lệch. Mục tiêu mơ hồ dẫn tới đánh giá sai chất lượng.

Khái niệm phạm vi cần nắm từ đầu là AI hẹp (narrow AI) và AI tổng quát (general AI). Mọi hệ đang vận hành trong thực tế đều là AI hẹp, nghĩa là đạt hiệu quả cao trong phạm vi nhiệm vụ xác định. Hệ phân loại ảnh sản phẩm không suy ra được nhu cầu tồn kho, hệ trả lời tin nhắn không điều khiển được phương tiện. AI tổng quát chỉ tồn tại ở mức giả thuyết nghiên cứu về hệ có thể chuyển giao năng lực linh hoạt như con người. Phân biệt này giúp tránh suy luận sai rằng thành công trong một nhiệm vụ đồng nghĩa với năng lực toàn diện.

## 2. AI làm gì

Mục này mô tả sáu nhóm chức năng chuẩn của AI hiện nay. Các ví dụ lấy theo một cửa hàng bán áo để đảm bảo tính liên tục và dễ đối chiếu, đồng thời phản ánh đúng cách doanh nghiệp triển khai trên quy mô lớn.

1. Thị giác máy. Đầu vào là ảnh và video. Chức năng gồm phân loại sản phẩm, nhận diện lỗi bề mặt, đọc ký tự trên nhãn, đối chiếu ảnh trùng lặp. Giá trị là chuẩn hóa và xử lý hàng nghìn ảnh với chất lượng đồng đều.
2. Xử lý giọng nói. Đầu vào là tín hiệu âm thanh. Chức năng gồm chuyển giọng thành văn bản, định danh người nói, phân loại ý định như đổi kích cỡ hay tra cứu vận chuyển. Giá trị là ghi nhận đầy đủ nội dung tổng đài và rút ngắn thời gian chờ.
3. Xử lý ngôn ngữ. Đầu vào là văn bản như tin nhắn và đánh giá. Chức năng gồm phân loại ý định, phân tích quan điểm khen chê theo khía cạnh, tóm tắt khối lượng lớn phản hồi thành các điểm chính, soạn thảo bản nháp để nhân sự kiểm duyệt. Giá trị là phản hồi nhanh và nắm được trọng tâm của khách hàng.
4. Dự báo định lượng. Đầu vào là chuỗi đơn hàng, lượt xem và yếu tố mùa vụ. Chức năng gồm ước lượng nhu cầu theo kích cỡ, xác suất trả hàng, nhu cầu bổ sung tồn kho. Giá trị là cân đối nhập hàng, giảm tồn đọng và giảm hết hàng giữa chừng.
5. Gợi ý và hỗ trợ quyết định. Đầu vào là lịch sử hành vi của từng khách hàng. Chức năng gồm xếp hạng sản phẩm phù hợp, lựa chọn khung giờ giao nhận, cảnh báo khi sản phẩm quan tâm sắp hết. Giá trị là rút ngắn hành trình tìm kiếm và tăng mức độ phù hợp của đề xuất.
6. Sinh nội dung ở mức bản nháp. Đầu vào là thuộc tính sản phẩm có sẵn. Chức năng gồm soạn mô tả, đề xuất tiêu đề truyền thông, tạo hình minh họa phối đồ. Mọi kết quả đầu ra đều yêu cầu con người kiểm duyệt vì hệ thống có thể diễn đạt trôi chảy nhưng sai chất liệu, sai thông số hoặc sai giá. Giá trị là rút ngắn thời gian khởi tạo thay vì bắt đầu từ trang trắng.

Ở cấp độ tổ chức, sáu nhóm trên vận hành trên dòng dữ liệu liên tục từ cảm biến, tương tác người dùng và nhật ký hệ thống. AI cho phép tự động hóa hỗ trợ khách hàng, cá thể hóa tiếp thị theo phân khúc, phát hiện bất thường trong vận hành và cung cấp phân tích dự báo phục vụ điều hành. Hiệu quả cốt lõi là ra quyết định có cơ sở hơn trên quy mô lớn với chất lượng ổn định.

## 3. Ba ngộ nhận cần làm rõ

1. Đồng nhất kết quả đúng với hiểu biết như con người. Hệ thống có thể dịch chuẩn xác một nội dung mà không có trải nghiệm tương ứng. Vì vậy các nhiệm vụ đòi hỏi thấu cảm và trách nhiệm cần con người quyết định cuối cùng.
2. Cho rằng hệ thống mang tính trung lập tuyệt đối. Do học từ dữ liệu do con người tạo ra, hệ thống kế thừa cả định kiến và sai số trong dữ liệu. Dữ liệu đầu vào lệch thì đầu ra lệch. Mọi kết quả quan trọng đều cần kiểm chứng độc lập.
3. Xem AI như một thực thể đơn nhất. Thực tế mỗi nhóm chức năng tương ứng với một hướng kỹ thuật và một loại dữ liệu riêng. Khi tiếp nhận một thông tin về AI, cần xác định đó là chức năng nào, trên dữ liệu nào và trong phạm vi nào.

## 4. Tóm lược và chuyển tiếp

AI là công nghệ giúp máy thực hiện nhiệm vụ trí tuệ bằng cách học quy luật từ dữ liệu, khác với tự động hóa chỉ tuân thủ quy tắc viết sẵn. Mọi hệ hoàn chỉnh gồm dữ liệu, mô hình chứa quy luật và mục tiêu đánh giá. Phạm vi ứng dụng gồm sáu nhóm là thị giác, giọng nói, ngôn ngữ, dự báo, gợi ý và sinh bản nháp. Mọi thành công hiện tại đều thuộc AI hẹp và cần kiểm chứng của con người trong các quyết định quan trọng.

Để tự kiểm tra, hãy diễn đạt lại định nghĩa AI trong một phút mà không sao chép nguyên văn. Hãy lấy một đơn vị kinh doanh quen thuộc và phân loại hoạt động của họ vào sáu nhóm trên.

Bài tiếp theo trình bày lịch sử hình thành AI từ tư duy dựa trên quy tắc sang học từ dữ liệu, qua đó lý giải vì sao phương pháp hiện nay chiếm ưu thế và vì sao cần thận trọng trước các làn sóng truyền thông.

<p align="center">
  <a href="../README.md">Về mục lục</a> | <a href="../02_lich_su/README.md">Sang bài 02</a>
</p>
