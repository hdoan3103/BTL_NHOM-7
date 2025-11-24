# System Patterns - Movie Review Website

## MVC Architecture

### Controller Pattern
```php
// Base Controller class trong core/Controller.php
class Controller {
    protected $pdo;  // Database connection
    
    public function __construct($pdo) {
        $this->pdo = $pdo;
    }
}

// Specific Controllers extend base
class MovieController extends Controller {
    public function detail($id) {
        // Business logic here
    }
}
```

### Model Pattern
```php
// Base Model class trong core/Model.php  
class Model {
    protected $pdo;
    protected $table;
    
    // Common CRUD operations
}

// Specific Models extend base
class Movie extends Model {
    protected $table = 'movies';
    
    // Movie-specific methods
}
```

### View Pattern
- PHP templates trong `views/` folder
- Layout system với header/footer shared
- Data passing từ controller qua variables

## Database Patterns

### Table Structure
- **users**: id, username, email, password, full_name, role, created_at
- **movies**: id, title, description, director, cast, release_year, poster, genre_id, slug, created_by, created_at
- **genres**: id, name, description, slug, created_at
- **reviews**: id, movie_id, user_id, title, content, rating, status, created_at
- **discussions**: id, title, content, movie_id, user_id, status, created_at

### Relationship Patterns
- **One-to-Many**: Genre -> Movies, User -> Reviews, Movie -> Reviews
- **Foreign Keys**: Đảm bảo data integrity
- **Status fields**: 'active', 'inactive', 'approved', 'pending' cho moderation

## Routing Patterns

### URL Structure
```
/movie/123           -> MovieController::detail(123)
/movie/detail/123    -> MovieController::detail(123)  
/discussion/create   -> DiscussionController::create()
/admin/movies        -> AdminController::movies()
```

### URLHelper Pattern
```php
// Centralized URL generation
URLHelper::movieDetail($id)     // /movie/detail/123
URLHelper::adminMovies()        // /admin/movies
URLHelper::poster($filename)    // /uploads/posters/image.jpg
```

## Security Patterns

### Input Validation
```php
// SQL Injection prevention
$stmt = $pdo->prepare("SELECT * FROM movies WHERE id = ?");
$stmt->execute([$id]);

// XSS prevention
echo htmlspecialchars($user_input);
```

### Authentication Pattern
```php
// Session-based auth
if (!isset($_SESSION['user_id'])) {
    header('Location: /login');
    exit;
}

// Role-based access
if ($_SESSION['role'] !== 'admin') {
    // Access denied
}
```

## File Organization Patterns

### MVC Separation
- **Controllers**: Handle HTTP requests, business logic
- **Models**: Database interactions, data validation
- **Views**: HTML templates, presentation logic

### Asset Organization
- **CSS/JS**: Trong `assets/` folder
- **Uploads**: Trong `uploads/posters/` với proper permissions
- **Layouts**: Shared header/footer trong `views/layouts/`

## Error Handling Patterns

### Database Errors
```php
try {
    $pdo = new PDO($dsn, $user, $pass);
} catch(PDOException $e) {
    echo "Database error: " . $e->getMessage();
}
```

### Form Validation
```php
$errors = [];
if (empty($title)) {
    $errors[] = "Tiêu đề không được để trống";
}
if (!empty($errors)) {
    // Display errors to user
}
```

## Code Style Patterns

### Vietnamese Language
- Comments bằng tiếng Việt
- Error messages bằng tiếng Việt  
- Variable names tiếng Anh nhưng clear meaning

### Naming Conventions
- **Classes**: PascalCase (MovieController)
- **Methods**: camelCase (getByIdWithDetails)
- **Variables**: snake_case cho database fields, camelCase cho PHP vars
- **Files**: PascalCase cho classes, lowercase cho views
