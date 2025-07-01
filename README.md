# MERN-TEST - Mujtaba Qureshi  
**Web E-Commerce Application**

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
Build a **web-based E-Commerce application** using **React.js** and optionally Node.js/Express/MongoDB for full-stack capability. As a mid-level MERN developer with 2 years of experience, you're expected to build a complete, real-world platform, including custom authentication, store/product modules, dashboards, and dynamic UX. Do not rely entirely on AI — your reasoning should be visible in the project structure and commit messages.

### Extended Scope (Real-World Challenge)
1. **JWT Authentication** (Login, Register, Role-based access)  
2. **Create Developer Store Profile**  
3. **Upload Digital Products (PDFs, ZIPs, etc.)**  
4. **Home Page (Products Listing + Filters + Categories)**  
5. **Product Detail Page (with mock reviews)**  
6. **Add to Cart, Cart Listing & Mock Checkout**  
7. **Buyer Dashboard (Purchased Items)**  
8. **Seller Dashboard (Analytics with Chart.js)**  
9. **Admin Dashboard (User/Product Management)**  
10. **Mobile-Responsive Design**

> Optional: Add a static AI-chat interface to simulate "Contact the Seller"

---

## FAKESTOREAPI INTEGRATION  
If you do not want to create a custom backend, you may use [FakeStoreAPI](https://fakestoreapi.com/docs) for product/cart logic only. However, authentication, uploads, and dashboards must be implemented manually.

1. **Authentication**  
   - Prefer custom login/signup using JWT & bcrypt.

2. **Products**  
   - Or use: `GET https://fakestoreapi.com/products`  
   - `GET https://fakestoreapi.com/products/{id}`  

3. **Carts**  
   - `POST /carts`, `GET /carts`, `DELETE /carts/{id}`

---

## WEB SCREENS & FEATURES

### 1. Login Screen
- **Custom API**: `POST /auth/login`  
- **JWT Token Storage**: localStorage or HttpOnly cookies  
- **Redirect**: To Home Page on success  

### 2. Sign Up Screen
- Custom or mocked  
- Role selection: `buyer`, `seller`  
- After signup: redirect to login or auto-login  

### 3. Forgot Password
- Static with mock success message  

### 4. Home Page (Products + Filters)
- Grid layout  
- Filter by tag/category/price  
- Click to go to product detail  

### 5. Product Detail Page
- Static or mocked reviews  
- Downloadable preview or files (if owned)  
- "Add to Cart" button  

### 6. Cart Page
- View items  
- Remove items  
- Mock checkout (updates buyer dashboard)  

### 7. Dashboards
- **Buyer**: Purchased products, download buttons  
- **Seller**: Uploaded products, product analytics using Chart.js  
- **Admin**: List all users, block/unblock seller accounts  

### 8. Mobile-Responsive Design
- TailwindCSS or Bootstrap recommended  

---

## FRONT-END REQUIREMENTS (React.js or Next.js)

1. **Framework**  
   - Use Create React App or Next.js  
   - Use **react-router-dom** or Next.js routing  

2. **State Management**  
   - Use Redux, Zustand, or Context API  
   - Auth token & cart state managed centrally  

3. **API Integration**  
   - Axios or Fetch with interceptors  
   - Handle 401, 403 errors properly  

4. **Structure & Modularity**  
   - Pages, Components, Services, Stores, Constants, etc.  

5. **Advanced UI**  
   - Reusable modal, dropdown, table, file upload components  

---

## OPTIONAL BACKEND (FULL MERN)

If you implement your own backend:

- **NestJS or ExpressJS** (Node-based)  
- **MongoDB** for users, products, purchases  
- **JWT Auth** for protected routes  
- **Multer/Cloudinary** for file uploads  
- **Product search/filter endpoints**  
- **Admin API** for dashboard controls  

---

## CODE QUALITY MANAGEMENT

- Follow ESLint rules  
- DRY and reusable logic  
- Descriptive comments where needed  
- Handle edge cases (empty products, invalid tokens, expired carts)

---

## CODE MANAGEMENT

1. **Git Workflow**  
   - Clear, atomic commits  
   - Use branches like `feature/cart`, `feature/auth`, etc.

2. **Pull Requests**  
   - Summarize key changes  

3. **Commit Log**  
   - Helps us understand your thought process (vs AI-generated code)

---

## HOW TO RUN THE APPLICATION LOCALLY

1. **Clone the Repo**
   ```bash
   git clone https://github.com/mujtabaqureshi2/devnest.git
   cd devnest
