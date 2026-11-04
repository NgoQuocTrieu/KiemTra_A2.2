# AI_LOG

- **Công cụ:** Copilot.
- **Hiện tượng ban đầu:** Trang GitHub Pages mở được nhưng CSS được yêu cầu ở `/css/style.css` trong khi `style.css` ở thư mục gốc. URL cũ trả HTTP 404; URL `/style.css` trả HTTP 200.
- **Nhận định trước khi hỏi AI:** Đường dẫn tương đối trong HTML không khớp vị trí thật của tệp CSS. Ngoài ra, trường email có `type="texr"` và tên thuộc tính chuyển màu trong CSS bị gõ sai.
- **Gợi ý AI:** Sửa đường dẫn CSS thành `style.css`, sửa kiểu email thành `email` và sửa `bacground-color` thành `background-color`.
- **Quyết định:** Đối chiếu từng lỗi với tệp và URL trước khi chấp nhận; chỉ áp dụng ba sửa đổi này, không thêm chức năng ngoài phạm vi HTML/CSS.
- **Thay đổi mã:** Các sửa đổi nằm trong [commit sửa lỗi](https://github.com/NgoQuocTrieu/KiemTra_A2.2/commit/2b7b7f583b55c9802e2bfaeb4a3ee20e5daacc2a).
- **Kiểm chứng:** `index.html` và `style.css` trên GitHub Pages trả HTTP 200; đường dẫn CSS cũ trả 404, còn đường dẫn mới `/style.css` trả 200. GitHub ghi nhận deploy thành công từ `main` tại SHA `e45e5fa6c63a9490df54400f88bca48b5aa8edd2` ngày 04/11/2026.
