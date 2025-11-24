# Movie Review Website - Project Brief

## Project Overview
Đây là một website review phim được xây dựng bằng PHP và MySQL, chạy trên môi trường XAMPP. Dự án nhằm tạo ra một nền tảng để người yêu phim có thể:
- Chia sẻ thông tin về phim
- Viết review và đánh giá phim
- Thảo luận về phim trong cộng đồng
- Tìm kiếm và khám phá phim mới

## Core Requirements

### Technical Constraints
- **Backend**: PHP (thuần, không framework)
- **Database**: MySQL trên XAMPP
- **Frontend**: Bootstrap (dark mode), tối thiểu JavaScript
- **Environment**: XAMPP trên macOS
- **Language**: Tiếng Việt

### Key Features
1. **User Management**: Đăng ký/đăng nhập, phân quyền (Admin/User)
2. **Movie Management**: Thêm phim, upload poster, phân loại thể loại
3. **Review System**: Viết review, đánh giá sao, comment
4. **Discussion Forum**: Tạo topic thảo luận, comment, upvote/downvote
5. **Search & Filter**: Tìm kiếm phim, lọc theo thể loại
6. **Admin Panel**: Quản lý phim, thể loại, users, reviews

### Design Requirements
- **Dark Theme**: Giao diện tối hiện đại
- **Responsive**: Bootstrap, mobile-friendly
- **Consistent**: Thiết kế đồng nhất giữa các trang
- **Minimal Dependencies**: Hạn chế API và JavaScript

## Project Structure
```
movie-review/
├── config/database.php          # Database connection
├── core/                        # Core MVC classes
├── controllers/                 # Business logic
├── models/                      # Database models
├── views/                       # Templates (PHP)
├── assets/css/js/              # Static files
├── uploads/posters/            # File uploads
└── index.php                   # Entry point with routing
```

## Development Philosophy
- **Step by step**: Làm từng bước một, từng chức năng
- **Simple & Clean**: Code đơn giản, dễ hiểu
- **Vietnamese First**: Giao diện và communication bằng tiếng Việt
- **Student Project**: Học tập về PHP và MySQL trong môi trường thực tế
