# Technical Context - Movie Review Website

## Technology Stack

### Backend
- **PHP 8.2.4**: Server-side language, no framework (thuần PHP)
- **MySQL**: Relational database for data storage
- **PDO**: Database abstraction layer for secure queries
- **Sessions**: User authentication and state management

### Frontend
- **Bootstrap 5**: CSS framework for responsive design
- **Dark Theme**: Custom dark mode styling
- **Minimal JavaScript**: Basic interactions only
- **Font Awesome**: Icon library

### Development Environment
- **XAMPP**: Local development stack (Apache + MySQL + PHP)
- **macOS**: Development platform
- **phpMyAdmin**: Database management interface
- **Apache 2.4.56**: Web server

## Architecture Patterns

### MVC Structure
```
controllers/  -> Business logic and request handling
models/       -> Database interactions and data modeling  
views/        -> Presentation layer (PHP templates)
core/         -> Base classes and utilities
```

### Database Design
- **PDO with prepared statements**: SQL injection protection
- **UTF8MB4 charset**: Full Unicode support for Vietnamese
- **Foreign key constraints**: Data integrity
- **Indexed columns**: Performance optimization

### Routing System
- **Custom URL routing**: SEO-friendly URLs
- **URLHelper class**: Centralized URL generation
- **Clean URLs**: `/movie/123` instead of `?page=movie&id=123`

## Security Measures

### Input Validation
- **Prepared statements**: SQL injection prevention
- **Input sanitization**: XSS protection
- **File upload validation**: Security for poster uploads
- **CSRF protection**: Form token validation

### Authentication
- **Password hashing**: bcrypt for secure password storage
- **Session management**: Secure session handling
- **Role-based access**: Admin vs User permissions

## Performance Considerations

### Database Optimization
- **Indexed queries**: Fast lookups on frequently searched columns
- **Pagination**: Limit results per page
- **Optimized JOINs**: Efficient multi-table queries

### File Handling
- **Image optimization**: Poster upload with size limits
- **Static asset caching**: CSS/JS browser caching
- **Minimal external dependencies**: Faster load times

## Development Constraints

### No External APIs
- Tự xây dựng toàn bộ dữ liệu phim
- Không sử dụng TMDB, IMDB APIs
- Upload poster thủ công

### Minimal JavaScript
- Ưu tiên server-side rendering
- JavaScript chỉ cho UX improvements
- Tránh phụ thuộc vào frontend frameworks

### Vietnamese Language Focus
- UTF8MB4 database charset
- Vietnamese slug generation
- Tiếng Việt comments và interfaces

## Deployment Considerations

### XAMPP Configuration
- Custom socket path for macOS: `/Applications/XAMPP/xamppfiles/var/mysql/mysql.sock`
- File upload permissions: `uploads/posters/` directory
- Apache mod_rewrite: Clean URL support

### File Structure
- Organized MVC folders
- Separated assets (CSS, JS, images)
- Configuration files isolated
- Upload directories secured
