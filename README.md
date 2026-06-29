
# 🎤💼 Interact.ai: AI-Powered Job Interview Preparation Platform 📊

A job interview preparation platform powered by Vapi AI Voice agents. This project allows users to practice interview scenarios with AI-driven voice assistants and receive instant feedback based on their conversations.

## 🌐 Live Demo

Experience the application live: [Interact.ai Interview Platform](https://interview-platform-sand.vercel.app/)

## 🤖 Introduction

Built with Next.js for the user interface and backend logic, Firebase for authentication and data storage, styled with TailwindCSS and using Vapi's voice agents, Interact.ai helps users prepare for job interviews through AI-assisted mock interviews. The platform offers immediate feedback and provides a seamless experience for interview practice.

## 📱 Mobile App & Cross-Platform Strategy

We are developing a **React Native mobile application** to bring Interact.ai to iOS and Android devices. The mobile app will offer the same core features as the web platform, optimized for on-the-go interview practice.

### Cross-Platform Approach
- **Framework**: React Native for a single codebase across iOS and Android
- **State Management**: Redux Toolkit for consistent state across platforms
- **Backend**: Shared Firebase backend for seamless data sync
- **Voice Integration**: Vapi AI SDK for mobile voice capabilities
- **Development**: Expo for faster prototyping and OTA updates

This cross-platform strategy ensures users can:
- Start practice sessions on desktop and continue on mobile
- Access interview history and feedback across all devices
- Practice anytime, anywhere with a consistent user experience

## ✨ Features

- 🎙️ **AI Voice Interviews** - Practice with realistic Vapi AI voice agents
- 📊 **Instant Feedback** - Receive detailed analysis on your responses
- 🔐 **Authentication** - Secure login with Firebase (Email/Google)
- 📈 **Progress Tracking** - Monitor your improvement over time
- 🎯 **Role-Specific Interviews** - Practice for specific job roles
- 📱 **Cross-Platform** - Available on Web, iOS, and Android
- 💾 **History Storage** - Access all your past interviews
- 🎨 **Modern UI** - Clean, responsive design with TailwindCSS

## 🛠️ Tech Stack

### Web Platform
- **Frontend**: Next.js 14, React, TailwindCSS
- **Backend**: Next.js API Routes
- **Database**: Firebase Firestore
- **Authentication**: Firebase Auth
- **AI Voice**: Vapi AI
- **Hosting**: Vercel

### Mobile Platform (In Development)
- **Framework**: React Native with Expo
- **State Management**: Redux Toolkit
- **Navigation**: React Navigation
- **Backend**: Firebase (shared with web)
- **Voice**: Vapi AI SDK
- **Hosting**: Expo Application Services

## 📂 Project Structure

```

interact-ai/
├── components/          # Reusable React components
│   ├── ui/             # UI components
│   ├── interview/      # Interview-specific components
│   └── dashboard/      # Dashboard components
├── pages/
│   ├── api/            # Next.js API routes
│   │   ├── auth/       # Authentication endpoints
│   │   └── interview/  # Interview endpoints
│   ├── dashboard/      # User dashboard
│   ├── interview/      # Interview simulation
│   └── auth/           # Authentication pages
├── firebase/           # Firebase configuration
│   ├── config.js       # Firebase setup
│   ├── auth.js         # Auth methods
│   └── firestore.js    # Database operations
├── hooks/              # Custom React hooks
│   ├── useAuth.js      # Authentication hook
│   └── useInterview.js # Interview logic hook
├── utils/              # Utility functions
├── styles/             # Global styles
├── public/             # Static assets
└── mobile/             # React Native mobile app (coming soon)
├── src/
├── App.js
└── app.json

```

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- Firebase account
- Vapi AI account

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/interact-ai.git
cd interact-ai
```

2. Install dependencies

```bash
npm install
# or
yarn install
```

3. Set up environment variables
   Create a .env.local file in the root directory:

```env
NEXT_PUBLIC_FIREBASE_API_KEY=your_firebase_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_auth_domain
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_storage_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id
NEXT_PUBLIC_VAPI_API_KEY=your_vapi_api_key
```

4. Run the development server

```bash
npm run dev
# or
yarn dev
```

5. Open your browser
   Visit http://localhost:3000

📱 Mobile App Setup (Coming Soon)

The React Native mobile app is currently in development. To run the mobile app locally:

```bash
cd mobile
npm install
npx expo start
```

Scan the QR code with Expo Go app on your device.

🔧 Key API Endpoints

Endpoint Method Description
/api/auth/register POST User registration
/api/auth/login POST User login
/api/interview/start POST Start a new interview
/api/interview/feedback POST Get interview feedback
/api/interview/history GET Get user's interview history
/api/interview/save POST Save interview results

📊 Database Schema

Users Collection

```javascript
{
  uid: string,
  email: string,
  displayName: string,
  photoURL: string,
  createdAt: timestamp,
  preferences: {
    experienceLevel: string,
    targetRole: string
  }
}
```

Interviews Collection

```javascript
{
  id: string,
  userId: string,
  role: string,
  experienceLevel: string,
  questions: array,
  answers: array,
  feedback: object,
  score: number,
  createdAt: timestamp,
  duration: number
}
```

🎯 Roadmap

· Web platform launch
· AI voice integration with Vapi
· Firebase authentication
· Interview feedback system
· React Native mobile app (Q3 2026)
· Cross-platform data sync
· Advanced analytics dashboard
· Custom interview question generation
· Video interview support
· Enterprise features

🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (git checkout -b feature/AmazingFeature)
3. Commit your changes (git commit -m 'Add some AmazingFeature')
4. Push to the branch (git push origin feature/AmazingFeature)
5. Open a Pull Request

Development Guidelines

· Follow the existing code style
· Write meaningful commit messages
· Add tests for new features
· Update documentation as needed

🐛 Bug Reports & Feature Requests

Please use the GitHub Issues page to report bugs or suggest features.

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments

· Vapi AI for voice agent capabilities
· Firebase for backend services
· Next.js for the React framework
· TailwindCSS for styling
· React Native for mobile development

📞 Contact

· Project Maintainer: Your Name
· GitHub: @yourusername
· Twitter: @yourhandle
· Website: interact-ai.com

---

⭐ Show Your Support

If you found this project helpful, please give it a ⭐ on GitHub!

```

---

**📝 Instructions:**
1. Copy everything above (from ```markdown to ```)
2. Replace `yourusername`, `your.email@example.com`, `yourhandle`, and `interact-ai.com` with your actual details
3. Save as `README.md` in your project root
4. That's it! Ready to paste anywhere 🚀
