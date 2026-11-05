# AI_LOG

- **Công cụ:** Copilot.
- **Hiện tượng ban đầu:** Trang GitHub Pages mở được nhưng CSS được yêu cầu ở `/css/style.css` trong khi `style.css` ở thư mục gốc. URL cũ trả HTTP 404; URL `/style.css` trả HTTP 200.
- **Nhận định trước khi hỏi AI:** Đường dẫn tương đối trong HTML không khớp vị trí thật của tệp CSS. Ngoài ra, trường email có `type="texr"` và tên thuộc tính chuyển màu trong CSS bị gõ sai.
- **Gợi ý AI:** Sửa đường dẫn CSS thành `style.css`, sửa kiểu email thành `email` và sửa `bacground-color` thành `background-color`.
- **Quyết định:** Đối chiếu từng lỗi với tệp và URL trước khi chấp nhận; chỉ áp dụng ba sửa đổi này, không thêm chức năng ngoài phạm vi HTML/CSS.
- **Thay đổi mã:** Các sửa đổi nằm trong [commit sửa lỗi](https://github.com/NgoQuocTrieu/KiemTra_A2.2/commit/2b7b7f583b55c9802e2bfaeb4a3ee20e5daacc2a).
- **Kiểm chứng:** `index.html` và `style.css` trên GitHub Pages trả HTTP 200; đường dẫn CSS cũ trả 404, còn đường dẫn mới `/style.css` trả 200. GitHub ghi nhận deploy thành công từ `main` tại SHA `e45e5fa6c63a9490df54400f88bca48b5aa8edd2` ngày 04/11/2026.

## Cập nhật V8 – 05/11/2026

- **Yêu cầu:** Hoàn thiện portfolio bằng HTML/CSS thuần, thêm các cải tiến giao diện và luồng biểu mẫu, rồi cập nhật tài liệu bàn giao.
- **Gợi ý AI:** Dùng checkbox và CSS để đổi giao diện tối/sáng; dùng kiểm tra `required`, `minlength`, `maxlength` có sẵn của trình duyệt; thêm nút cuộn đầu trang và trang xác nhận biểu mẫu.
- **Quyết định:** Không thêm JavaScript. Biểu mẫu mở `ket-qua.html` trong tab mới; không đặt tên cho các trường để thông tin nhập không bị truyền qua URL. Trang xác nhận thông báo đây là bản demo và có liên kết trở về `index.html`.
- **Thay đổi mã và tài liệu:** Cập nhật `index.html`, `style.css`, thêm `ket-qua.html`, ghi thay đổi vào `CHANGLELOG.md` và viết lại `README.md` theo mẫu Lab 8.
- **Kiểm chứng:** `git diff --check` đạt; kiểm tra mã xác nhận biểu mẫu có nút nộp, mở tab mới, có trường bắt buộc và liên kết quay về; không có JavaScript hoặc dữ liệu biểu mẫu được truyền đi.
- **Hạn chế:** Chưa kiểm thử tương tác trực tiếp trên trình duyệt và chưa xác minh triển khai V8 trên GitHub Pages. Biểu mẫu chỉ mô phỏng, không gửi hoặc lưu thông tin.
