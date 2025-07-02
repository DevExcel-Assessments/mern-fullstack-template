# MERN-TEST - Mujtaba Qureshi  
**DevNest – Developer Course SaaS Platform**

## CANDIDATE DETAILS  
**NAME:** Mujtaba Qureshi  
**EMAIL:** qmujtaba09@gmail.com  
**LAST INTERVIEW:** {To be scheduled}

---

## SUBMISSION DETAILS  
**TOTAL DAYS: 4**

**TOTAL HOURS: 16**

**START DATE:** **2025-07-03**

**SUBMISSION DEADLINE:** **2025-07-10**



> **NOTE:** All features must be commit-time-tracked.  
> **NOTE:** Include `.env.example` and detailed run instructions in `README.md`.  
> **NOTE:** All API endpoints must be built and documented by you.

---

## PROJECT OVERVIEW  
Build a **developer-focused SaaS platform** where users can **create**, **sell**, and **enroll** in video-based technical courses. Each user may register as a `mentor` or `learner` and should have access only to their permitted features.

This project simulates a real-world product like **Udemy / Teachable** but scoped down for a 7-day full-stack challenge.

---

## CORE SCOPE

### 🔐 Authentication
- `POST /auth/register`  
- `POST /auth/login`  
- Roles: `mentor`, `learner`  
- Use JWT + bcrypt  
- Role-based protection middleware  
- Store token securely (localStorage or cookie)

---

### 📹 Course Creation (Mentor only)
- `POST /courses`  
- `GET /courses/my`  
- Course Fields:
  - Title, Description, Category
  - Upload video (max 100MB, 5 minutes)
  - Auto-generate thumbnail (10s timestamp)
- Validate file format + duration
- Store videos on disk or Cloudinary/S3

---

### 📘 Course Catalog (Public)
- `GET /courses` — Paginated list  
- `GET /courses/:id` — Full details + demo player  
- Filter by tag or category  
- Only enrolled users can watch full video  

---

### 💸 Enroll & Payment
- `POST /orders` — Enroll using mock Stripe  
- `GET /orders/my` — View enrolled courses  
- Prevent duplicate enrollment  
- Bonus: Store Stripe PaymentIntent ID

---

### 🎥 Video Streaming & Security
- Users can stream video if:
  - ✅ Authenticated
  - ✅ Enrolled in the course  
- Don't expose full video URL (e.g., presigned or internal proxy route)
- Must prevent direct file download without access

---

### 📊 Dashboard (Role Based)
#### Mentor:
- Revenue (mock)
- Total sales per course
- Edit/delete their own courses

#### Learner:
- List of enrolled courses
- Continue watching

---

## FRONTEND (React or Next.js)

- Auth pages: login, register  
- Course catalog + filter  
- Course detail page + video player (demo for public)  
- Enrolled dashboard  
- Mentor dashboard for uploads and stats  
- Mobile Responsive  
- TailwindCSS preferred  

---

## BACKEND (MANDATORY)

- Express or NestJS  
- MongoDB (with Mongoose)  
- JWT-based authentication  
- Role middleware  
- File upload (Multer or Cloudinary SDK)  
- Thumbnail generation (ffmpeg or ffmpeg.wasm)  
- Stream protection (resumable or range requests)  
- Stripe (test key mode only)

---

## BONUS FEATURES (Optional)
- Course ratings & reviews  
- Video chapters (timestamps)  
- FFMPEG-based video compression  
- Graphs using Chart.js or Recharts  
- Unit tests for auth & video endpoints  

---

## CODE QUALITY REQUIREMENTS

- Modular backend (`routes`, `controllers`, `services`)  
- Reusable front-end components  
- Graceful error messages everywhere  
- `.env.example` file included  
- `DECISION_LOG.md` required  
  - What problems you solved  
  - Where you used docs/AI  
  - What you would improve if given more time  

---

## HOW TO RUN LOCALLY

```bash
# Backend
cd server
npm install
npm run dev

# Frontend
cd client
npm install
npm run dev
