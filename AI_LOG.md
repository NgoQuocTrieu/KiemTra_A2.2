# AI_LOG

- **Công cụ:** Copilot.
- **Hiện tượng:** Trang Pages tải được nội dung nhưng yêu cầu `/css/style.css` bị 404; tệp `style.css` nằm ở thư mục gốc. Trong mã còn có `type="texr"` và gõ sai `bacground-color`.
- **Nhận định và quyết định:** Đối chiếu HTML/CSS và URL trước khi sửa. Chỉ sửa ba lỗi có căn cứ: đường dẫn CSS, kiểu email và tên thuộc tính chuyển màu.
- **Kiểm tra:** Trước khi sửa, `/css/style.css` trả 404 và `/style.css` có nội dung. Mã sau sửa mới được kiểm tra tĩnh tại local; chưa push nên chưa xác nhận bản Pages mới.
- **Phần tự làm:** Đọc mã, chọn các lỗi cần sửa và sẽ kiểm tra lại sau khi triển khai.
