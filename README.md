# AutomaticSMSScheduler

# Backend

This project is built using **Node.js (Express)** with **MongoDB** for data storage and **BullMQ (Redis)** for queue processing.

## 🚀 How to Run the Project

1️⃣ Clone the project and navigate into the directory:  
`cd datmanBackend`  

2️⃣ Install dependencies:  
`npm install`  

3️⃣ Create a `.env` file and add the required environment variables:  

PORT=your_port 
MONGOURI=your_mongodb_uri
REDIS_HOST=your_redis_host
REDIS_PORT=your_redis_port
REDIS_PASSWORD=your_redis_password 
REDIS_HOST_URL=your_redis_host_url 
JWT_SECRET=your_jwt_secret 
MAIL=your_email 
MAILPASS=your_email_password

4️⃣ Start the project:  
`cd src && nodemon index.js`  

---

### ✅ Important Notes:
- Ensure the **.env** file is correctly set up before running the project.
- Redis must be running for queue processing.

---

# Frontend

This project is built using **React (Vite)** and **Tailwind CSS** for styling. It serves as the frontend for the SMS scheduling system.

## How to Run the Project

# 1️⃣ Clone the project and navigate into the directory
cd datmanFrontend

# 2️⃣ Install dependencies
npm install

# 3️⃣ Create a .env file and add the base API URL
echo "VITE_API_BASE_URL=your_base_api_url" > .env

# 4️⃣ Start the project
npm run dev

