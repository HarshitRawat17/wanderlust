# 🌍 WanderLust – Travel Listing Platform

A full-stack travel listing and destination exploration web application that allows users to discover places, create and manage listings, upload images, view locations on interactive maps, and share experiences through reviews and ratings. Built with a focus on clean architecture, security, and scalability.

---

## 🚀 Live Demo

**[https://wanderlust-j31l.onrender.com/listings](https://wanderlust-j31l.onrender.com/listings)**

---

## 📖 Project Overview

WanderLust provides a comprehensive platform where users can explore travel destinations and share detailed listings. Each listing includes images, descriptions, pricing, location details, and user reviews. Authenticated users can create, edit, and delete their own listings, while visitors can browse and review destinations.

The application follows the **MVC (Model-View-Controller)** architecture to ensure better organization, maintainability, and scalability. Third-party services are integrated for cloud image storage and map visualization, along with secure authentication and authorization.

---

## ✨ Key Features

- 🔐 **User Authentication** – Secure Signup, Login, and Logout
- 🧑‍💼 **Role-based Authorization** – Protected routes and ownership validation
- 🏠 **Listing Management** – Create, Edit, and Delete travel listings
- 🖼️ **Cloud Image Storage** – Seamless image uploads via Cloudinary
- ⭐ **Review & Rating System** – Users can rate and review listings
- 🗺️ **Interactive Maps** – Location visualization using Mapbox
- 🛡️ **Secure Sessions** – Session-based authentication with Passport.js
- 📱 **Responsive Design** – Optimized for mobile, tablet, and desktop
- ✅ **Data Validation** – Server-side validation using Joi
- 💬 **Flash Messages** – Real-time user feedback

---

## 🛠️ Tech Stack

### Frontend
- **HTML5** – Semantic markup
- **CSS3** – Modern styling
- **Bootstrap** – Responsive UI framework
- **EJS** – Embedded JavaScript templates

### Backend
- **Node.js** – JavaScript runtime
- **Express.js** – Web application framework

### Database
- **MongoDB** – NoSQL database
- **Mongoose** – MongoDB object modeling
- **MongoDB Atlas** – Cloud database hosting

### Third-Party Services
- **Cloudinary** – Cloud-based image storage and management
- **Mapbox** – Interactive maps and geolocation
- **Passport.js** – Authentication middleware
- **Express-Session** – Session management
- **Connect-Flash** – Flash message middleware

### Deployment
- **Render** – Cloud application hosting

---

## 📁 Project Structure

```
WanderLust/
│
├── controllers/        # Application logic and request handlers
├── models/            # MongoDB schemas (Listing, User, Review)
├── routes/            # Express route definitions
├── views/             # EJS template files
│   ├── layouts/       # Page layouts
│   ├── listings/      # Listing-related views
│   └── users/         # User authentication views
├── public/            # Static assets
│   ├── css/          # Stylesheets
│   ├── js/           # Client-side JavaScript
│   └── images/       # Static images
├── utils/             # Utility functions and helpers
├── middleware/        # Custom middleware (auth, validation)
├── cloudConfig.js     # Cloudinary configuration
├── app.js            # Main application entry point
├── .env              # Environment variables (not in repo)
└── package.json      # Project dependencies
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v16+)
- MongoDB Atlas account or local MongoDB
- Cloudinary account
- Mapbox account
- npm or yarn


## 🔐 Authentication & Security

- ✅ **Password Hashing** – Passwords are securely hashed before storage
- 🔑 **Session-based Auth** – Using Passport.js for authentication
- 🛡️ **Protected Routes** – Authorization middleware for secure endpoints
- 👤 **Ownership Validation** – Only listing owners can update or delete
- 🔒 **Session Security** – Secure session handling with express-session

---

## 🧪 Validation & Error Handling

- ✅ **Server-side Validation** – Using Joi schema validation
- 🎯 **Centralized Error Handling** – Custom error handling middleware
- 💬 **Flash Messages** – User-friendly feedback for actions
- 🐛 **Error Logging** – Comprehensive error tracking

---

## 🗺️ API Routes

### Listings
| Method | Route | Description | Auth Required |
|--------|-------|-------------|---------------|
| GET | `/listings` | Get all listings | No |
| GET | `/listings/new` | Show create form | Yes |
| POST | `/listings` | Create new listing | Yes |
| GET | `/listings/:id` | Show listing details | No |
| GET | `/listings/:id/edit` | Show edit form | Yes (Owner) |
| PUT | `/listings/:id` | Update listing | Yes (Owner) |
| DELETE | `/listings/:id` | Delete listing | Yes (Owner) |

### Reviews
| Method | Route | Description | Auth Required |
|--------|-------|-------------|---------------|
| POST | `/listings/:id/reviews` | Create review | Yes |
| DELETE | `/listings/:id/reviews/:reviewId` | Delete review | Yes (Owner) |

### Authentication
| Method | Route | Description |
|--------|-------|-------------|
| GET | `/signup` | Show signup form |
| POST | `/signup` | Register new user |
| GET | `/login` | Show login form |
| POST | `/login` | Authenticate user |
| GET | `/logout` | Logout user |

---

## 🌱 Future Enhancements

- [ ] ❤️ Wishlist / Favorites feature
- [ ] 🔍 Advanced search and filtering options
- [ ] 👤 User profile pages with listing history
- [ ] 📅 Booking and reservation system
- [ ] 🔔 Real-time notifications
- [ ] 💬 Direct messaging between users
- [ ] 📊 Analytics dashboard for listing owners
- [ ] 🌐 Multi-language support
- [ ] 📱 Mobile app (React Native)
- [ ] 💳 Payment gateway integration

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Open a Pull Request

---

## 📜 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Cloudinary** – For image hosting and management
- **Mapbox** – For interactive map integration
- **Bootstrap** – For responsive UI components
- **MongoDB Atlas** – For cloud database hosting
---

<div align="center">

</div>
