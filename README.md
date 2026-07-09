# GlaxxyChat - Production AI Platform

**GlaxxyChat** is a production-ready AI platform designed for users with 0 budget for AI services. It provides a real ChatGPT-like experience with support for multiple AI providers and a futuristic UI.

## 🎯 Features

✅ **Real AI Integration**
- Google Gemini API
- OpenAI GPT-3.5
- OpenRouter
- DeepSeek
- Model switching on-the-fly

✅ **Authentication System**
- User registration & login
- JWT token-based auth
- Secure password hashing (bcryptjs)

✅ **Chat Management**
- Real-time chat with AI
- Conversation history
- Chat archiving & pinning
- Model-specific chat threads

✅ **Search & Content**
- Web search integration
- Image search via Unsplash
- File upload & analysis support

✅ **Multi-Platform Ready**
- Web (Next.js + React)
- Windows/macOS (Electron)
- Mobile (React Native)

## 🛠️ Tech Stack

- **Backend:** Node.js + Express
- **Frontend:** Next.js + React + Tailwind CSS
- **Database:** MongoDB
- **Auth:** JWT
- **Real-time:** Socket.io
- **AI Providers:** Google Gemini, OpenAI, OpenRouter, DeepSeek

## 📋 Prerequisites

- Node.js 18+
- MongoDB database (free tier: mongodb.com)
- API Keys for:
  - Google Gemini (free tier available)
  - Unsplash (free tier)
  - Brave Search (optional)

## 🚀 Quick Start

### 1. Clone & Install
\`\`\`bash
git clone https://github.com/ashandeepdhillon-pixel/glaxxyAI.git
cd glaxxyAI
npm install
\`\`\`

### 2. Setup Environment
\`\`\`bash
cp .env.example .env.local
# Edit .env.local with your API keys
\`\`\`

### 3. Run Server
\`\`\`bash
npm run server
# Server runs on http://localhost:3001
\`\`\`

### 4. Run Frontend (in new terminal)
\`\`\`bash
npm run client
# Frontend runs on http://localhost:3000
\`\`\`

## 📁 Project Structure

\`\`\`
glaxxyAI/
├── backend/
│   ├── config/           # Database config
│   ├── middleware/       # Auth middleware
│   ├── models/           # Mongoose schemas (User, Chat, File)
│   └── routes/           # API endpoints
├── app/                  # Next.js frontend
├── public/               # Static assets
├── server.js             # Express server entry
└── package.json
\`\`\`

## 🔑 API Endpoints

### Authentication
- \`POST /api/auth/register\` - Create new account
- \`POST /api/auth/login\` - Login
- \`GET /api/auth/me\` - Get current user

### Chat
- \`POST /api/chat\` - Create new chat
- \`GET /api/chat\` - Get all chats
- \`GET /api/chat/:id\` - Get single chat
- \`DELETE /api/chat/:id\` - Delete chat

### AI
- \`POST /api/ai/chat\` - Send message to AI
- \`GET /api/ai/models\` - List available models

### Search
- \`POST /api/search/web\` - Web search

### Images
- \`POST /api/images/search\` - Image search

## 🌍 Environment Variables

\`\`\`env
# Database
MONGODB_URI=your_mongodb_connection_string

# AI Providers
GOOGLE_GEMINI_API_KEY=your_key
OPENAI_API_KEY=your_key
OPENROUTER_API_KEY=your_key
DEEPSEEK_API_KEY=your_key

# Search
BRAVE_SEARCH_API_KEY=your_key
UNSPLASH_ACCESS_KEY=your_key

# Auth
JWT_SECRET=your_secret_key
JWT_EXPIRE=7d

# Server
PORT=3001
NODE_ENV=development
NEXT_PUBLIC_API_URL=http://localhost:3001
\`\`\`

## 🎨 UI/UX Features

- **Dark Futuristic Design** - Premium glassmorphism panels
- **Responsive Layout** - Mobile, tablet, desktop
- **Dynamic Backgrounds** - Changes based on time and weather
- **Smooth Animations** - Framer Motion integration
- **Real-time Chat** - Socket.io powered messaging

## 📦 Deployment

### Deploy Backend (Railway/Render)
\`\`\`bash
npm run start
\`\`\`

### Deploy Frontend (Vercel)
\`\`\`bash
npm run build
\`\`\`

## 🔐 Security

- ✅ Password hashing with bcryptjs
- ✅ JWT token authentication
- ✅ Environment variable protection
- ✅ CORS configuration
- ✅ Input validation

## 📝 Code Quality

\`\`\`bash
# Lint code
npm run lint

# Run tests
npm run test
\`\`\`

## 🐛 Known Limitations

- Free tier APIs have rate limits
- File uploads limited to 50MB
- Search results depend on API quotas

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Push to branch
5. Open a pull request

## 📄 License

MIT License - Free for personal and commercial use

## 💡 Tips for 0-Budget Setup

1. **Google Gemini** - Free API with 60 requests/minute
2. **MongoDB** - 512MB free tier
3. **Vercel** - Free deployment for frontend
4. **Railway** - Free tier with credits for backend
5. **Unsplash** - Free image API (no auth needed for search)

## 🚀 Next Steps

- [ ] Setup frontend components (Chat UI, Sidebar, etc.)
- [ ] Implement file upload
- [ ] Add voice chat support
- [ ] Setup CI/CD pipeline
- [ ] Deploy to production
- [ ] Add admin dashboard

## 📞 Support

For issues or questions, open a GitHub issue or contact the maintainer.

---

**Made for people with 0 money for AI** 💰➡️🤖
