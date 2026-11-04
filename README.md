# Portfolio V7

Portfolio cá nhân làm bằng HTML và CSS, tiếp tục từ Lab 5.

- **Tác giả:** Ngo Quoc Trieu
- **Repository:** https://github.com/NgoQuocTrieu/KiemTra_A2.2
- **GitHub Pages:** https://ngoquoctrieu.github.io/KiemTra_A2.2/
- **Công nghệ:** HTML5, CSS3; không dùng thư viện ngoài.

## Chạy và kiểm tra

Mở `index.html` trong trình duyệt. Mã nguồn chính gồm `index.html` và `style.css`, đặt cùng thư mục; GitHub Pages xuất bản từ nhánh `main`, thư mục gốc.

Các khu vực có thể thử: điều hướng giữa các mục, liên kết dự án, trạng thái hover/focus, bố cục thẻ ở các kích thước màn hình và kiểm tra trường bắt buộc của form. Form chỉ mô phỏng; không gửi email hay lưu thông tin. Không nhập dữ liệu thật.

## Hồ sơ

- [AI_LOG.md](./AI_LOG.md): hiện tượng, nhận định, quyết định và kiểm tra.
- [RELEASE_NOTES.md](./RELEASE_NOTES.md): thay đổi, commit và hạn chế.

## Kiểm chứng local – repo – URL

Kiểm tra ngày 04/11/2026. SHA mã nguồn được đối chiếu là `e45e5fa6c63a9490df54400f88bca48b5aa8edd2`; tại thời điểm kiểm tra, `main` local khớp `origin/main` . GitHub Pages báo deploy thành công cho cùng SHA.

| Hạng mục | Kết quả | Căn cứ |
|---|---|---|
| Trang chính | HTTP 200; tiêu đề “Lab 5 · Portfolio thực hành”, lời chào “Triệu” | [URL Pages](https://ngoquoctrieu.github.io/KiemTra_A2.2/) |
| CSS | `/style.css` HTTP 200; đây là đường dẫn trong HTML | [Tệp CSS đã xuất bản](https://ngoquoctrieu.github.io/KiemTra_A2.2/style.css) |
| Đường dẫn CSS cũ | `/css/style.css` HTTP 404; nguyên nhân là CSS nằm ở thư mục gốc, không phải thư mục `css` | [Commit sửa đường dẫn](https://github.com/NgoQuocTrieu/KiemTra_A2.2/commit/2b7b7f583b55c9802e2bfaeb4a3ee20e5daacc2a) |
| Phiên bản deploy | Thành công từ `main`, SHA `e45e5fa6c63a9490df54400f88bca48b5aa8edd2` | [Lịch sử commit](https://github.com/NgoQuocTrieu/KiemTra_A2.2/commits/main/) |
| Kiểm tra local/repo | `main` khớp `origin/main`; không có thay đổi local tại thời điểm kiểm tra | Trạng thái Git ngày 04/11/2026 |

### Cải tiến giao diện và lý do

Trước khi sửa, HTML yêu cầu `/css/style.css` nhưng đường dẫn đó trả HTTP 404; vì vậy trình duyệt không tải được CSS. Sau khi đổi liên kết thành `style.css`, tệp CSS trên Pages trả HTTP 200. CSS hiện có Grid một cột ở màn hình nhỏ, chuyển thành hai và ba cột ở màn hình rộng; liên kết và form có chỉ báo `focus-visible` để hỗ trợ thao tác bàn phím. Có thể đối chiếu mã ở [commit sửa](https://github.com/NgoQuocTrieu/KiemTra_A2.2/commit/2b7b7f583b55c9802e2bfaeb4a3ee20e5daacc2a) và bản đang chạy ở [GitHub Pages](https://ngoquoctrieu.github.io/KiemTra_A2.2/).

## Demo trực tiếp

Mở URL Pages, chỉ đường dẫn CSS và SHA ở phần kiểm chứng; thu nhỏ cửa sổ để cho thấy bố cục co giãn; dùng phím Tab để xem focus; cuối cùng thử để trống trường bắt buộc trong form. Form là mô phỏng, không có máy chủ nhận dữ liệu.

