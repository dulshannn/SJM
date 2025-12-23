# Secure Jewellery Management System (SJM)

A premium, secure web application for managing jewellery business operations with a luxury dark theme and OTP-based authentication.

## Developer Information

**Developed by:** K. M. Nethmi Sanjalee
**Organization:** ALL TECHNOLOGY
**Email:** kokiladulshan021@gmail.com

## Features

### Authentication Module
- Luxury dark-themed login interface
- Two-factor authentication with OTP verification
- 5-minute OTP expiry with countdown timer
- Secure session management
- OTP logging and tracking

### Customer Management Module
- Complete CRUD operations for customers
- Advanced search and filtering
- Responsive table with pagination
- Status management (Active/Inactive)
- Data validation and error handling

### Profile Management Module
- View user profile information
- Edit profile details
- Secure password change with validation
- Real-time password matching indicator

### Design Features
- Luxury dark theme with gold accents (#d4af37)
- Multiple layered video backgrounds
- Premium glassmorphism effects
- Responsive design
- Smooth animations and transitions
- Professional typography (Segoe UI)

## Technology Stack

- **Framework:** Laravel 12.x
- **PHP Version:** 8.2+
- **Database:** SQLite
- **Frontend:** Blade Templates, Vanilla JavaScript, Custom CSS
- **Security:** Bcrypt hashing, CSRF protection, OTP verification

## Quick Start

### Prerequisites
- PHP 8.2+ with required extensions (PDO, SQLite, XML, DOM, cURL)
- Composer
- Node.js and npm

### Installation

```bash
# 1. Install dependencies
composer install
npm install

# 2. Setup environment
cp .env.example .env
php artisan key:generate

# 3. Create database
touch database/database.sqlite

# 4. Run migrations
php artisan migrate:fresh --seed

# 5. Build assets
npm run build

# 6. Start server
php artisan serve
```

### Default Login Credentials
- **Email:** admin@sjm.com
- **Password:** password123

The OTP code will be logged in the Laravel logs at `storage/logs/laravel.log`

## Documentation

For detailed setup instructions, features documentation, and customization guide, please refer to `SETUP_GUIDE.md`.

## Project Structure

```
app/
├── Http/Controllers/
│   ├── AuthController.php          # Authentication & OTP
│   ├── CustomerController.php      # Customer CRUD
│   ├── ProfileController.php       # Profile management
│   └── DashboardController.php     # Dashboard
├── Models/
│   ├── User.php
│   ├── Customer.php
│   └── OtpLog.php
resources/
├── views/
│   ├── layouts/app.blade.php       # Main layout
│   ├── auth/                       # Login & OTP pages
│   ├── customers/                  # Customer management
│   ├── profile/                    # Profile pages
│   └── dashboard.blade.php
database/
└── migrations/
    ├── create_customers_table.php
    └── create_otp_logs_table.php
```

## Security Features

- Bcrypt password hashing (12 rounds)
- Time-based OTP with expiry
- CSRF token protection
- Server-side input validation
- XSS protection
- SQL injection prevention
- Secure session handling

## Module Responsibilities

**K. M. Nethmi Sanjalee** is responsible for:
- Authentication system (Frontend & Backend)
- OTP verification system
- Customer management module (Frontend & Backend)
- Profile management (Frontend & Backend)
- Luxury dark theme implementation
- Security implementation

## Support

For questions, issues, or support:
- Developer: K. M. Nethmi Sanjalee
- Organization: ALL TECHNOLOGY
- Email: kokiladulshan021@gmail.com

## License

This is proprietary software developed for ALL TECHNOLOGY.

---

**Built with Laravel** - The PHP Framework for Web Artisans
