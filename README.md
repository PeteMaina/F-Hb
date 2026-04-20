# (c) 2026 Pete Fashion Hub. All rights reserved.


the transformation of this site began to a bigger and better software
# Pete Fashion Hub - Full-Stack E-Commerce Platform

> **Status:**  
> **Stack:** FastAPI + React + PostgreSQL + Material UI + Docker

e-commerce platform specializing in workwear, uniforms, and custom branding services.

---

## 🚀 Quick Start

```bash
# Clone and navigate
cd Pete Fashion Hub

# Setup environment
copy .env.example .env

# Start all services with Docker
docker-compose up --build

# Seed database (in new terminal)
docker-compose exec backend python scripts/seed_data.py
```

**Services:**
- 🎨 Frontend: http://localhost:3000
- 🔌 Backend API: http://localhost:8000
- 📚 API Docs: http://localhost:8000/docs
- 🗄️ PostgreSQL: localhost:5432
- 📦 MinIO: http://localhost:9001

---

## ✅ What's Built

### Backend (FastAPI)
✅ Complete REST API with JWT authentication  
✅ PostgreSQL database with SQLModel ORM  
✅ Product & Category management  
✅ Quote request system  
✅ Image upload functionality  
✅ Role-based access control (User/Admin)  
✅ Automatic API documentation (Swagger)  

### Frontend (React + Material UI)
✅ Custom premium theme with Pete Fashion Hub branding  
✅ Responsive navigation with mobile drawer  
✅ Shopping cart state management (Zustand)  
✅ Authentication flow setup  
✅ Product card component with hover effects  
✅ Landing page with hero & company info  
✅ Protected route system  

---

## 📁 Project Structure

```
Pete Fashion Hub/
├── backend/           # FastAPI application
│   ├── app/
│   │   ├── api/v1/   # API endpoints
│   │   ├── core/     # Config, database, security
│   │   ├── models/   # SQLModel database models
│   │   └── schemas/  # Pydantic validation
│   └── scripts/      # Database seeding
├── frontend/         # React application
│   └── src/
│       ├── components/  # Reusable UI components
│       ├── pages/       # Route pages
│       ├── services/    # API client
│       ├── store/       # State management
│       └── theme/       # MUI customization
├── docker-compose.yml
├── Makefile          # Development shortcuts
└── .env.example
```

---

## 🎯 Key Features

### For Customers
- Browse products by category
- Request custom bulk quotes
- Shopping cart & checkout
- Order tracking
- User account management

### For Admins
- Product management dashboard
- Quote request handling
- Order processing
- Inventory tracking
- Customer management

---

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
|-------|------------|---------|
| Frontend | React 18 | UI library |
| UI Components | Material UI v5 | Design system |
| State | Zustand | Global state |
| Routing | React Router v6 | Navigation |
| Backend | FastAPI | REST API |
| Database | PostgreSQL 15 | Data storage |
| ORM | SQLModel | Database modeling |
| Auth | JWT + bcrypt | Security |
| DevOps | Docker Compose | Containerization |

---

## 📖 API Documentation

Once running, visit http://localhost:8000/docs for interactive API documentation.

### Main Endpoints

**Authentication**
- `POST /api/v1/auth/register` - User registration
- `POST /api/v1/auth/login` - Login (returns JWT)
- `GET /api/v1/auth/me` - Current user profile

**Products**
- `GET /api/v1/products` - List products (with filters)
- `GET /api/v1/products/{id}` - Product details
- `POST /api/v1/products` - Create product *(Admin)*

**Quotes**
- `POST /api/v1/quotes` - Submit quote request
- `GET /api/v1/quotes/my-quotes` - User's quotes
- `GET /api/v1/admin/quotes` - All quotes *(Admin)*

---

## 🔐 Default Credentials

After seeding the database:

```
Email: admin@petefashionhub.com
Password: admin123
```

⚠️ **Change these in production!**

---

## 📋 Development Commands

Using the Makefile:

```bash
make up              # Start all services
make down            # Stop all services
make logs            # View all logs
make migrate         # Run database migrations
make seed            # Seed database with sample data
make test-backend    # Run backend tests
make test-frontend   # Run frontend tests
```

---

## 🗺️ Roadmap

### Phase 1: Core Features (IN PROGRESS)
- [x] Backend API foundation
- [x] Frontend structure
- [ ] Complete shop page with filters
- [ ] Product detail page
- [ ] Multi-step quote builder
- [ ] Auth pages (login/register)

### Phase 2: Admin Dashboard
- [ ] Product management DataGrid
- [ ] Quote management interface
- [ ] Analytics dashboard
- [ ] Order processing

### Phase 3: Polish
- [ ] Email notifications
- [ ] Image optimization
- [ ] Loading states & animations
- [ ] Toast notifications

### Phase 4: Production
- [ ] Automated testing (Pytest + Jest)
- [ ] CI/CD pipeline (GitHub Actions)
- [ ] Cloud deployment
- [ ] Performance optimization

---

## 🎨 Design Philosophy

**Premium Aesthetics**
- Custom Material UI theme matching Pete Fashion Hub brand
- Abril Fatface font for headings (from original design)
- Smooth micro-animations on all interactions
- Professional gradient backgrounds
- Custom shadows for depth

**Mobile-First**
- Responsive navigation with drawer
- Touch-friendly buttons (44px minimum)
- Optimized layouts for all screen sizes

**Developer Experience**
- Type-safe API with Pydantic
- Automatic API documentation
- Hot reload for both frontend & backend
- Docker for consistent environments

---

## 🧪 Testing

```bash
# Backend tests
cd backend
pytest

# Frontend tests
cd frontend
npm test

# E2E tests (TODO)
npm run test:e2e
```

---

## 📦 Deployment

### Recommended Stack
- **Frontend:** Vercel or Netlify
- **Backend:** Railway or Render
- **Database:** Neon or Supabase (PostgreSQL)
- **Images:** AWS S3 or Cloudinary

### Environment Variables
See `.env.example` for all required variables.

---

## 🤝 Contributing

This is currently a portfolio/learning project. Feel free to fork and adapt for your own use!

---

## 📄 License

MIT License - See LICENSE file for details

---

## 🎓 Skills Demonstrated

This project showcases:
- ✅ Full-stack development (React + FastAPI)
- ✅ RESTful API design
- ✅ Database modeling (PostgreSQL)
- ✅ JWT authentication & authorization
- ✅ State management (Zustand)
- ✅ Material UI theming & customization
- ✅ Docker containerization
- ✅ Responsive design
- ✅ Security best practices

---


---

**Built with ❤️ as a portfolio project demonstrating modern full-stack development practices.**



