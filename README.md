File Basic_auth.js

- Trước tiên tải express: npm install express
- chạy file basic_auth.js: node basic_auth.js
- Với route "/" và "/public" vẫn sẽ truy cập được mà không cần mật khẩu, kết quả hiển thị "Welcome! Visit first public resource."
<img width="1919" height="990" alt="Screenshot 2025-09-25 185556" src="https://github.com/user-attachments/assets/5335ae65-c901-4c14-af65-6a314ed5d991" />
<img width="1919" height="1079" alt="Screenshot 2025-09-25 185753" src="https://github.com/user-attachments/assets/a7dd019d-d203-4e8b-b2f4-6bd4c4a55428" />
- với route "/secure" nó sẽ yêu cầu gửi thêm Authentication username và password nếu không sẽ hiện thông báo "Authentication required." HTTP Status 401
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/f913ea8b-5c5d-4712-9adc-d6213dadc480" />
- khi ta nhập username và password thì sẽ login thành công và thông báo "You have accessed a protected resource 🎉" HTTP Status 200
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/89b29ee4-f5a6-47e5-a44b-db40e2a027a5" />
-khi ta nhập sai username hoặc password thì sẽ login thất bại và có thông báo "Access denied." HTTP Status 403
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/c4efc764-8653-447a-8a74-dbd2cfd89cbe" />


File Cookie_auth.js

- trước tiên tải mongoose, cookie-parser
- chạy file File Cookie_auth.js
- với phương thức POST Route "/login" chọn vào tab body, chọn raw và nhập
{
  "username": "admin",
  "password": "12345"

} 
- Kết quả trả về là "Logged in!"
- Postman lưu lại cookie
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/f6874e5a-8faf-435d-82b9-ba0b23d44d8f" />

- Server gửi cookie auth_cookie_token về.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/a1bb0f03-b607-4868-8b2a-8e49c39949c4" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/88430976-fe58-4b5a-95ca-36e8c587eab8" />


