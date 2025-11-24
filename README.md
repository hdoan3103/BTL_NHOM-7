# Website Trao Đổi & Review Phim

## Tổng Quan Dự Án

Website trao đổi/thảo luận/review về các bộ phim là một nền tảng trực tuyến cho phép người dùng chia sẻ, thảo luận và đánh giá các bộ phim yêu thích. Dự án được xây dựng với mục tiêu tạo ra một cộng đồng yêu phim năng động và tương tác.

## Mục Tiêu Dự Án

- Tạo ra một nền tảng để người yêu phim có thể chia sẻ cảm nhận và đánh giá
- Xây dựng cộng đồng thảo luận sôi nổi về các bộ phim
- Cung cấp thông tin chi tiết về các bộ phim
- Hỗ trợ người dùng tìm kiếm và khám phá phim mới

## Ý Tưởng Chính

### Chức Năng Cốt Lõi
1. **Đăng Bài Thông Tin Phim**: Người dùng có thể chia sẻ thông tin về các bộ phim
2. **Review & Đánh Giá**: Viết nhận xét và cho điểm các bộ phim
3. **Thảo Luận Cộng Đồng**: Trao đổi ý kiến về phim trong các topic thảo luận
4. **Tìm Kiếm & Lọc**: Dễ dàng tìm kiếm phim theo nhiều tiêu chí

### Thiết Kế Giao Diện
- **Dark Mode**: Giao diện tối hiện đại, thân thiện với mắt
- **Responsive**: Tương thích mọi thiết bị
- **User-Friendly**: Dễ sử dụng và trực quan

## Công Nghệ Sử Dụng

### Backend
- **PHP**: Ngôn ngữ lập trình chính cho server-side
- **MySQL**: Cơ sở dữ liệu quan hệ để lưu trữ thông tin

### Frontend
- **Bootstrap**: Framework CSS để tạo giao diện responsive
- **Dark Theme**: Chủ đề tối chuyên nghiệp
- **JavaScript**: Tương tác động trên giao diện

### Environment
- **XAMPP**: Môi trường phát triển local
- **Apache**: Web server
- **phpMyAdmin**: Quản lý cơ sở dữ liệu

## Phân Tích Yêu Cầu

### Chức Năng Chính

#### 1. Quản Lý Người Dùng
- Đăng ký/Đăng nhập
- Quản lý profile cá nhân
- Phân quyền người dùng (Admin, User thường)

#### 2. Quản Lý Phim
- Thêm thông tin phim mới
- Chỉnh sửa thông tin phim
- Upload poster/hình ảnh
- Phân loại theo thể loại

#### 3. Hệ Thống Review
- Viết review chi tiết
- Đánh giá sao (1-5 sao)
- Like/Dislike review
- Comment trên review

#### 4. Diễn Đàn Thảo Luận
- Tạo topic thảo luận
- Comment và reply
- Upvote/Downvote
- Theo dõi topic

#### 5. Tìm Kiếm & Lọc
- Tìm kiếm theo tên phim
- Lọc theo thể loại
- Sắp xếp theo rating
- Gợi ý phim tương tự

### Thiết Kế Cơ Sở Dữ Liệu

#### Bảng Chính
- **users**: Thông tin người dùng
- **movies**: Thông tin phim
- **reviews**: Đánh giá phim
- **discussions**: Topic thảo luận
- **comments**: Bình luận
- **genres**: Thể loại phim
- **ratings**: Điểm đánh giá

## Thiết Kế UI/UX

### Dark Mode Theme
- Màu nền tối (#1a1a1a, #2d2d2d)
- Text màu sáng (#ffffff, #f0f0f0)
- Accent colors nổi bật
- Card design với shadow

### Layout Structure
- **Header**: Navigation, search, user menu
- **Sidebar**: Categories, filters
- **Main Content**: Movie cards, reviews, discussions
- **Footer**: Links, info
- 
## Kế Hoạch Phát Triển

### Phase 1: Cơ Bản
- [ ] Setup environment
- [ ] Thiết kế database
- [ ] Tạo giao diện cơ bản
- [ ] Chức năng đăng ký/đăng nhập

### Phase 2: Core Features
- [ ] Quản lý phim
- [ ] Hệ thống review
- [ ] Tìm kiếm cơ bản

### Phase 3: Advanced
- [ ] Diễn đàn thảo luận
- [ ] Tương tác xã hội
- [ ] Tối ưu performance

### Phase 4: Polish
- [ ] Testing
- [ ] Bug fixes
- [ ] Documentation
- [ ] Deployment

## Đối Tượng Người Dùng

- **Người yêu phim**: Muốn chia sẻ cảm nhận về phim
- **Critic nghiệp dư**: Viết review chuyên sâu
- **Người tìm phim**: Tham khảo ý kiến trước khi xem
- **Cộng đồng**: Thảo luận và tranh luận về phim

## Tiềm Năng Mở Rộng

- Tích hợp API phim (TMDB, IMDB)
- Mobile app
- Recommendation system
- Social features nâng cao
- Monetization (ads, premium)

## Bảo Mật

- Validation input
- SQL injection prevention
- XSS protection
- Session management
- Password hashing

## Responsive Design

- Mobile-first approach
- Tablet optimization
- Desktop enhancement
- Cross-browser compatibility

## URL Routing System

### URL Patterns được hỗ trợ:

#### Trang chủ:
- `/` hoặc `/home` - Trang chủ

#### Phim:
- `/movie` hoặc `/movies` - Danh sách phim
- `/movie?search=keyword` - Tìm kiếm phim
- `/movie?genre=action` - Lọc theo thể loại
- `/movie/123` hoặc `/movie/detail/123` - Chi tiết phim với ID 123

#### Review:
- `/review/write/123` - Viết review cho phim ID 123

#### Thảo luận:
- `/discussion` hoặc `/discussions` - Danh sách thảo luận
- `/discussion?search=keyword` - Tìm kiếm thảo luận
- `/discussion?movie_id=123` - Thảo luận về phim ID 123
- `/discussion/123` hoặc `/discussion/detail/123` - Chi tiết thảo luận ID 123
- `/discussion/create` - Tạo thảo luận mới
- `/discussion/create?movie_id=123` - Tạo thảo luận cho phim ID 123

#### Người dùng:
- `/user/profile` hoặc `/profile` - Hồ sơ người dùng
- `/user/reviews` - Reviews của người dùng

#### Xác thực:
- `/auth/login` hoặc `/login` - Đăng nhập
- `/auth/register` hoặc `/register` - Đăng ký
- `/auth/logout` hoặc `/logout` - Đăng xuất

### Sử dụng URLHelper trong code:

```php
// Thay vì hardcode URL:
echo '<a href="' . BASE_URL . '/movie/detail/' . $movie['id'] . '">Chi tiết</a>';

// Sử dụng URLHelper:
echo '<a href="' . URLHelper::movieDetail($movie['id']) . '">Chi tiết</a>';
```

### Các phương thức URLHelper có sẵn:
- `URLHelper::home()` - Trang chủ
- `URLHelper::movies($search, $genre)` - Danh sách phim
- `URLHelper::movieDetail($movieId)` - Chi tiết phim
- `URLHelper::writeReview($movieId)` - Viết review
- `URLHelper::discussions($search, $movie_id)` - Danh sách thảo luận
- `URLHelper::discussionDetail($discussionId)` - Chi tiết thảo luận
- `URLHelper::createDiscussion($movieId)` - Tạo thảo luận
- `URLHelper::userProfile()` - Hồ sơ người dùng
- `URLHelper::userReviews()` - Reviews của người dùng
- `URLHelper::login()`, `URLHelper::register()`, `URLHelper::logout()` - Xác thực
- `URLHelper::poster($filename)` - URL poster phim
- `URLHelper::isActive($path)` - Kiểm tra active navigation

---

*Dự án được phát triển như một phần của khóa học lập trình web, nhằm tạo ra một nền tảng hoàn chỉnh cho cộng đồng yêu phim.*
