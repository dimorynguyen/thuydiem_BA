# Portfolio Nguyen Thi Thuy Diem — hướng dẫn Vercel

## Đưa website lên Vercel qua GitHub
1. Giải nén file ZIP này.
2. Tạo repository trên GitHub (có thể chọn Private).
3. Chọn Add file → Upload files, tải thư mục dist, vercel.json và README.md lên repository, rồi Commit changes. Không tải nguyên file ZIP lên GitHub.
4. Đăng nhập https://vercel.com bằng GitHub. Chọn Add New → Project, chọn Import repository vừa tạo.
5. Chọn Framework Preset: Other; Root Directory: thư mục gốc chứa vercel.json; Build Command: bật Override và để trống; Output Directory: dist. Không cần biến môi trường.
6. Chọn Deploy. Sau khi hoàn tất, mở URL Vercel trả về.
7. Kiểm tra cả 4 trang và nút VI/EN. Tải lại trực tiếp /education-skills, /projects, /personal-projects.

## Cập nhật sau này
Chỉnh file trong GitHub và commit; Vercel tự triển khai lại từ repository đã liên kết.
- dist/assets/content.js: nội dung VI/EN. File có các cập nhật ở cuối; sửa giá trị cuối cùng đang ghi đè.
- dist/assets/redesign.js: bố cục hiện tại, popup và một số nhãn giao diện.
- dist/assets/redesign.css: giao diện hiện tại.
- dist/assets/app.js: điều hướng, sự kiện và các thành phần chung.
- dist/assets/: ảnh và tài nguyên.
- dist/index.html và các thư mục trang: điểm vào cho từng đường dẫn.
Đây là website HTML/CSS/JavaScript tĩnh, không cần npm install hoặc build. Source trong dist là source có thể chỉnh sửa trực tiếp.

## Xem thử trên máy
Nếu có Python: mở terminal trong thư mục đã giải nén, chạy python -m http.server 8080 --directory dist, rồi mở http://localhost:8080. Không mở index.html bằng cách nhấp đúp vì đường dẫn tài nguyên bắt đầu bằng /.

## Nội dung còn chờ
- Tiếng Anh mô tả Hành trình dự án và nhóm người dùng ROOTMAP.
- CV và link LinkedIn cá nhân (link hiện tại /feed/ là bảng tin chung).

## Tài liệu chính thức
https://vercel.com/docs/builds/configure-a-build
https://vercel.com/docs/deployments

Lưu ý: source không bao gồm thông tin đăng nhập hay cấu hình riêng của nền tảng preview. Kiểm tra quyền truy cập website sau khi deploy để người xem portfolio có thể mở link.
