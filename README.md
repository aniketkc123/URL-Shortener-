
URL Shortener

A simple and efficient URL shortener built using Node.js, MongoDB, and React.js.

Features

Shorten long URLs into concise links.

Track click analytics for each shortened URL.

Secure and scalable backend with MongoDB.

User-friendly React frontend for easy interaction.

API support for developers to generate short links.

Tech Stack

Frontend: React.js

Backend: Node.js, Express.js

Database: MongoDB (Mongoose ODM)

Run it locally :

1. Clone the repository.

2.Install dependencies for both frontend and backend:

cd server npm install cd client npm install

3.reate a .env file in the root directory and add the following:

MONGODB_URI=your-mongodb-uri
PORT=your-port-number

Start the development server:
-Server npm start 
-Client npm start

The URL Shortener Web Application will be running on http://localhost:your-port-number



Deployment: Vercel (Frontend), Render (Backend), MongoDB Atlas (Database)

Installation

Prerequisites

Ensure you have the following installed:

Node.js

MongoDB

Clone the Repository

git clone https://github.com/yourusername/url-shortener.git
cd url-shortener

Backend Setup

cd server
npm install

Configure Environment Variables

Create a .env file in the backend/ directory and add the following:

PORT=5000
MONGO_URI=your_mongodb_connection_string
BASE_URL=http://localhost:5000

Start the backend server:

npm start

Frontend Setup

cd ../client
npm install

Configure Environment Variables

Create a .env file in the frontend/ directory and add:

REACT_APP_API_URL=http://localhost:5000

Start the frontend server:

npm start

API Endpoints

Shorten a URL

POST /api/shorten

{
  "longUrl": "https://example.com"
}

Response:

{
  "shortUrl": "http://localhost:5000/abcd123"
}

Redirect a Shortened URL

GET /:shortUrl Redirects the user to the original long URL.

Deployment

Backend

Deploy on Render:

Add your environment variables to the hosting platform.

Deploy using GitHub integration or manual push.






