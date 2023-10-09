Multiple ID multiple databases multiple server

Mục đích cho các hệ thống lớn giảm tải phân bố, tăng tốc truy cập…..
DatabaseRouter: chịu trách nhiệm định tuyến đăng nhập, định tuyến kết nối, định tuyết backup.... 1 - >  n database Data.
(bạn có thể set 1000 user chuyển hướng database khác)

Server : List conection database
NumberUser : số user cộng 1 khi đăng ký thành công trên 1 databasenode <= 1000;
User: Userid và Parenid (Multiple ID)  quan hệ 1:1 với bảng Roles, Options, Profiles
NodeDatabase là thông tin Server (json)
Profiles : chứa thông tin của user có thể thêm trường.
Roles: chứa phân quyền trường theo phần mềm yêu cầu.
Options : chưa thông tin cấu hình của phần mềm.
DatabaseNode1
DatabaseNode2
………………
DatabaseNode: giống nhau cấu trúc của phần mềm.
Hoạt động:
Khi đăng nhập nhập xong sẽ load thông tin 1 user 1 Profiles  1 Roles Options  lên session con lại kết nối bình thường đến các DatabaseNode trong NodeDatabase  của bản User
https://raw.githubusercontent.com/Smart-Kit/SmartSql-Docs/master/docs/imgs/SmartSql-features.png
