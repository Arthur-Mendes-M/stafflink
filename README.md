# Stafflink

HR management system for small and medium-sized companies. Built as a university
project with a full Node.js backend and a vanilla JS/CSS frontend, covering the
entire employee lifecycle — from registration to attendance, vacations, payroll,
and internal news.

**Live demo:** [stafflink-kappa.vercel.app](https://stafflink-kappa.vercel.app)

---

## Tech stack

**Backend** *(this repository)*

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Multer](https://img.shields.io/badge/Multer-FF6C37?style=flat-square)

**Frontend** *(separate repository)*

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![SCSS](https://img.shields.io/badge/SCSS-CC6699?style=flat-square&logo=sass&logoColor=white)

---

## API routes

| Resource | Methods | Description |
|----------|---------|-------------|
| `/employees` | GET, POST, PUT, DELETE | Employee CRUD with photo upload |
| `/employees/photo/:name` | GET | Serve employee photo from database |
| `/attendance` | GET, POST, PUT, DELETE | Clock-in/out tracking per employee |
| `/vacation` | GET, POST, DELETE | Vacation request management |
| `/news` | GET, POST, PUT, DELETE | Internal company news with banner images |
| `/registers` | GET, POST | General registration records |
| `/tolken` | — | Authentication token management |

---

## Features

- Employee registration with optional photo upload (stored as binary in PostgreSQL)
- Attendance tracking with clock-in and clock-out per employee
- Vacation scheduling and history
- Internal news feed with image banners
- Token-based authentication
- Full CRUD for all resources

---

## Running locally

```bash
git clone https://github.com/Arthur-Mendes-M/stafflink
cd stafflink
npm install
# create a .env file with your DATABASE_URL and PORT
npm run dev
```

---

*Built by [Arthur Martins](https://github.com/Arthur-Mendes-M)*
