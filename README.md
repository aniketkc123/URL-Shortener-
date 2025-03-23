# 🚀 URL Shortener

A **simple and efficient** URL shortener built using **Node.js, MongoDB, and React.js**. Convert long URLs into short, shareable links instantly!

---

## 🌟 Features
✔️ Shorten long URLs into concise links.
✔️ Track **click analytics** for each shortened URL.
✔️ Secure and **scalable backend** with MongoDB.
✔️ **User-friendly** React frontend for easy interaction.
✔️ **API support** for developers to generate short links.

---

## 🛠 Tech Stack
- 🎨 **Frontend:** React.js, Tailwind CSS
- 🏗 **Backend:** Node.js, Express.js
- 🗄 **Database:** MongoDB (Mongoose ODM)
- 🔒 **Authentication (Optional):** JWT

---

## 🚀 Run it Locally

### 📌 Prerequisites
Ensure you have the following installed:
- [✅ Node.js](https://nodejs.org/)
- [✅ MongoDB](https://www.mongodb.com/)

### 📥 Clone the Repository
```sh
git clone https://github.com/yourusername/url-shortener.git
cd url-shortener
```

### 📦 Install Dependencies
For both frontend and backend:
```sh
cd server 
npm install 
cd ../client 
npm install
```

### ⚙️ Configure Environment Variables
Create a `.env` file in the root directory and add the following:
```
MONGODB_URI=your-mongodb-uri
PORT=your-port-number
```

### ▶️ Start the Development Server
For the backend:
```sh
cd server
npm start
```
For the frontend:
```sh
cd client
npm start
```

🎉 The URL Shortener Web Application will be running on `http://localhost:your-port-number`

---

## 🌎 Deployment
- **Frontend:** [Vercel](https://vercel.com/)
- **Backend:** [Render](https://render.com/)
- **Database:** [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)

---

## 📥 Installation

### 🖥 Backend Setup
```sh
cd server
npm install
```

#### 🛠 Configure Environment Variables
Create a `.env` file in the `backend/` directory and add the following:
```
PORT=5000
MONGO_URI=your_mongodb_connection_string
BASE_URL=http://localhost:5000
```

Start the backend server:
```sh
npm start
```

### 🎨 Frontend Setup
```sh
cd ../client
npm install
```

#### 🛠 Configure Environment Variables
Create a `.env` file in the `frontend/` directory and add:
```
REACT_APP_API_URL=http://localhost:5000
```

Start the frontend server:
```sh
npm start
```

---

## 🔗 API Endpoints

### 🔹 Shorten a URL
**POST** `/api/shorten`
```json
{
  "longUrl": "https://example.com"
}
```
**Response:**
```json
{
  "shortUrl": "http://localhost:5000/abcd123"
}
```

### 🔹 Redirect a Shortened URL
**GET** `/:shortUrl`
Redirects the user to the original long URL.

---

## 🚀 Deployment Guide
### 🔹 Backend
Deploy on **Render**:
- Add your environment variables to the hosting platform.
- Deploy using GitHub integration or manual push.

---

💡 **Contributions are welcome!** Feel free to fork the repository and submit a pull request. 🛠️

