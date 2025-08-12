Bài làm này tập trung vào việc xây dựng một hệ thống API quản lý sinh viên sử dụng công nghệ FastAPI. Mục tiêu của dự án là tạo ra một API đơn giản, dễ triển khai, cho phép người dùng thực hiện các thao tác cơ bản như thêm mới, cập nhật, tìm kiếm và xóa thông tin sinh viên.
Trong giai đoạn đầu, hệ thống được chạy trên môi trường cục bộ (localhost), giúp người học dễ dàng kiểm thử và hiểu rõ cách hoạt động của từng endpoint. Sau khi hoàn thiện, API có thể được triển khai lên Cloud để phục vụ các ứng dụng client từ xa.

Dự án được xây dựng bằng ngôn ngữ Python 3.x, sử dụng các công nghệ và thư viện sau:

FastAPI: Framework chính để xây dựng RESTful API, hỗ trợ tự động sinh tài liệu và giao diện thử nghiệm.

Uvicorn: Server ASGI dùng để chạy ứng dụng FastAPI.

Pydantic: Dùng để kiểm tra và xác thực dữ liệu đầu vào.

Dictionary (Python): Dữ liệu sinh viên được lưu tạm thời trong bộ nhớ dưới dạng Dictionary, giúp đơn giản hóa quá trình thử nghiệm.

JSON: Định dạng dữ liệu được sử dụng để trao đổi giữa client và server.

Pinggy / Render / Railway (ở giai đoạn nâng cao): Các nền tảng hỗ trợ triển khai API lên Cloud để truy cập từ xa.

Về thuật toán, hệ thống không sử dụng các thuật toán phức tạp mà chủ yếu xử lý theo logic CRUD cơ bản, đảm bảo tính rõ ràng và dễ hiểu cho người học.

Hệ thống gồm hai giao diện chính:

Giao diện nhập liệu sinh viên: Cho phép người dùng nhập thông tin sinh viên như mã số, họ tên, ngày sinh, lớp, email,... và thực hiện các thao tác như thêm mới, chỉnh sửa hoặc xóa. Giao diện được thiết kế đơn giản, dễ sử dụng, phù hợp với mục tiêu thử nghiệm ban đầu.

Giao diện tra cứu sinh viên: Người dùng có thể nhập mã sinh viên để tìm kiếm thông tin tương ứng. Nếu sinh viên tồn tại trong hệ thống, các thông tin sẽ được hiển thị đầy đủ. Nếu không, hệ thống sẽ thông báo không tìm thấy.

Ngoài ra, Swagger UI do FastAPI cung cấp cũng đóng vai trò như một giao diện thử nghiệm, cho phép người dùng gửi các yêu cầu HTTP như POST, GET, PUT, DELETE và xem phản hồi trực tiếp từ API.
