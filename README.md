# 🏙️ BCN Startup City – Hệ Thống Quản Lý Dự Án Nội Bộ (Mô Hình Startup)

> **Hệ sinh thái quản lý vòng đời và duy trì dự án công nghệ theo mô hình Startup & Thành phố dành cho Ban Công Nghệ (BCN).**

---

## 📌 1. Bối cảnh & Bài toán đặt ra

Hiện tại, Ban Công Nghệ (BCN) có rất nhiều dự án được các thành viên và team leader phát triển:

- Source code rải rác trên nhiều repository khác nhau.
- Tiến độ, tài liệu và trạng thái hoạt động chưa được đồng bộ hoặc theo dõi tập trung.
- Khi thành viên hoặc leader rời ban, việc bàn giao và tiếp quản dự án gặp nhiều khó khăn.
- Nhiều dự án bị gián đoạn hoặc lãng quên theo thời gian do thiếu cơ chế duy trì động lực.

🎯 **Mục tiêu:** Xây dựng một nền tảng không chỉ đơn thuần là _"gom danh sách link dự án"_, mà là một **hệ thống quản trị hoạt động toàn diện**: từ cấp phép, phân quyền, kiểm duyệt, theo dõi tiến độ đến cơ chế game hóa để duy trì sức sống cho từng dự án.

---

## 💡 2. Concept: "Thành phố BCN & Các Startup"

Hệ thống được thiết kế đồng bộ theo chủ đề **Thành phố BCN**:

- Thay vì chỉ _"Tạo một Project thông thường"_, mỗi dự án được định nghĩa như một **🏢 Startup** đang khởi nghiệp và vận hành trong lòng Thành phố BCN.
- Ban quản trị đóng vai trò như **Thị trưởng / Ban điều hành thành phố**, hỗ trợ thẩm định, cấp phép và phân bổ nguồn lực.

---

## ⚡ 3. Công nghệ sử dụng (Tech Stack)

- **Frontend:** [React](https://react.dev/)
- **Styling:** CSS thuần / CSS Modules (sẽ cập nhật thêm khi dự án mở rộng)
- **Routing:** React Router DOM (dự kiến)
- **Code Quality:** ESLint, Prettier

---

## 🚀 4. Tính Năng Dự Án

### 🎯 Giai đoạn MVP (Hiện tại)

Tập trung vào nền tảng quản lý thông tin cốt lõi và quy trình phê duyệt:

- **🏢 Đăng ký & Thành lập Startup:** Thành viên gửi đề án thành lập startup với đầy đủ mục tiêu, mô tả và kế hoạch.
- **🛡️ Kiểm duyệt Admin (Thị trưởng):** Xét duyệt hoặc từ chối đề án thành lập; xử lý yêu cầu giải thể dự án.
- **📋 Danh sách Startup:** Hiển thị trực quan toàn bộ các startup đang hoạt động dưới dạng Dashboard / Cards.
- **🔍 Chi tiết Startup:** Xem thông tin tổng quan, trạng thái, định hướng và nhân sự phụ trách.

---

### 🔮 Roadmap Phát Triển Tiếp Theo (Post-MVP)

1. **Quản lý chức năng (Feature Board - Thay thế Todo list truyền thống):**
   - Quản lý theo từng tính năng/module cụ thể (tương tự Kanban/Trello).
   - Quy trình kiểm soát chất lượng rõ ràng:  
     $$\text{Todo} \longrightarrow \text{Đang triển khai} \longrightarrow \text{Chờ review} \longrightarrow \text{Admin review} \longrightarrow \text{Admin duyệt} \longrightarrow \text{Hoàn thành}$$
   - Hỗ trợ triển khai song song nhiều chức năng phù hợp quy mô nhân sự.

2. **Quản lý thành viên & Tuyển dụng nội bộ:**
   - Leader gửi lời mời hoặc phê duyệt thành viên xin gia nhập startup.
   - Phân cấp vai trò rõ ràng giữa Leader và Member.

3. **Kho tài liệu & Guideline chuyển giao:**
   - Mỗi startup có không gian lưu trữ tài liệu kỹ thuật, hướng dẫn sử dụng và tài liệu bàn giao chuẩn hóa.

4. **Activity Logs (Nhật ký hoạt động):**
   - Tự động ghi nhận mọi tương tác, cập nhật giúp Admin theo dõi sức khỏe dự án mà không cần kiểm tra thủ công từng người.

5. **Cơ chế Game hóa – Quỹ Startup (Startup Fund & Burn Rate):**
   - Mỗi startup được cấp một quỹ vốn (ví dụ: `1.000 coin`).
   - Quỹ sẽ tiêu hao theo thời gian (_Burn rate_). Khi liên tục cập nhật, ra mắt tính năng và qua review, startup sẽ được "bơm vốn".
   - Dự án bỏ bê lâu ngày sẽ cạn kiệt quỹ và rơi vào trạng thái _Phá sản_, mở ra cơ hội cho thành viên mới tiếp quản và tái khởi động.

---

## 👥 5. Phân Quyền Vai Trò (Roles & Permissions)

| Vai trò                   | Quyền hạn chính                                                                                                  |
| :------------------------ | :--------------------------------------------------------------------------------------------------------------- |
| **👑 Admin / Thị trưởng** | Kiểm duyệt đề án thành lập/giải thể startup, review tính năng hoàn thành, cấp vốn và giám sát toàn hệ sinh thái. |
| **👨‍💼 Startup Leader**     | Quản lý thông tin startup, duyệt thành viên, phân công & cập nhật chức năng, biên soạn tài liệu kỹ thuật.        |
| **👨‍💻 Member**             | Nhận & thực hiện các chức năng, nộp review tính năng, đóng góp tài liệu và tham gia xây dựng startup.            |

---

## 📂 6. Cấu trúc thư mục (Dự kiến)

```text
startup-bcn/
├── public/                # Tài nguyên tĩnh (Favicon, Logo, Assets)
├── src/
│   ├── assets/            # Hình ảnh, icons, styles
│   ├── components/        # Các UI component tái sử dụng (Navbar, Sidebar, Card, Modal,...)
│   ├── pages/             # Các trang (Dashboard, StartupDetail, RegisterStartup, AdminReview,...)
│   ├── context/ / hooks/  # State management và Custom hooks
│   ├── services/ / data/  # Mock data / API calls
│   ├── types/             # TypeScript definitions / Data models
│   ├── App.jsx / App.tsx  # Router & Root layout
│   └── main.jsx / main.tsx
├── description/           # Tài liệu phân tích yêu cầu & hình ảnh concept
├── .gitignore
├── package.json
└── README.md
```

---

## 💻 7. Hướng dẫn Cài đặt & Khởi chạy (Dự án React)

### Yêu cầu môi trường:

- **Node.js**: `v18.0.0` trở lên
- **npm** hoặc **yarn** / **pnpm**

### Các bước chạy local:

```bash
# 1. Cài đặt các thư viện phụ thuộc
npm install

# 2. Khởi chạy server phát triển (Development mode)
npm run dev

# 3. Build sản phẩm hoàn chỉnh
npm run build
```

---

## 🛠️ 8. Hướng dẫn kết nối GitHub lần đầu

Để đẩy mã nguồn và tài liệu này lên kho lưu trữ GitHub của bạn:

```bash
# 1. Khởi tạo Git repository (nếu chưa có)
git init

# 2. Thêm tất cả các file vào staging
git add .

# 3. Tạo commit đầu tiên
git commit -m "feat: initialize BCN Startup City project with React stack"

# 4. Đổi tên nhánh chính thành main
git branch -M main

# 5. Thêm remote repository GitHub của bạn
git remote add origin https://github.com/<tai-khoan-cua-ban>/<ten-repo>.git

# 6. Push mã nguồn lên GitHub
git push -u origin main
```

---

_Phát triển bởi Ban Công Nghệ (BCN) - Kiến tạo và duy trì các dự án công nghệ bền vững._
