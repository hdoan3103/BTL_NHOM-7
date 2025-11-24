# **I. Lý do vì sao muốn xây dựng website này, đơn vị sở hữu website, người sử dụng website**

## **1.1. Lý do vì sao muốn xây dựng Website Review Phim**

Việc xây dựng website Review Phim xuất phát từ thực tế thiếu hụt các nền tảng đánh giá phim bằng tiếng Việt chất lượng cho cộng đồng người yêu điện ảnh Việt Nam. Các trang review phim quốc tế như IMDb, Rotten Tomatoes tuy nổi tiếng nhưng không phù hợp với văn hóa và quan điểm thẩm mỹ của người Việt, đồng thời rào cản ngôn ngữ hạn chế việc tham gia thảo luận sâu sắc.

Website được tạo ra để phục vụ những mục đích cụ thể:

**Tạo cộng đồng yêu phim Việt Nam:** Xây dựng một nền tảng trực tuyến nơi người yêu phim có thể tự do chia sẻ cảm nhận, viết review chuyên sâu và thảo luận về phim bằng tiếng mẹ đẻ.

**Cung cấp thông tin phim đáng tin cậy:** Người dùng có thể dễ dàng tìm hiểu thông tin chi tiết về phim, đọc các bài đánh giá từ cộng đồng và tham khảo rating trước khi quyết định xem phim.

**Hỗ trợ khám phá phim mới:** Hệ thống phân loại theo thể loại và tính năng tìm kiếm giúp người dùng khám phá những bộ phim phù hợp với sở thích cá nhân.

**Xây dựng cơ sở dữ liệu phim Việt:** Lưu trữ và tổ chức thông tin phim một cách có hệ thống, góp phần bảo tồn và phát triển văn hóa thảo luận điện ảnh Việt Nam.

## **1.2. Đơn vị sở hữu website**

**Tên dự án:** Website Review Phim Việt Nam  
**Đơn vị phát triển:** Nhóm sinh viên Công nghệ Thông tin  
**Môi trường phát triển:** XAMPP Local Development  
**Công nghệ sử dụng:** PHP, MySQL, Bootstrap  
**Địa chỉ website:** <http://localhost/movie-review>  
**Email liên hệ:** <admin@moviereview.vn>

## **1.3. Người sử dụng website**

Website Review Phim phục vụ các nhóm đối tượng chính sau:

**Người yêu phim cá nhân:** Những người muốn tìm hiểu thông tin phim, đọc review từ cộng đồng và chia sẻ cảm nhận cá nhân về các bộ phim đã xem.

**Movie critic nghiệp dư:** Những người có đam mê viết lách về phim, muốn xây dựng danh tiếng và chia sẻ những bài phân tích chuyên sâu với cộng đồng.

**Sinh viên điện ảnh:** Học viên và người nghiên cứu về điện ảnh, cần nguồn tài liệu tham khảo và môi trường trao đổi kiến thức chuyên môn.

**Cộng đồng thảo luận:** Những thành viên tích cực tham gia các cuộc thảo luận về phim, tranh luận về nghệ thuật điện ảnh và xu hướng phim ảnh.

**Quản trị viên:** Những người có trách nhiệm quản lý nội dung, kiểm duyệt bài viết và duy trì chất lượng của nền tảng.

# **II. Các yêu cầu về nội dung, chức năng, giao diện của website**

## **2.1. Yêu cầu về nội dung**

Website Review Phim cần cung cấp nội dung phong phú và có tổ chức để phục vụ nhu cầu đa dạng của người dùng:

**Trang chủ (Home):** Hiển thị những bộ phim mới nhất được thêm vào hệ thống, phim có rating cao nhất từ cộng đồng, và các thảo luận nổi bật. Giao diện trang chủ cần trực quan, giúp người dùng nhanh chóng nắm bắt được những nội dung hot nhất.

**Danh sách phim (Movies):** Trình bày thông tin tổng quan về các bộ phim bao gồm poster chất lượng cao, tên phim, thể loại, năm phát hành, đạo diễn và rating trung bình từ cộng đồng. Hỗ trợ phân trang và sắp xếp theo nhiều tiêu chí.

**Chi tiết phim (Movie Details):** Cung cấp thông tin đầy đủ về từng bộ phim bao gồm synopsis chi tiết, thông tin đạo diễn, dàn diễn viên, thể loại, năm phát hành, thời lượng và poster chất lượng cao. Trang này cũng tổng hợp tất cả review từ cộng đồng.

**Hệ thống Review:** Cho phép người dùng viết review chi tiết với hệ thống đánh giá sao từ 1-5, tạo tiêu đề hấp dẫn và nội dung review phong phú. Các review được hiển thị theo thứ tự thời gian hoặc rating.

**Diễn đàn thảo luận (Discussions):** Nơi diễn ra các cuộc thảo luận về phim, từ phân tích chuyên sâu đến chia sẻ cảm nhận cá nhân. Hỗ trợ tạo topic mới và bình luận trên các chủ đề có sẵn.

**Trang cá nhân (User Profile):** Hiển thị thông tin cá nhân của người dùng, lịch sử các review đã viết, thảo luận đã tham gia và thống kê hoạt động.

**Panel quản trị (Admin Panel):** Giao diện quản lý dành cho admin với các chức năng quản lý phim, thể loại, người dùng, kiểm duyệt review và thống kê hệ thống.

## **2.2. Yêu cầu về chức năng**

Website cần có các chức năng cốt lõi sau để đáp ứng nhu cầu người dùng:

**Đăng ký và đăng nhập:** Hệ thống xác thực người dùng an toàn với validation đầy đủ, hỗ trợ đăng ký tài khoản mới và đăng nhập cho thành viên hiện có.

**Quản lý phim:** Admin có thể thêm, sửa, xóa thông tin phim, upload poster và phân loại theo thể loại. Hỗ trợ tạo slug tự động cho URL thân thiện SEO.

**Viết và quản lý Review:** Người dùng có thể viết review chi tiết, đánh giá sao, chỉnh sửa review của mình. Hệ thống tự động tính rating trung bình cho mỗi phim.

**Hệ thống thảo luận:** Tạo topic thảo luận mới, bình luận và phản hồi trong các chủ đề. Hiển thị thảo luận hot và theo dõi topic yêu thích.

**Tìm kiếm và lọc:** Tìm kiếm phim theo từ khóa, lọc theo thể loại, năm phát hành, đạo diễn. Hỗ trợ sắp xếp kết quả theo rating, thời gian.

**Quản trị hệ thống:** Admin có thể quản lý người dùng, kiểm duyệt nội dung, xem thống kê và cấu hình hệ thống.

## **2.3. Yêu cầu về giao diện**

Giao diện website cần đáp ứng các tiêu chuẩn hiện đại về UX/UI:

**Thiết kế tổng thể:** Sử dụng Dark Theme làm chủ đạo với màu nền tối, text sáng và accent colors nổi bật. Tạo cảm giác hiện đại, chuyên nghiệp và thân thiện với mắt khi sử dụng lâu.

**Bố cục responsive:** Giao diện tương thích hoàn toàn trên mobile, tablet và desktop. Sử dụng Bootstrap framework để đảm bảo responsive design và consistency.

**Navigation:** Menu điều hướng rõ ràng, cố định và dễ sử dụng. Search bar dễ tiếp cận từ mọi trang.

**Typography:** Font chữ dễ đọc, hỗ trợ tiếng Việt tốt. Hierarchy rõ ràng giữa các cấp độ heading và content.

**Hình ảnh:** Poster phim chất lượng cao, tối ưu về dung lượng. Hỗ trợ lazy loading và placeholder khi chưa có ảnh.

**Performance:** Tốc độ tải trang nhanh dưới 3 giây, tối ưu database queries và static assets.

**Accessibility:** Tuân thủ các chuẩn web accessibility, hỗ trợ keyboard navigation và screen reader.

# **III. Thiết kế nội dung, chức năng, giao diện của website, mô hình dữ liệu**

## **3.1. Thiết kế nội dung**

### **3.1.1. Bố cục giao diện tổng thể**

Website được thiết kế theo mô hình MVC với bố cục nhất quán trên toàn bộ các trang:

**Header:** Chứa logo website, menu điều hướng chính (Trang chủ, Phim, Thảo luận), thanh tìm kiếm và menu người dùng (đăng nhập/đăng ký hoặc thông tin cá nhân).

**Hero Section:** Banner chính trên trang chủ hiển thị phim nổi bật với call-to-action button.

**Main Content:** Khu vực nội dung chính được bố trí theo grid layout, hiển thị danh sách phim với poster, rating và thông tin cơ bản.

**Sidebar:** Panel bên phải chứa bộ lọc theo thể loại, năm phát hành và danh sách top movies trending.

**Footer:** Chứa các links hữu ích, thông tin về website, contact và social media.

### **3.1.2. Thiết kế màu sắc**

Website sử dụng Dark Theme làm chủ đạo để tạo cảm giác hiện đại và chuyên nghiệp:

**Màu nền chính:** #0d1117 (background tối), #161b22 (secondary background)
**Màu text:** #f0f6fc (text chính), #7d8590 (text phụ)
**Màu accent:** #f78166 (orange cho buttons), #58a6ff (blue cho links)
**Màu components:** #21262d (nền card), #30363d (borders)

### **3.1.3. Typography và hình ảnh**

**Font chữ:** Sử dụng system font stack để đảm bảo hiệu suất tối ưu và tương thích đa nền tảng.

**Hierarchy:** H1 (2.5rem), H2 (2rem), H3 (1.75rem), body text (1rem) với weights từ Regular (400) đến Bold (700).

**Poster phim:** Tỷ lệ chuẩn 2:3, resolution minimum 300x450px, hỗ trợ lazy loading.

**Responsive images:** Tự động resize theo screen size, có placeholder khi chưa load.

## **3.2. Thiết kế chức năng**

Website Movie Review được thiết kế với các chức năng chi tiết cho từng trang như sau:

### **3.2.1. Trang Chủ (Home Page)**

**Controller:** `HomeController::index()`

**Chức năng chính:**
- Hiển thị hero section với tiêu đề chào mừng và call-to-action buttons
- Lấy và hiển thị 6 phim mới nhất được thêm vào hệ thống
- Lấy và hiển thị 6 phim có rating cao nhất từ cộng đồng
- Mỗi phim được hiển thị với poster, title, description, thể loại, năm phát hành và button "Xem Chi Tiết"

**Dữ liệu được xử lý:**
- `$latestMovies`: Danh sách phim mới nhất (limit 6)
- `$topRatedMovies`: Danh sách phim rating cao nhất (limit 6)
- Navigation buttons cho guest users (Khám Phá Phim, Tham Gia Ngay)

### **3.2.2. Danh Sách Phim (Movie Listing)**

**Controller:** `MovieController::index()`

**Chức năng tìm kiếm và lọc:**
- Tìm kiếm phim theo từ khóa trong title, description, director
- Lọc phim theo thể loại (genre dropdown)
- Hiển thị kết quả tìm kiếm với số lượng phim tìm thấy
- Hiển thị tất cả phim nếu không có tìm kiếm

**Hiển thị dữ liệu:**
- Poster phim với fallback nếu không có ảnh
- Thông tin cơ bản: title, description (rút gọn 100 ký tự), thể loại, năm phát hành
- Button "Xem Chi Tiết" để chuyển đến trang detail

**Tham số URL:**
- `?search=keyword`: Tìm kiếm theo từ khóa
- `?genre=id`: Lọc theo thể loại

### **3.2.3. Chi Tiết Phim (Movie Detail)**

**Controller:** `MovieController::detail($id)`

**Chức năng chính:**
- Hiển thị thông tin đầy đủ của phim: poster, title, description, director, cast, genre, năm phát hành
- Lấy và hiển thị tất cả reviews của phim với rating và nội dung
- Lấy và hiển thị các thảo luận liên quan đến phim
- Kiểm tra và hiển thị review của user hiện tại (nếu đã đăng nhập)

**Validation:**
- Kiểm tra ID phim hợp lệ (numeric)
- Kiểm tra phim có tồn tại trong database
- Redirect về movie listing nếu có lỗi

**Dữ liệu được xử lý:**
- `$movie`: Thông tin chi tiết phim
- `$reviews`: Tất cả reviews của phim
- `$discussions`: Thảo luận liên quan đến phim
- `$userReview`: Review của user hiện tại (nếu có)

### **3.2.4. Hệ thống Authentication**

**Login Controller:** `AuthController::login()`

**Chức năng đăng nhập:**
- Form với username/email và password
- Validation: kiểm tra fields không rỗng
- Xác thực thông tin qua `User::login()` method
- Tạo session với user_id, username, full_name, role
- Redirect về trang chủ khi thành công

**Register Controller:** `AuthController::register()`

**Chức năng đăng ký:**
- Form validation đầy đủ: username (min 3 chars), email (valid format), password (min 6 chars)
- Kiểm tra confirm password khớp
- Kiểm tra username và email chưa tồn tại
- Hash password và lưu vào database
- Redirect đến trang login khi thành công

**Logout:** Xóa tất cả session và redirect về trang chủ

### **3.2.5. Hệ thống Review**

**Controller:** `ReviewController::write($movieId)`

**Chức năng viết review:**
- Yêu cầu đăng nhập (`requireLogin()`)
- Kiểm tra movie ID hợp lệ và phim tồn tại
- Kiểm tra user đã review phim này chưa
- Form với title, content, rating (1-5 sao)
- Validation đầy đủ cho tất cả fields
- Cập nhật review nếu đã tồn tại, tạo mới nếu chưa

**Dữ liệu xử lý:**
- `$movie`: Thông tin phim để review
- `$existingReview`: Review hiện tại của user (nếu có)
- Hỗ trợ cả create và update review trong cùng một form

### **3.2.6. Hệ thống Thảo Luận**

**Discussion Listing:** `DiscussionController::index()`

**Chức năng chính:**
- Hiển thị tất cả discussions với thông tin chi tiết
- Tìm kiếm discussion theo từ khóa trong title/content
- Lọc discussions theo phim cụ thể
- Hiển thị "hot discussions" (5 discussions nổi bật)
- Dropdown danh sách phim để lọc

**Discussion Detail:** `DiscussionController::detail($id)`

**Chức năng chi tiết:**
- Hiển thị nội dung đầy đủ của discussion
- Thông tin người tạo và thời gian
- Số lượt xem (views counter)
- Liên kết đến phim liên quan (nếu có)

**Tham số URL:**
- `?search=keyword`: Tìm kiếm discussions
- `?movie=id`: Lọc theo phim

### **3.2.7. Trang Cá Nhân User**

**Controller:** `UserController::profile()`

**Chức năng profile:**
- Yêu cầu đăng nhập để truy cập
- Hiển thị thông tin cá nhân của user
- Thống kê hoạt động: số reviews, discussions đã tạo
- Hiển thị 5 reviews gần đây của user
- Hiển thị 5 discussions gần đây của user
- Form cập nhật thông tin cá nhân

**Reviews page:** `UserController::reviews()`

**Chức năng quản lý reviews:**
- Hiển thị tất cả reviews của user với phân trang
- Sắp xếp theo thời gian (mới nhất trước)
- Links để chỉnh sửa hoặc xem detail mỗi review

### **3.2.8. Hệ thống Admin**

**Admin Dashboard:** `AdminController::dashboard()`

**Chức năng tổng quan:**
- Thống kê tổng số phim, users, reviews, discussions
- Danh sách phim, users, reviews, discussions mới nhất
- Quick actions: thêm phim mới, quản lý genres

**Quản lý Phim:** `AdminController` - movies section

**Chức năng CRUD:**
- Listing: Hiển thị tất cả phim với thông tin cơ bản và actions
- Create: Form thêm phim mới với upload poster, chọn genre
- Edit: Form chỉnh sửa thông tin phim, thay đổi poster
- Delete: Xóa phim với confirmation

**Quản lý Thể Loại:** `AdminController` - genres section

**Chức năng CRUD:**
- Listing: Hiển thị tất cả genres với số phim thuộc mỗi thể loại
- Create: Form thêm genre mới với auto-generate slug
- Edit: Form chỉnh sửa tên và slug của genre
- Delete: Xóa genre (kiểm tra không có phim liên kết)

**Quản lý Users và Reviews:**
- User management: Xem danh sách users, thay đổi role, khóa tài khoản
- Review moderation: Duyệt, từ chối hoặc xóa reviews

### **3.2.9. Tính năng Navigation và Security**

**URL Routing:**
- SEO-friendly URLs với slug cho phim và genres
- Clean URLs không hiển thị file extensions
- Breadcrumb navigation cho user experience

**Security Features:**
- Session-based authentication
- Password hashing với bcrypt
- CSRF protection cho forms
- Input validation và sanitization
- File upload validation (type, size)
- Admin role checking cho protected actions

**Error Handling:**
- 404 page cho resources không tồn tại
- Flash messages cho success/error notifications
- Form validation messages
- Graceful fallbacks cho missing data (ví dụ: no poster)

## **3.3. Thiết kế giao diện**

### **3.3.1. Thiết kế phản hồi (Responsive Design)**

**Thiết kế ưu tiên di động (Mobile-first):**

- Hệ thống lưới Bootstrap cho bố cục phản hồi đa thiết bị
- Menu hamburger cho điều hướng trên thiết bị di động
- Các nút và liên kết thân thiện với cảm ứng
- Kích thước hình ảnh được tối ưu hóa cho di động

**Cải tiến cho màn hình desktop:**

- Hiệu ứng hover cho các thành phần tương tác
- Phím tắt bàn phím
- Bố cục nhiều cột
- Thanh lọc nâng cao ở sidebar

### **3.3.2. Trải nghiệm người dùng (User Experience)**

**Trạng thái loading:**

- Màn hình skeleton cho việc tải nội dung
- Thanh tiến trình cho tải file lên
- Biểu tượng xoay cho các yêu cầu AJAX
- Xử lý lỗi với thông báo thân thiện người dùng

**Khả năng tiếp cận (Accessibility):**

- Cấu trúc HTML ngữ nghĩa rõ ràng
- Nhãn ARIA cho trình đọc màn hình
- Hỗ trợ điều hướng bằng bàn phím
- Tuân thủ độ tương phản màu sắc (WCAG 2.1)

## **3.4. Mô hình dữ liệu**

### **3.4.1. Cấu trúc bảng cơ sở dữ liệu**

**Bảng users:**

| Trường | Kiểu dữ liệu | Thuộc tính | Mô tả |
|--------|-------------|------------|-------|
| id | INT | PRIMARY KEY, AUTO_INCREMENT | ID người dùng |
| username | VARCHAR(50) | UNIQUE, NOT NULL | Tên đăng nhập |
| email | VARCHAR(100) | UNIQUE, NOT NULL | Địa chỉ email |
| password | VARCHAR(255) | NOT NULL | Mật khẩu đã hash |
| full_name | VARCHAR(100) | NOT NULL | Họ và tên |
| role | ENUM('user', 'admin') | DEFAULT 'user' | Vai trò người dùng |
| avatar | VARCHAR(255) | NULL | Đường dẫn ảnh đại diện |
| created_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP | Thời gian tạo |
| updated_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP | Thời gian cập nhật |

**Bảng movies:**

| Trường | Kiểu dữ liệu | Thuộc tính | Mô tả |
|--------|-------------|------------|-------|
| id | INT | PRIMARY KEY, AUTO_INCREMENT | ID phim |
| title | VARCHAR(255) | NOT NULL | Tên phim |
| slug | VARCHAR(255) | UNIQUE, NOT NULL | URL slug |
| description | TEXT | NULL | Mô tả phim |
| director | VARCHAR(100) | NULL | Đạo diễn |
| cast | TEXT | NULL | Dàn diễn viên |
| release_year | YEAR | NULL | Năm phát hành |
| duration | INT | NULL | Thời lượng (phút) |
| poster | VARCHAR(255) | NULL | Đường dẫn poster |
| genre_id | INT | FOREIGN KEY REFERENCES genres(id) | ID thể loại |
| created_by | INT | FOREIGN KEY REFERENCES users(id) | Người tạo |
| status | ENUM('active', 'inactive') | DEFAULT 'active' | Trạng thái |
| created_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP | Thời gian tạo |
| updated_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP | Thời gian cập nhật |

**Bảng genres:**

| Trường | Kiểu dữ liệu | Thuộc tính | Mô tả |
|--------|-------------|------------|-------|
| id | INT | PRIMARY KEY, AUTO_INCREMENT | ID thể loại |
| name | VARCHAR(100) | UNIQUE, NOT NULL | Tên thể loại |
| slug | VARCHAR(100) | UNIQUE, NOT NULL | URL slug |
| description | TEXT | NULL | Mô tả thể loại |
| created_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP | Thời gian tạo |

**Bảng reviews:**

| Trường | Kiểu dữ liệu | Thuộc tính | Mô tả |
|--------|-------------|------------|-------|
| id | INT | PRIMARY KEY, AUTO_INCREMENT | ID review |
| movie_id | INT | FOREIGN KEY REFERENCES movies(id) | ID phim |
| user_id | INT | FOREIGN KEY REFERENCES users(id) | ID người dùng |
| title | VARCHAR(255) | NOT NULL | Tiêu đề review |
| content | TEXT | NOT NULL | Nội dung review |
| rating | TINYINT | CHECK(rating >= 1 AND rating <= 5) | Đánh giá (1-5 sao) |
| status | ENUM('pending', 'approved', 'rejected') | DEFAULT 'pending' | Trạng thái duyệt |
| created_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP | Thời gian tạo |
| updated_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP | Thời gian cập nhật |

**Bảng discussions:**

| Trường | Kiểu dữ liệu | Thuộc tính | Mô tả |
|--------|-------------|------------|-------|
| id | INT | PRIMARY KEY, AUTO_INCREMENT | ID thảo luận |
| title | VARCHAR(255) | NOT NULL | Tiêu đề thảo luận |
| content | TEXT | NOT NULL | Nội dung thảo luận |
| movie_id | INT | FOREIGN KEY REFERENCES movies(id), NULL | ID phim (optional) |
| user_id | INT | FOREIGN KEY REFERENCES users(id) | ID người tạo |
| views | INT | DEFAULT 0 | Số lượt xem |
| status | ENUM('active', 'closed') | DEFAULT 'active' | Trạng thái |
| created_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP | Thời gian tạo |
| updated_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP | Thời gian cập nhật |

**Bảng comments:**

| Trường | Kiểu dữ liệu | Thuộc tính | Mô tả |
|--------|-------------|------------|-------|
| id | INT | PRIMARY KEY, AUTO_INCREMENT | ID comment |
| content | TEXT | NOT NULL | Nội dung comment |
| user_id | INT | FOREIGN KEY REFERENCES users(id) | ID người dùng |
| review_id | INT | FOREIGN KEY REFERENCES reviews(id), NULL | ID review (nếu comment thuộc review) |
| discussion_id | INT | FOREIGN KEY REFERENCES discussions(id), NULL | ID thảo luận (nếu comment thuộc discussion) |
| parent_id | INT | FOREIGN KEY REFERENCES comments(id), NULL | ID comment cha (cho threaded replies) |
| status | ENUM('active', 'hidden') | DEFAULT 'active' | Trạng thái hiển thị |
| created_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP | Thời gian tạo |
| updated_at | TIMESTAMP | DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP | Thời gian cập nhật |

### **3.4.2. Relationships và Indexes**

**Quan hệ giữa các bảng:**

- **One-to-Many:** users → reviews, users → discussions, users → comments, genres → movies, movies → reviews, reviews → comments, discussions → comments
- **Many-to-One:** reviews → movies, discussions → movies, comments → users
- **Self-referencing:** comments → comments (parent_id cho threaded comments)
- **Optional relationships:** discussions → movies (có thể không liên kết phim), comments → reviews/discussions (comment thuộc về review hoặc discussion)
- **Foreign Key Constraints:** Đảm bảo data integrity và cascade deletes

**Indexing Strategy:**
- **Primary Keys:** Auto-increment integers cho performance
- **Search Indexes:** title, director fields cho full-text search
- **Composite Indexes:** (movie_id, user_id) cho unique review per user per movie
- **Status Indexes:** Trên status fields cho filtering queries

**Data Validation:**
- **NOT NULL constraints:** Cho required fields
- **UNIQUE constraints:** Username, email, slugs
- **CHECK constraints:** Rating range, status enums
- **Foreign Key constraints:** Referential integrity

# **IV. Các ngôn ngữ lập trình sử dụng để xây dựng website, demo các phần cài đặt**

## **4.1. HTML**

HTML là ngôn ngữ đánh dấu cơ bản được sử dụng để thiết kế cấu trúc tổng thể của website Movie Review. Trong quá trình xây dựng website, bước đầu tiên là sử dụng HTML để xác định các thành phần chính như header chứa logo và menu điều hướng, thanh tìm kiếm, khu vực nội dung chính hiển thị danh sách phim, sidebar chứa bộ lọc thể loại và footer thông tin liên hệ. Sau khi cấu trúc được xác định, nội dung sẽ được thêm vào thông qua các thẻ HTML phù hợp, bao gồm thông tin phim, poster, mô tả, đánh giá sao và các review từ người dùng nhằm tạo ra một trải nghiệm phong phú cho cộng đồng yêu phim. Ngoài ra, HTML còn cho phép tạo liên kết giữa các trang phim, từ danh sách đến chi tiết phim, từ review đến thảo luận, giúp cải thiện khả năng điều hướng trong website. Cuối cùng, các biểu mẫu đăng ký, đăng nhập, viết review và tạo thảo luận cũng được xây dựng bằng HTML để người dùng có thể tham gia cộng đồng và chia sẻ cảm nhận về phim một cách thuận tiện.

## **4.2. CSS**

CSS (Cascading Style Sheets) được sử dụng để định dạng và trình bày giao diện website Movie Review theo phong cách Dark Theme hiện đại và hấp dẫn. Với CSS, ta có thể thiết lập màu nền tối (#0d1117), màu text sáng (#f0f6fc), và các màu accent nổi bật như cam (#f78166) cho buttons và xanh (#58a6ff) cho links, tạo nên một giao diện chuyên nghiệp phù hợp với theme điện ảnh. CSS cũng được sử dụng để định dạng layout responsive với Bootstrap framework, đảm bảo website hiển thị tốt trên mọi thiết bị từ mobile đến desktop. Ngoài ra, CSS còn cho phép tạo các hiệu ứng hover cho poster phim, animation cho rating sao, và styling cho các components như cards hiển thị phim, buttons điều hướng, form inputs, nhằm tăng tính tương tác và sinh động cho website, đồng thời giúp sắp xếp các phần tử hợp lý với grid layout rõ ràng và dễ theo dõi.

## **4.3. JavaScript**

JavaScript đóng vai trò quan trọng trong việc tăng tính tương tác và động cho website Movie Review, tuy nhiên theo yêu cầu thiết kế, việc sử dụng JavaScript được hạn chế tối đa để tập trung vào xử lý server-side với PHP. Khi người dùng thực hiện các hành động như click vào rating sao, hover poster phim, hoặc submit form, JavaScript có thể xử lý các validation cơ bản và hiệu ứng visual feedback theo thời gian thực. JavaScript còn được sử dụng tối thiểu để tạo các hiệu ứng smooth scrolling, image lazy loading cho poster phim, và basic form validation trước khi gửi lên server, giúp cải thiện user experience mà không làm phức tạp hệ thống. Trong tương lai, JavaScript có thể được mở rộng để hỗ trợ các tính năng như real-time notifications cho discussions mới, AJAX loading cho pagination, và search suggestions, nhưng hiện tại được giữ ở mức minimal để đảm bảo tính đơn giản và ổn định của ứng dụng web.

## **4.4. PHP**

PHP là ngôn ngữ phía máy chủ chính được sử dụng để xây dựng toàn bộ logic backend cho website Movie Review theo mô hình MVC (Model-View-Controller). PHP xử lý tất cả các biểu mẫu HTML từ đăng ký, đăng nhập, đến viết review, tạo thảo luận và quản lý phim, cho phép thu thập và xử lý dữ liệu người dùng một cách an toàn với validation đầy đủ và password hashing. Quan trọng nhất, PHP có khả năng kết nối và tương tác mạnh mẽ với MySQL database thông qua PDO, giúp lưu trữ, truy xuất và cập nhật dữ liệu về phim, users, reviews, discussions và comments một cách hiệu quả với prepared statements để bảo mật chống SQL injection. PHP cũng được sử dụng để xây dựng hệ thống authentication với session management, role-based access control phân quyền user và admin, file upload handling cho poster phim, URL routing với slug generation cho SEO, và template rendering cho các view pages, góp phần tạo nên một ứng dụng web đầy đủ tính năng và bảo mật cao.

## **4.5. MySQL**

MySQL là hệ quản trị cơ sở dữ liệu quan hệ được sử dụng để lưu trữ toàn bộ dữ liệu của website Movie Review trong môi trường XAMPP. Database được thiết kế với 6 bảng chính (users, movies, genres, reviews, discussions, comments) có quan hệ chặt chẽ thông qua foreign keys để đảm bảo tính toàn vẹn dữ liệu. MySQL hỗ trợ các tính năng quan trọng như FULLTEXT search cho tìm kiếm phim theo title và description, indexing cho performance tối ưu, transaction handling cho các thao tác phức tạp, và constraint checking để validation dữ liệu ở database level. Bên cạnh đó, MySQL còn cung cấp các function built-in như AVG() để tính rating trung bình cho phim, COUNT() để thống kê số lượng reviews và discussions, DATE functions để sắp xếp theo thời gian, và ENUM types để quản lý status của các records, giúp website có thể xử lý và truy vấn dữ liệu một cách nhanh chóng và chính xác.

## **4.6. Bootstrap Framework**

Bootstrap là framework CSS được sử dụng làm nền tảng cho responsive design và UI components của website Movie Review. Bootstrap cung cấp hệ thống grid 12-column giúp tạo layout responsive tự động thích ứng từ mobile đến desktop, các utility classes cho spacing, typography và colors giúp maintain consistency across toàn bộ website. Framework này cũng cung cấp sẵn các components như navbar với hamburger menu, cards cho hiển thị movie items, modals cho confirmations, forms với validation styling, buttons với various states, và pagination components. Đặc biệt, Bootstrap được customize để phù hợp với Dark Theme của website thông qua việc override các CSS variables và classes, tạo nên một giao diện độc đáo mà vẫn giữ được tính nhất quán và professional. Việc sử dụng Bootstrap giúp giảm thiểu code CSS tự viết, tăng tốc development process, và đảm bảo cross-browser compatibility cũng như mobile-first responsive design.

# **V. Đánh giá kết quả và kết luận**

## **5.1. Đánh giá**

Dự án thiết kế website Movie Review đã đáp ứng tốt các yêu cầu cơ bản về giao diện, nội dung và chức năng cho một nền tảng đánh giá phim bằng tiếng Việt. Giao diện được thiết kế theo Dark Theme hiện đại với màu sắc hài hòa, typography rõ ràng và layout responsive, mang lại ấn tượng chuyên nghiệp cho người dùng yêu thích điện ảnh ngay từ lần truy cập đầu tiên. Các chức năng chính như đăng ký, đăng nhập, xem danh sách phim, viết review, tham gia thảo luận và quản trị hệ thống đều hoạt động trơn tru, đảm bảo luồng thao tác đơn giản và trực quan. Trải nghiệm người dùng được tối ưu nhờ bố cục hợp lý với search và filter functionality, quy trình viết review rõ ràng với rating system 1-5 sao, và hệ thống thảo luận organized theo từng phim. Người dùng có thể dễ dàng tìm kiếm phim theo tên hoặc thể loại, đọc reviews từ cộng đồng, chia sẻ cảm nhận cá nhân và tham gia discussions sôi nổi.

Tuy nhiên, hệ thống hiện tại vẫn ở mức development cơ bản, chưa tích hợp các tính năng nâng cao như recommendation system dựa trên user preferences, social features như follow users hay like/dislike reviews, và notification system cho activities mới. Do đang trong giai đoạn prototype, website cũng chưa có nhiều dữ liệu phim phong phú, chưa tích hợp API để auto-fetch movie information từ các nguồn như TMDB hay IMDb, và chưa có advanced search với multiple filters. Bên cạnh đó, hệ thống comment threading cho discussions còn đơn giản, chưa có real-time updates, và admin panel tuy functional nhưng chưa có dashboard analytics chi tiết về user engagement và content statistics.

Tổng thể, sản phẩm là một nền tảng vững chắc để phát triển thành một cộng đồng review phim hoàn chỉnh trong tương lai. Dự án thể hiện được khả năng vận dụng kiến thức về web development với PHP/MySQL, responsive design, và user experience design vào một sản phẩm thực tế có tính ứng dụng cao và tiềm năng phát triển thành một platform chuyên nghiệp cho cộng đồng yêu phim Việt Nam.

## **5.2. Kết luận**

Hiện nay, văn hóa điện ảnh và nhu cầu giải trí qua phim ảnh ngày càng phát triển mạnh mẽ trong cộng đồng người Việt, kéo theo sự gia tăng trong việc tìm kiếm thông tin, review và thảo luận về phim trực tuyến. Trong thời đại mạng xã hội và digital media, việc sở hữu một nền tảng review phim bằng tiếng Việt giúp người yêu phim dễ dàng kết nối với nhau, chia sẻ cảm nhận và khám phá những tác phẩm điện ảnh mới. Không khó để thấy rằng, các website review phim đang đóng vai trò quan trọng trong việc hướng dẫn lựa chọn phim, xây dựng cộng đồng thảo luận văn hóa điện ảnh và bảo tồn những đánh giá chất lượng từ góc nhìn người Việt. Nhờ có những nền tảng này, người dùng có thể dễ dàng tìm hiểu thông tin phim, đọc review chi tiết, tham khảo rating từ cộng đồng và tham gia discussions sâu sắc chỉ bằng vài thao tác đơn giản.

Việc xây dựng website Movie Review không chỉ mang lại tiện ích cho người yêu phim, mà còn là công cụ hỗ trợ phát triển văn hóa thảo luận điện ảnh Việt Nam một cách có hệ thống và chuyên nghiệp. Website giúp tổ chức thông tin phim rõ ràng, cập nhật review nhanh chóng và hỗ trợ tương tác trực tiếp giữa các thành viên cộng đồng, từ đó nâng cao chất lượng discussion và góp phần education về điện ảnh. Website Movie Review với Dark Theme hiện đại là một nền tảng tiêu biểu cho mô hình này, với giao diện đẹp mắt phù hợp với thẩm mỹ người trẻ, bố cục intuitive, và functionality đáp ứng thói quen sử dụng internet của người dùng hiện nay. Nội dung website được đầu tư kỹ lưỡng với database phim có đầy đủ thông tin, hệ thống review với rating system chuẩn, discussions organized theo phim, cùng với responsive design và clean interface để enhance user experience. Không chỉ vậy, website còn hỗ trợ chức năng admin management và user profile system, giúp cộng đồng có thể self-moderate và maintain quality content một cách hiệu quả.

Tóm lại, Website Movie Review không chỉ là một platform để đánh giá phim, mà còn là không gian văn hóa số nơi những người yêu điện ảnh có thể gặp gỡ, thảo luận và học hỏi lẫn nhau. Website này hứa hẹn sẽ là một công cụ community building mạnh mẽ, góp phần nâng cao appreciation cho nghệ thuật điện ảnh và khẳng định vị thế của cộng đồng review phim Việt Nam trong bối cảnh digital entertainment hiện đại. Với foundation technology vững chắc và vision rõ ràng, dự án có tiềm năng phát triển thành một destination chính cho movie enthusiasts tại Việt Nam.
