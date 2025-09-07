# AI-Powered Fitness Trainer App

A comprehensive, AI-driven fitness application built with the MERN stack (MongoDB, Express.js, React, Node.js) and Next.js. This application provides personalized workout experiences with real-time form analysis and adaptive training programs.

![Fitness App](https://img.shields.io/badge/React-18.2-blue) ![Next.js](https://img.shields.io/badge/Next.js-13.4-black) ![Node.js](https://img.shields.io/badge/Node.js-18.0-green) ![MongoDB](https://img.shields.io/badge/MongoDB-6.0-green) ![License](https://img.shields.io/badge/License-MIT-yellow)

## ✨ Features

- **🤖 AI-Powered Form Analysis**: Real-time exercise form correction using computer vision
- **🎯 Personalized Workout Plans**: Adaptive training programs based on your goals and progress
- **📊 Progress Tracking**: Comprehensive analytics and visualizations of your fitness journey
- **🏋️ Exercise Library**: Extensive collection of exercises with detailed instructions
- **📱 Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **🔐 Secure Authentication**: JWT-based user authentication and authorization
- **⚡ Real-time Feedback**: Instant guidance during workouts

## 🛠️ Technology Stack

### Frontend
- **Next.js 13** with App Router
- **React 18** with Hooks and Context API
- **Tailwind CSS** for styling
- **Framer Motion** for animations
- **TensorFlow.js** for client-side AI

### Backend
- **Node.js** with Express.js
- **MongoDB** with Mongoose ODM
- **JWT** for authentication
- **bcryptjs** for password hashing

### AI Components
- **MediaPipe** for pose estimation
- **Custom TensorFlow models** for form analysis
- **Python Flask API** for advanced processing (optional)

## 📦 Installation

### Prerequisites
- Node.js (v18 or higher)
- MongoDB (v6 or higher)
- npm or yarn

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/AnugrahMassey/ai-fitness-trainer.git
   cd ai-fitness-trainer
   ```

2. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Environment Setup**
   
   Create a `.env` file in the backend directory:
   ```env
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/fitness-app
   JWT_SECRET=your_jwt_secret_here
   JWT_EXPIRE=7d
   NODE_ENV=development
   ```
   
   Create a `.env.local` file in the frontend directory:
   ```env
   NEXT_PUBLIC_API_URL=http://localhost:5000
   NEXT_PUBLIC_AI_SERVICE_URL=http://localhost:5001
   ```

5. **Start the development servers**
   
   Backend (Terminal 1):
   ```bash
   cd backend
   npm run dev
   ```
   
   Frontend (Terminal 2):
   ```bash
   cd frontend
   npm run dev
   ```

6. **Access the application**
   Open [http://localhost:3000](http://localhost:3000) in your browser

## 🚀 Usage

1. **Create an Account**: Sign up with your email and basic information
2. **Set Your Goals**: Define your fitness objectives and preferences
3. **Start a Workout**: Choose from recommended routines or create your own
4. **Get AI Feedback**: Use your camera for real-time form analysis
5. **Track Progress**: Monitor your improvements over time

## 🔧 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/users/register` | User registration |
| POST | `/api/users/login` | User authentication |
| GET | `/api/exercises` | Get exercise library |
| POST | `/api/workouts` | Create workout plan |
| GET | `/api/workouts/history` | Get workout history |
| POST | `/api/ai/analyze` | Submit exercise for form analysis |

## 🏗️ Project Structure

```
ai-fitness-trainer/
├── backend/
│   ├── controllers/     # Route controllers
│   ├── models/          # MongoDB models
│   ├── routes/          # API routes
│   ├── middleware/      # Custom middleware
│   ├── utils/           # Helper functions
│   └── server.js        # Express server
├── frontend/
│   ├── app/             # Next.js app directory
│   ├── components/      # Reusable components
│   ├── hooks/           # Custom React hooks
│   ├── contexts/        # React contexts
│   ├── lib/             # Utility libraries
│   └── public/          # Static assets
└── docs/                # Documentation
```

## 🤖 AI Integration

The application uses several AI technologies:

1. **Pose Estimation**: MediaPipe for detecting body landmarks
2. **Form Analysis**: Custom algorithms to evaluate exercise technique
3. **Recommendation Engine**: Machine learning for personalized workouts

To enable full AI functionality, you may need to set up additional services for more complex processing.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/AnugrahMassey/AI-Fitness-Trainer-App/issues).

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 Support

If you have any questions or need help, please:

1. Check the [documentation](docs/)
2. Search existing [issues](https://github.com/AnugrahMassey/AI-Fitness-Trainer-App/issues)
3. Create a new issue with detailed information

## 🙏 Acknowledgments

- MediaPipe for pose estimation technology
- TensorFlow.js team for browser-based ML
- The MERN stack community for excellent resources and tools

---

<div align="center">
Made with ❤️ and JavaScript
</div>
