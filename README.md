Trước khi triển khai lên Cloud, hệ thống API được xây dựng và chạy hoàn toàn trên môi trường cục bộ (localhost). Người dùng có thể tương tác với API thông qua các công cụ như Postman, curl, hoặc trực tiếp từ trình duyệt thông qua giao diện Swagger UI do FastAPI tự động tạo ra.

Dữ liệu sinh viên được lưu trữ tạm thời bằng Dictionary trong bộ nhớ của ứng dụng Python, giúp việc thử nghiệm và kiểm tra chức năng trở nên nhanh chóng và đơn giản mà không cần cấu hình cơ sở dữ liệu phức tạp. Việc này đặc biệt hữu ích trong giai đoạn phát triển ban đầu, khi mục tiêu là kiểm tra logic xử lý và đảm bảo các endpoint hoạt động đúng.

Toàn bộ hệ thống có thể được khởi chạy bằng lệnh uvicorn main:app --reload, cho phép cập nhật nhanh khi có thay đổi trong mã nguồn. Người dùng có thể gửi các yêu cầu như tạo mới, cập nhật, tìm kiếm hoặc xóa sinh viên thông qua các phương thức HTTP như POST, PUT, GET, và DELETE.

Việc chạy trên localhost giúp quá trình phát triển diễn ra thuận tiện, không phụ thuộc vào kết nối mạng hay hạ tầng triển khai. Sau khi hoàn thiện các chức năng cơ bản, hệ thống sẽ được đưa lên Cloud để phục vụ các ứng dụng client từ xa.
