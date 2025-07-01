# MERN-TEST - Mujtaba Qureshi  
**Web-Based Developer Store Platform**

## CANDIDATE DETAILS  
**NAME:** Mujtaba Qureshi  
**EMAIL:** qmujtaba09@gmail.com  
**LAST INTERVIEW:** {To be scheduled}

---

## SUBMISSION DETAILS  
**START DATE:** {YYYY-MM-DD}  
**SUBMISSION DEADLINE:** {YYYY-MM-DD + 7 days}

> **NOTE:** We will monitor the submission date from your commit history. We will only review commits made on or before the submission date.  
> **NOTE:** Please provide a **separate README** or a **dedicated section** describing how to run the project locally.

---

## PROJECT OVERVIEW  
Build a **full-stack MERN application** for developers to create and manage their own **digital product store**.

As part of this assignment, you are expected to:
- Design and build your own **custom REST API** using **Node.js/Express and MongoDB**
- Create a **React.js** (or **Next.js**) frontend to interact with your APIs
- Implement **authentication**, **file uploads**, and **role-based logic**

---

## CORE SCOPE (BUILD API YOURSELF — NO EXTERNAL FAKESTORE OR BOILERPLATE)

### 1. **Authentication (JWT-based)**  
- `POST /auth/register` — Register user with email, password, role (buyer/seller)  
- `POST /auth/login` — Login and return JWT token  
- Use bcrypt for hashing  
- Protect all routes with middleware  
- Optional: token refresh logic

### 2. **User Roles & Profiles**  
- Roles: `buyer`, `seller`, `admin`  
- `GET /users/me` — Fetch current user profile  
- `PUT /users/me` — Update profile (name, bio, etc.)  

### 3. **Digital Product Management**  
- `POST /products` — Seller adds a product with title, price, description, file upload (PDF/ZIP)  
- `GET /products` — Public product list  
- `GET /products/:id` — Product detail  
- `DELETE /products/:id` — Seller deletes own product  
- File uploads can be stored locally or via Cloudinary  

### 4. **Product Purchase Flow (Mock Checkout)**  
- `POST /orders` — Buyer purchases a product  
- `GET /orders` — Buyer sees purchased products  
- Prevent re-purchasing of same product  
- No payment gateway needed — simulate success  

### 5. **Admin Management**  
- `GET /admin/users` — List all users  
- `PATCH /admin/users/:id/ban` — Ban/unban user  
- `GET /admin/products` — View/delete any product

---

## WEB SCREENS & FEATURES

### 1. Login / Signup Screens
- Form validation  
- Store token and redirect upon success  

### 2. Seller Dashboard
- Create products  
- View uploaded products  
- Delete product  
- View total downloads per product

### 3. Buyer Dashboard
- View purchased products  
- Download files  
- Show purchase date  

### 4. Public Marketplace
- Home page showing all products  
- Filter by price, category, or tag  
- Click to view product details  

### 5. Admin Panel
- View all users  
- Ban/unban accounts  
- View all products and remove violations  

---

## FRONT-END REQUIREMENTS (React.js)

1. **Routing**  
   - Use `react-router-dom` for navigation  
   - Pages: `/login`, `/signup`, `/marketplace`, `/dashboard`, `/admin`  

2. **State Management**  
   - Use Redux, Zustand, or Context API  
   - Handle auth and user data  

3. **API Layer**  
   - Axios with interceptors  
   - Handle 401 and API errors cleanly  

4. **Component Reusability**  
   - Build reusable inputs, modals, cards  

5. **Responsive Design**  
   - Use TailwindCSS, Bootstrap, or plain SCSS  

---

## BACKEND REQUIREMENTS (MANDATORY)

1. **Node.js + Express.js API**  
2. **MongoDB/Mongoose** for data modeling  
3. **Authentication using JWT**  
4. **RESTful Routes for all features**  
5. **Role-based access control middleware**  
6. **File uploads (PDF, ZIP)**  
7. **Error handling and validation**  
8. **.env-based config (JWT_SECRET, DB_URI, etc.)**

---

## CODE QUALITY MANAGEMENT

- Modular backend folder structure (e.g., `routes/`, `controllers/`, `models/`)  
- Use ESLint or Prettier if possible  
- Include `README.md` with clear run instructions  
- Optional: Include Swagger/OpenAPI doc for backend  

---

## CODE MANAGEMENT

1. **Git Commits**  
   - Commit regularly with clear messages  
2. **Branches**  
   - Feature branches preferred  
3. **Pull Requests**  
   - Submit via GitHub if collaborating  

---

## HOW TO RUN THE APPLICATION LOCALLY

1. **Clone the Repo**
   ```bash
   git clone https://github.com/mujtabaqureshi2/mern-test.git
   cd mern-test
