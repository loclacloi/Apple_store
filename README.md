# 🍎 Apple Store Website Clone - Enterprise Edition

<p align="center">
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
</p>

Dự án mô phỏng cửa hàng trực tuyến của Apple với đầy đủ tính năng cho người dùng và quản trị viên. Được tối ưu hóa hiệu suất, hỗ trợ tiếng Việt toàn diện và tích hợp hệ thống báo cáo kinh doanh chuyên sâu.

---

## 📖 Mục lục

- [🚀 Tính năng chính](#-tính-năng-chính)
- [🏗️ Cấu trúc thư mục](#-cấu-trúc-thư-mục)
- [🛠️ Công nghệ sử dụng](#-công-nghệ-sử-dụng)
- [🏁 Hướng dẫn cài đặt](#-hướng-dẫn-cài-đặt)
---

## 🚀 Tính năng chính

### 🛒 Dành cho Khách hàng (Client)

- **Giao diện chuẩn Apple**: Thiết kế tối giản, sang trọng, hiệu ứng mượt mà.
- **Tìm kiếm & So sánh**: Tìm kiếm cực nhanh và so sánh thông số chi tiết (Mac, iPhone, iPad).
- **Giỏ hàng & Yêu thích**: Quản lý mua sắm và lưu sản phẩm quan tâm.
- **Tài khoản**: Xem lịch sử đơn hàng và thông tin cá nhân.

### 📊 Dành cho Quản trị viên (Admin)

- **Bảng điều khiển**: Biểu đồ doanh thu, thống kê theo danh mục và đơn hàng (Pie/Bar Chart).
- **Quản lý toàn diện**: Sản phẩm, Đơn hàng, Người dùng và Banner quảng cáo.
- **Báo cáo chuyên sâu**: Xuất Excel (CSV) và tự động sao lưu vào thư mục `excel/`.

---

## 🏗️ Cấu trúc thư mục

```text
Apple/
├── client/        # Giao diện người dùng (React + Vite)
├── admin/         # Trang quản trị (React + Vite)
├── server/        # API và Logic máy chủ (Node.js + Express)
├── excel/         # Thư mục lưu trữ báo cáo đã xuất
```

---

## 🛠️ Công nghệ sử dụng

- **Frontend**: React.js, Lucide Icons, Recharts, Tailwind/CSS.
- **Backend**: Node.js, Express, MongoDB.
- **Tools**: Vite, pnpm, Git, Docker.

---

## 🏁 Hướng dẫn cài đặt

Dự án này có 2 cách chạy: Bằng Docker (khuyên dùng) hoặc chạy thủ công truyền thống.

### Cách 1: Sử dụng Docker (Khuyên dùng)

Dành cho người mới tải dự án, không cần cài cấu hình MongoDB hay Compass phức tạp.

1. Khởi động Database (MongoDB):
   ```bash
   docker-compose up -d
   ```
   *(Theo dõi Database qua trình duyệt tại `http://localhost:8081` với tài khoản `admin` / `password`)*

2. Khởi tạo dữ liệu mẫu (Seeding) để web có sẵn sản phẩm:
   ```bash
   cd server
   pnpm install
   pnpm run seed
   ```

### Cách 2: Chạy thủ công truyền thống

Dành cho máy đã có sẵn MongoDB hoặc muốn phát triển sâu vào code.

1. **Khởi động Server**:
   ```bash
   cd server
   pnpm install
   pnpm run dev
   ```

2. **Khởi động Client**:
   ```bash
   cd client
   pnpm install
   pnpm dev
   ```

3. **Khởi động Admin**:
   ```bash
   cd admin
   pnpm install
   pnpm dev
   ```




---
*Created with ❤️ by loclacloi team.*