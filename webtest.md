# **_Web development test_**

- Hiểu các thành phần cấu tạo nên web application
+ Gồm :
+ Giao diện Client(Chứa giao diện bề ngoài của trang web, giúp người dùng có thể tương tác qua các nút bấm hay thanh cuộn, ô ...) Được cấu thành từ HTML/CSS/JS và những tệp phương tiện,...
+ Server (Nơi xử lý các logic, nhận request từ client, xử lý yêu cầu vào gửi trả lại cho client hiển thị ra ngoài màn hình) 
+ Database: Nơi lưu trữ bản ghi dữ liêu, nơi chứa dữ liệu của toàn bộ hệ thống.

- Hiểu các bước 1 request vận hành như thế nào

+ Client - Server giao tiếp thông qua giao thức HTTTP (Phương thức truyền tải siêu văn bản)

- Bước 1: Client gửi request đến server
- Bước 2: Server xử lý logic.
- Bước 3: Server trả response về cho client

Trong đó :
HTTP Request, HTTP Response có cấu trúc tương tự nhau bao gồm 3 thành phần: 
- Status Line

- Response Header

- Response Body.

Status Line: Bao gồm ba phần:

- HTTP Version: Phiên bản giao thức HTTP;

- Status Code: Mã trạng thái;

- Reason Phrase (còn gọi là Status Text): Mô tả trạng thái.

Mã trạng thái là một số nguyên có 3 chữ số, được cấp bởi máy chủ để phản hồi Request của máy khách gửi đến. Mã trạng thái của HTTP Response được chia thành năm lớp theo tiêu chuẩn, và lớp được xác định bởi chữ số đầu tiên của mã trạng thái:

- 1xx: Thông tin – Request đã được tiếp nhận, quá trình tiếp tục;

- 2xx: Thành công – Request đã được tiếp nhận, hiểu và chấp nhận thành công;

- 3xx: Chuyển hướng – Cần thực hiện thêm hành động để hoàn thành Request;

- 4xx: Lỗi máy khách – Request chứa cú pháp sai hoặc không thể thực hiện được;

- 5xx: Lỗi máy chủ – Máy chủ không thực hiện được một Request rõ ràng hợp lệ.

- Vẽ sơ đồ hoạt động của 1 web application bắt đầu từ khi người dùng gõ 1 địa chỉ web site lên thanh address bar của trình duyệt

![alt text](https://github.com/thanhpm95/git_example/blob/main/diagram.png)

Trong đó:
- VIEW là những gì người dùng thấy.
- CONTROLLER là nơi xử lý logic. 
- SERVICE là nơi chứa những câu lệnh thao tác database
- MODEL là nơi khai báo thực thể, mapping với Database
- DATABASE là nơi chứa bản ghi dữ liệu của hệ thống