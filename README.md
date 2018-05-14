# Document tạo khóa học cho học viên tại hocexcel.online

## Chuẩn bị:
- API URI: Gửi qua email 
- Username: Gửi qua email
- Access_key: Gửi qua email
## Kết nối

Sử dụng phương thức POST để post dữ liệu lên API Hocexcel Online với các thông tin sau: 
- username (required): Tài khoản đối tác tại Hocexcel Online
- access_key (required): Mã xác thực của tài khoản đối tác tại Hocexcel Online 
- contact_name (required): Tên học viên
- contact_email (required): Email học viên (bạn phải chắc chắn rằng email này chính xác để có thể nhận được mã kích hoạt hóa học từ Hocexcel Online)
- contact_phone (required): Số điện thoại học viên
- contact_address (required): Địa chỉ học viên
- contact_job (option): Nghề nghiệp của học viên
- price_to_pay (required): Số tiền của học viên đã trả cho dịch vụ của bên đối tác

Server sẽ trả về response với kiểu dữ liệu JSON

   `{
	    "success": true,
	    "message": "Register course success"
    }`
        
Sau khi nhận được kết quả response từ Hocexcel API, tùy vào kết quả có thể xử lý tiếp theo tại hệ thống của đối tác.
