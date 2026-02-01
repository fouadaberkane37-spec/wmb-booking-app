[README.md](https://github.com/user-attachments/files/24988001/README.md)
# Groupe WMB - Appointment Booking System

A modern, fully-functional appointment booking system for home services with calendar management, built with vanilla HTML, CSS, and JavaScript.

🔗 **[Live Demo](https://your-username.github.io/wmb-booking-system/)**

## 🌟 Features

### Authentication
- Secure login system
- Session management (Remember me)
- Auto-redirect for authenticated users
- Demo credentials for testing

### Booking System
- **Duration Selection**: 60, 120, or 180 minute appointments
- **Smart Scheduling**: 
  - Daily limit: 480 minutes (8 hours)
  - Weekly limit: 2400 minutes (40 hours)
  - 30-minute buffer between appointments
  - Work hours: 7:00 AM - 6:00 PM
- **Multi-Service Selection**:
  - Window cleaning (exterior/interior)
  - Gutter cleaning (exterior/interior)
  - Soft wash
- **Salesperson Management**: Add/remove team members dynamically
- **Real-time Availability**: See available time slots instantly

### Calendar System
- **Full Calendar View**: Navigate through months (2026-2030)
- **Appointment Details**: Click any appointment for full information
- **Statistics Dashboard**: 
  - Total appointments
  - Today's schedule
  - Weekly overview
  - Monthly hours
- **Export Functionality**: Download appointments as CSV

### Design
- 🎨 Professional blue color theme
- 📱 Fully responsive (mobile, tablet, desktop)
- ✨ Smooth animations and transitions
- 🎯 Clean, modern UI/UX

## 🚀 Quick Start

### Demo Credentials
```
Email: demo@groupewmb.com
Password: demo123
```

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/wmb-booking-system.git
   cd wmb-booking-system
   ```

2. **Open in browser**
   ```bash
   # Simply open index.html in your browser
   open index.html
   # or
   python -m http.server 8000
   # then visit http://localhost:8000
   ```

3. **Login and explore!**

## 📁 Project Structure

```
wmb-booking-system/
├── index.html                      # Login page (entry point)
├── appointment-booking-wmb.html    # New booking form
├── appointments-calendar.html      # Calendar view
└── README.md                       # Documentation
```

## 🌐 GitHub Pages Deployment

This project is configured for GitHub Pages deployment:

1. **Push to GitHub**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

2. **Enable GitHub Pages**
   - Go to repository Settings
   - Navigate to Pages
   - Source: Deploy from main branch
   - Root directory: / (root)
   - Save

3. **Access your site**
   - Your site will be live at: `https://your-username.github.io/wmb-booking-system/`

## 💻 Technology Stack

- **HTML5**: Semantic markup
- **CSS3**: Custom styling with CSS variables, animations
- **Vanilla JavaScript**: No frameworks, pure JS
- **Fonts**: Google Fonts (Crimson Pro, DM Mono)

## 🎨 Color Palette

```css
--cream: #faf8f3
--charcoal: #2a2a2a
--sage: #6b8cb3 (primary blue)
--terracotta: #5c7ad6 (accent blue)
--soft-grey: #e8e4dc
--deep-green: #4a5f7b (dark blue)
```

## 📱 Browser Support

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

## 🔧 Customization

### Change Demo Credentials
Edit `index.html` line ~252:
```javascript
if (email === 'YOUR_EMAIL' && password === 'YOUR_PASSWORD') {
```

### Add Salespeople
Default salespeople are defined in `appointment-booking-wmb.html` line ~1013:
```javascript
salespeople: ['John Smith', 'Sarah Johnson', 'Michael Brown', 'Emily Davis']
```

### Modify Services
Services are defined in `appointment-booking-wmb.html` around line 647-665

### Adjust Time Limits
Constants in `appointment-booking-wmb.html` line ~1001:
```javascript
const BUFFER_TIME = 30;      // minutes
const DAILY_LIMIT = 480;     // minutes per day
const WEEKLY_LIMIT = 2400;   // minutes per week
const WORK_START = 7;        // 7 AM
const WORK_END = 18;         // 6 PM
```

## 📊 Features Roadmap

### Current (v1.0)
- ✅ Full booking system
- ✅ Calendar management
- ✅ User authentication
- ✅ Export functionality

### Future Enhancements
- ⏳ Backend integration
- ⏳ Database persistence
- ⏳ Email notifications
- ⏳ Payment processing
- ⏳ Multi-user accounts
- ⏳ SMS reminders
- ⏳ Customer portal
- ⏳ Analytics dashboard

## 🚨 Important Notes

### Current Limitations
- **No Data Persistence**: Appointments are demo data only
- **No Email Confirmation**: Requires backend integration
- **Single Login**: One demo account only
- **Client-Side Only**: All logic runs in browser

### For Production Use
To make this production-ready, you'll need:

1. **Backend Server**
   - Node.js + Express
   - Python + Flask/Django
   - PHP + Laravel

2. **Database**
   - MySQL / PostgreSQL
   - MongoDB
   - Firebase / Supabase

3. **Email Service**
   - SendGrid
   - Mailgun
   - AWS SES

4. **Authentication**
   - JWT tokens
   - OAuth integration
   - Password hashing (bcrypt)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👥 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 Contact

**Groupe WMB**
- Website: [groupewmb.com](https://groupewmb.com)
- Email: info@groupewmb.com

## 🙏 Acknowledgments

- Font families: [Google Fonts](https://fonts.google.com/)
- Icons: Unicode emoji characters
- Design inspiration: Modern SaaS applications

---

Made with ❤️ for Groupe WMB

**⭐ Star this repo if you find it helpful!**
