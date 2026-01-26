# 💬 Real-Time Chat App (MERN + Socket.io)

A full-stack real-time chat platform powered by the MERN stack and WebSocket technology, delivering instant, reliable communication with seamless user presence awareness. Featuring secure JWT-based authentication and reactive UI built with Tailwind CSS, the app supports smooth one-on-one messaging, dynamic online/offline tracking, and fully synchronized chat experience—ideal for modern social or collaborative environments.

## 🔍 Key Features

- **🧱 Full-Stack MERN Architecture**

  Built with MongoDB, Express.js, React, and Node.js to ensure seamless backend-frontend integration with scalable infrastructure.

- **🔐 JWT-Based Authentication**

  Secure authentication system with JSON Web Tokens (JWT), featuring token validation middleware, route protection, and user session persistence across refreshes. Uses cookies over localStorage for better security, and keeps client state in sync for seamless, refresh-resistant login experience.

- **⚡ Real-Time Messaging with Socket.io**
  
  Leverages WebSockets via Socket.io for instantaneous message delivery, typing indicators, online status, and room-based handling. Enhances engagement by mimicking real-world chat responsiveness.
  
- **🎨 Clean & Responsive UI**
  
  Crafted with Tailwind CSS and DaisyUI, the interface is responsive by design, polished across devices, and consistent in look, feel, and behavior. Visual feedback and hover interactions enhance usability and flow.
  
- **🌐 Global State Management with Zustand**
  
  Uses Zustand to manage shared state with minimal boilerplate. Keeps the app fast and predictable without Redux or heavy context, making the codebase easier to maintain and extend.

## 📁 Project Structure

```bash
mern-chat-app/
├── backend/                         # Backend - Node.js + Express + MongoDB
│   ├── controllers/                 # Request handlers (auth, messages, etc.)
│   ├── db/                          # MongoDB connection setup
│   ├── middleware/                  # Middleware (JWT auth, error handlers)
│   ├── models/                      # Mongoose schemas (User, Message)
│   ├── routes/                      # Express API route definitions
│   ├── socket/                      # Socket.io event handlers and setup
│   ├── utils/                       # Utility functions
│   └── server.js                    # Entry point for the backend server
│
├── src/                             # Frontend - React + Zustand + Socket.io client
│   ├── components/                  # Reusable UI components (sidebar, message containers, etc.)
│   ├── pages/                       # Pages (Login, Register, Chat, etc.)
│   ├── context/                     # React context for global state
│   ├── hooks/                       # Custom React hooks
│   ├── zustand/                     # Zustand store setup
│   ├── utils/                       # Utility helpers
│   ├── assets/                      # Static assets
│   ├── App.jsx                      # Main app component
│   └── main.jsx                     # App entry point
│
├── package.json                     # Frontend dependencies and scripts
├── .env                             # Environment variables
├── .gitignore                       # Files/folders to be ignored by Git
└── README.md                        # Project overview and documentation
```

## 🛠️ Tech Stack

- **Backend**: `Node.js`, `Express.js`, `MongoDB`, `Mongoose`

- **Frontend**: `React`, `React Router`

- **UI & Styling**: `Tailwind CSS`, `DaisyUI`, `react-hot-toast`

- **WebSocket**: `Socket.io`

- **State Management**: `Zustand`

- **Authentication**: `JWT`, `bcrypt`

## ⚙️ Dependencies

- **Node.js** — Required for backend and frontend
   👉 [Download Node.js](https://nodejs.org/en/download)

- **MongoDB** — Database for storing users and messages
   👉 [Download MongoDB](https://www.mongodb.com/try/download/community)

## 🚀 Setup & Usage

1. **Clone the repository**

   ```bash
   git clone https://github.com/HenryyyLI/mern-chat-app.git
   cd mern-chat-app
   ```

2. **Configure environment variables**

   ```bash
   # Create .env file in root directory with:
   MONGODB_URI=mongodb://localhost:27017/chat-app
   JWT_SECRET=your_jwt_secret_key
   PORT=5000
   NODE_ENV=development
   ```

3. **Install dependencies**

   ```bash
   # Install backend dependencies
   cd backend
   npm install
   
   # Install frontend dependencies
   cd ..
   npm install
   ```

4. **Start the application**

   ```bash
   # Start backend server (from backend directory)
   cd backend
   npm start
   
   # Start frontend dev server (from root directory, in new terminal)
   npm run dev
   ```

## 🌐 Deployment

👉 **Live Demo**: https://chat-app-prod-xvv5.onrender.com

## 📧 Contact

Henry Li - [GitHub Profile](https://github.com/HenryyyLI)

Project Link: [https://github.com/HenryyyLI/mern-chat-app](https://github.com/HenryyyLI/mern-chat-app)

---

⭐ If you find this project useful, please consider giving it a star!
