Lịch sử AI_prompt:
Tôi đang bắt đầu tìm hiểu về Git và HTML. Bạn hãy đóng vai trò như một giảng viên. Hãy giải thích lý do chuẩn W3C yêu cầu sử dụng danh sách <ul>/<li> cho menu thay vì chỉ viết các thẻ <a> nằm ngang cho tôi hiểu.
Tại sao các trang web lớn lại bọc thẻ <a> bên trong thẻ <li> để làm menu? Làm thế có lợi ích gì cho người khiếm thị dùng Screen Reader không?
Bối cảnh dự án:

Công ty đang chạy một chiến dịch Marketing lớn, trang chủ (index.html) hiện tại đang hoạt động ổn định và đón hàng ngàn lượt truy cập (nằm trên nhánh main). Tuy nhiên, Giám đốc yêu cầu phải bổ sung gấp một Menu Điều Hướng (Navigation Bar) để khách hàng dễ tìm kiếm sản phẩm. Nếu bạn code thẳng lên nhánh main và xảy ra lỗi hỏng giao diện, toàn bộ chiến dịch sẽ đổ vỡ. Yêu cầu bắt buộc: Phải tạo một môi trường an toàn (nhánh mới) để xây dựng Menu bằng cấu trúc danh sách <ul>, sau khi test kỹ lưỡng mới được "ghép" (Merge) vào trang chính.
Tôi có bài toán trên để luyện tập Git&HTML, bạn hãy xem tôi thêm nav như này đã hợp lý chưa, có cần chỉnh sửa đoạn nào không?