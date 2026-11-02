# Naotube — Nền Tảng Video Đen & Cam Tùy Biến

Nền tảng chia sẻ và xem video YouTube mang phong cách Dark Mode với tông màu Cam & Đen hiện đại, tích hợp trực tiếp **YouTube Data API v3** và **YouTube IFrame Player API**.

---

## 🚀 Tính Năng Chính
- **Đề xuất video chuẩn YouTube**: Xem video phổ biến, thịnh hành và theo từng danh mục (*Âm nhạc, Gaming, Công nghệ, Lập trình, Khoa học, Tin tức, v.v.*).
- **Trang Chi Tiết Kênh (Channel Page)**: Xem banner kênh, avatar, số lượng người đăng ký, danh sách video tải lên (sắp xếp mới nhất / phổ biến nhất) và thông tin giới thiệu.
- **Tìm kiếm thông minh**: Tìm kiếm đồng thời video và kênh YouTube, hiển thị thẻ kênh nổi bật đầu danh sách tìm kiếm.
- **Trình phát video cao cấp**:
  - Chế độ Rạp Chiếu Phim (Theater Mode).
  - Thu nhỏ Mini-Player (Picture-in-Picture) nổi ở góc dưới để vừa lướt vừa xem.
  - Tóm tắt nội dung video bằng AI (AI Video Summary) kèm mốc thời gian click nhảy đến giây tương ứng.
  - Ghi chú mốc thời gian cá nhân (Timestamp Bookmarks) lưu vào trình duyệt và xuất ra file `.txt`.
- **Hệ thống tài khoản đăng nhập**:
  - Tài khoản: `qnnaot`
  - Mật khẩu: `123123`
  - Tích hợp **Khóa Bảo Vệ Riêng Tư (Vercel / GitHub Pages Private Lock)** trong phần Cài đặt.

---

## 📦 Hướng Dẫn Push Lên GitHub & Chạy Trên GitHub Pages (`github.io`)

Dự án đã được cấu hình sẵn file workflow `.github/workflows/deploy.yml` và đường dẫn tương đối `base: './'` trong `vite.config.ts`, tự động tương thích 100% với GitHub Pages mà không bị lỗi đường dẫn hay màn hình trắng.

### Bước 1: Tạo Repository Trên GitHub
1. Truy cập [github.com/new](https://github.com/new).
2. Đặt tên Repository (ví dụ: `naotube`).
3. Chọn chế độ **Public** (để dùng GitHub Pages miễn phí).
4. Nhấn **Create repository** (không cần tick chọn Readme hay .gitignore vì dự án đã có sẵn).

### Bước 2: Liên kết và Push Code Lên GitHub
Mở terminal trong thư mục dự án và chạy các lệnh sau:

```bash
# 1. Thêm link repository GitHub của bạn (thay thế USERNAME bằng tên GitHub của bạn)
git remote add origin https://github.com/USERNAME/naotube.git

# 2. Đặt tên nhánh chính là main
git branch -M main

# 3. Đẩy toàn bộ mã nguồn lên GitHub
git push -u origin main
```

### Bước 3: Kích Hoạt GitHub Pages Trên GitHub
1. Truy cập vào Repository trên GitHub của bạn.
2. Nhấn vào tab **Settings** (Cài đặt) ở thanh trên cùng.
3. Ở menu bên trái, chọn mục **Pages**.
4. Tại phần **Build and deployment** -> **Source**: chọn **GitHub Actions**.
5. Nhấn chuyển sang tab **Actions** trên Repository của bạn: bạn sẽ thấy quy trình `Deploy Naotube to GitHub Pages` đang tự động chạy và xuất bản website!
6. Khi hoàn tất (biểu tượng tích xanh ✅), trang web của bạn sẽ hoạt động tại:
   `https://USERNAME.github.io/naotube/`

---

## ⚡ Triển Khai Lên Vercel (Tùy Chọn)
1. Truy cập [vercel.com](https://vercel.com) và đăng nhập bằng tài khoản GitHub.
2. Chọn **Add New...** -> **Project** -> Chọn repository `naotube`.
3. Nhấn **Deploy** (Vercel tự động nhận diện Vite và cài đặt trong 30 giây).
4. Trang web sẽ chạy tại `https://naotube-xxx.vercel.app`.

---

## 🛠️ Chạy Thử Trên Máy Local
```bash
# Cài đặt thư viện
npm install

# Chạy server phát triển
npm run dev

# Đóng gói sản phẩm
npm run build
```
