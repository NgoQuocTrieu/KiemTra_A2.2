# Portfolio V8

Portfolio cá nhân tĩnh, xây dựng bằng HTML5 và CSS3, tiếp nối v7.

- **Họ tên – MSSV – Lớp:** Ngô Quốc Triệu – 2071020181 – CNTT-20-04
- **Ngành:** Công nghệ thông tin
- **Repository:** https://github.com/NgoQuocTrieu/KiemTra_A2.2
- **Demo:** https://ngoquoctrieu.github.io/KiemTra_A2.2/
- **Công nghệ:** HTML5, CSS3; không dùng JavaScript hay thư viện ngoài.

## Demo

Mở [Portfolio trên GitHub Pages](https://ngoquoctrieu.github.io/KiemTra_A2.2/).

> **Trạng thái phiên bản:** Những thay đổi V8 trong repository local đã commit.
## Cách mở

1. Tải hoặc clone repository về máy.
2. Mở thư mục dự án và mở `index.html` bằng trình duyệt; không cần cài đặt hay build.
3. Thử các mục điều hướng, công tắc giao diện tối/sáng, bố cục ở kích thước màn hình khác nhau và các trường bắt buộc trong form.
4. Bấm **Nộp thông tin** sau khi điền hợp lệ để mở trang xác nhận trong tab mới; dùng nút **Quay về trang ban đầu** để trở lại.

Form chỉ là bản demo tĩnh: trình duyệt kiểm tra dữ liệu, nhưng nội dung không được gửi hoặc lưu. Chỉ dùng dữ liệu giả.

## Chức năng V8

- Bật/tắt giao diện tối/sáng bằng HTML và CSS.
- Hiển thị trạng thái trực quan cho trường hợp lệ/chưa hợp lệ; các trường bắt buộc được kiểm tra bởi trình duyệt.
- Cuộn về đầu trang bằng nút cố định.
- Nộp form để mở trang xác nhận `ket-qua.html` trong tab mới; trang xác nhận có liên kết quay lại.

## Bảng kiểm tra

| Việc đã thử | Kết quả |
|---|---|
| Kiểm tra định dạng thay đổi bằng `git diff --check` | Đạt |
| Kiểm tra form có trường bắt buộc, nút nộp và mở trang xác nhận trong tab mới | Đạt khi kiểm tra mã HTML |
| Kiểm tra trang xác nhận có liên kết về `index.html` | Đạt khi kiểm tra mã HTML |
| Kiểm tra không có JavaScript và dữ liệu form không được truyền đi | Đạt khi kiểm tra mã nguồn; chưa kiểm thử tương tác trên trình duyệt |

## Tệp trong repository

- `index.html`: trang portfolio chính.
- `style.css`: kiểu dáng và bố cục responsive.
- `ket-qua.html`: trang xác nhận demo.
- [CHANGLELOG.md](./CHANGLELOG.md): ghi các thay đổi theo phiên bản. Tên tệp hiện tại là `CHANGLELOG.md`.
- [AI_LOG.md](./docs/AI_LOG.md): nhật ký AI.
- [RELEASE_NOTES.md](./RELEASE_NOTES.md): ghi chú phát hành hiện có.

## Trạng thái bàn giao