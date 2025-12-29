
---

# Automatic SMS Scheduler

## 📌 Project Overview

**Automatic SMS Scheduler** is a full-stack application designed to create, manage, and execute **SMS campaigns** in a scheduled and automated manner. The platform allows users to define SMS campaigns, control when they run, and manage recipient lists (shoppers) to whom messages are sent. The system uses **queue-based processing** to ensure reliable and scalable message delivery.

---

## 🚀 Key Features

* Create and manage **SMS campaigns**
* Schedule campaigns to run **on demand or at a specific time**
* Add and manage **shoppers (recipients)** using email IDs
* Asynchronous SMS processing using **Redis-based queues**
* Secure authentication using **JWT**
* Scalable and production-ready backend architecture

---

## 🧠 Tech Stack

### Backend

* Node.js (Express)
* MongoDB
* BullMQ (Redis)
* JWT Authentication

### Frontend

* React (Vite)
* Tailwind CSS

---

## 🖥️ Backend Setup

This service handles campaign creation, scheduling logic, queue processing, and data persistence.

### How to Run the Backend

1. Clone the repository and navigate to the backend directory
   `cd datmanBackend`

2. Install dependencies
   `npm install`

3. Create a `.env` file and configure environment variables

   PORT=your_port
   MONGOURI=your_mongodb_uri
   REDIS_HOST=your_redis_host
   REDIS_PORT=your_redis_port
   REDIS_PASSWORD=your_redis_password
   REDIS_HOST_URL=your_redis_host_url
   JWT_SECRET=your_jwt_secret
   MAIL=your_email
   MAILPASS=your_email_password

4. Start the backend server
   `cd src && nodemon index.js`

### Important Notes

* Ensure the `.env` file is correctly configured
* **Redis must be running** for queue-based campaign processing

---

## 🖥️ Frontend Setup

The frontend provides an interface to create SMS campaigns, schedule executions, and manage shoppers.

### How to Run the Frontend

1. Navigate to the frontend directory
   `cd datmanFrontend`

2. Install dependencies
   `npm install`

3. Create a `.env` file and add the API base URL

   VITE_API_BASE_URL=your_base_api_url

4. Start the development server
   `npm run dev`

---

## 🔄 Application Flow

1. Create an SMS campaign
2. Add shoppers (recipients) using email IDs
3. Schedule the campaign or trigger it manually
4. Jobs are queued using BullMQ
5. SMS messages are processed and sent asynchronously

---

## 📈 Future Improvements

* Campaign analytics and delivery reports
* Retry handling for failed SMS jobs
* Role-based access control
* Support for additional notification channels

---

## 📄 License

This project is for learning and internal use. Licensing can be added as required.

---
