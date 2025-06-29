
# 🍽️ ShopTheRecipe — Installation Manual

**Group ID:** B11
**Course:** E-Commerce (SE-311)
**Group Members:**

* Syeda Fatima Jaffar (SE-22051)
* Diya Fatima (SE-22053)
* Hamnah Adnan (SE-22055)
* Fathima Raihaan Ihsan (SE-22100)

## 📌 Project Idea

A platform where users can select recipes, and all required ingredients are automatically added to their cart for delivery. It includes dietary filters and kitchen tool add-ons, solving the hassle of meal planning and grocery shopping in one user-friendly interface.


## 🎯 Scope

* **User Features:** Recipe selection, dietary filters (vegan, keto, etc.)
* **Backend:** Inventory and pricing, smart ingredient mapping, secure payment processing
* **Frontend:** Simple and intuitive UI for browsing and shopping
* **Target Audience:** Home cooks, people with dietary needs, and anyone looking for quick, sustainable meal solutions
* **Outcomes:** Simplified meal planning, reduced food waste, and quick delivery services
* **Limitations:** Limited to certain geographic areas initially and restricted real-time support


## 🖥️ System Requirements

* **Operating System:** Windows
* **Required Tools:**

  * [Git](https://git-scm.com/)
  * [Node.js (v18.x or v20.x)](https://nodejs.org/)
  * npm (comes with Node.js)
  * [VS Code](https://code.visualstudio.com/)
  * [XAMPP](https://www.apachefriends.org/index.html)


## 🚀 Installation Steps

### 1. Install XAMPP

* Download and install XAMPP.
* Start **Apache** and **MySQL** from the XAMPP Control Panel.

### 2. Clone the Repository

```bash
git clone https://github.com/diyafatimalilani/ShopTheRecipeNew.git
```

* Save it in the `XAMPP/htdocs` directory.
* Open the project in VS Code.

### 3. Setup the Database

* Visit [http://localhost/phpmyadmin/](http://localhost/phpmyadmin/)
* Create a new database named `shoptherecipe`.
* Import the `shoptherecipe.sql` file located in the project root.

### 4. Backend Setup

```bash
cd Backend
npm install --save-dev nodemon
npm install
npm install dotenv
npm install @stripe/react-stripe-js @stripe/stripe-js
npm install lucide-react
npm start
```

* Create a `.env` file inside the `Backend` folder with the following content:

```env
STRIPE_SECRET_KEY=sk_test_51RNAAX2VepmVN62YQ7pLKqleAjCguBvM5kbMZqu047706pVBKojNFL23zDKNijxEzH0jbDbyRtTQfOBTTBNVRIir00DT00abqL
```

### 5. Frontend Setup

```bash
cd Frontend
npm install
npm install axios react-router-dom react-icons
npm install @stripe/react-stripe-js @stripe/stripe-js
npm install lucide-react
npm start
```

* Create a `.env` file inside the `Frontend` folder with the following content:

```env
REACT_APP_API_URL=https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=AIzaSyAKtFfWj5ubr5VriffaBz43pOMEWQrn03Q
```


## 🌐 Access the Application

* **Frontend:** [http://localhost:3000/](http://localhost:3000/)
* **Backend:** [http://localhost:8081/](http://localhost:8081/)


## 🔐 Admin Login

* **Email:** `admin@shoptherecipe.com`
* **Password:** `admin123`


