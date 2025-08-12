Bài làm này tập trung vào việc xây dựng một hệ thống API quản lý sinh viên đơn giản, sử dụng công nghệ FastAPI – một framework hiện đại và hiệu quả dành cho việc phát triển các ứng dụng web và dịch vụ RESTful. Mục tiêu chính của dự án là giúp người học nắm vững cách thiết kế, triển khai và thử nghiệm một API có khả năng xử lý các thao tác cơ bản như thêm mới, cập nhật, tìm kiếm và xóa thông tin sinh viên.
Trong giai đoạn đầu, hệ thống được triển khai và chạy trên môi trường cục bộ (localhost), giúp việc phát triển và kiểm thử diễn ra thuận tiện mà không cần đến hạ tầng Cloud. Người dùng có thể tương tác với API thông qua các công cụ như Postman hoặc trực tiếp từ trình duyệt thông qua giao diện Swagger UI do FastAPI tự động tạo ra.

Công nghệ và ngôn ngữ sử dụng:
Dự án được xây dựng hoàn toàn bằng ngôn ngữ Python 3.x, kết hợp với các công nghệ sau:
FastAPI: Framework chính để xây dựng API, hỗ trợ tự động sinh tài liệu và giao diện thử nghiệm thông qua Swagger UI.
Uvicorn: Server ASGI dùng để chạy ứng dụng FastAPI.
Pydantic: Thư viện hỗ trợ kiểm tra và xác thực dữ liệu đầu vào.
Dictionary (Python): Dữ liệu sinh viên được lưu tạm thời trong bộ nhớ dưới dạng Dictionary, giúp đơn giản hóa quá trình thử nghiệm.
JSON: Định dạng dữ liệu được sử dụng để trao đổi giữa client và server.
Trong giai đoạn nâng cao, hệ thống có thể được triển khai lên các nền tảng Cloud như Pinggy, Render hoặc Railway, giúp các ứng dụng client có thể truy cập API từ xa mà không cần dùng chung mạng nội bộ.
