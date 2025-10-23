<<<<<<< HEAD
# mind-coach-ai
=======
# Mind Coach AI Agent

A full-stack personal mental wellness assistant that provides AI-driven supportive conversations, mood tracking, and daily wellness tips.

## Features

- 🤖 **AI Chat-based Mind Coach**: Empathetic conversations powered by GPT-4o
- 📊 **Mood Tracker**: Daily mood logging with sentiment analysis
- 💡 **Daily Wellness Tips**: Personalized affirmations and wellness advice
- 📝 **Journal & Reflection**: Secure private diary with AI prompts
- 🔐 **Authentication**: Email/password + Google OAuth with JWT

## Tech Stack

### Frontend
- React (Vite) + TypeScript
- TailwindCSS + ShadCN UI
- Zustand (State Management)
- Framer Motion (Animations)
- Chart.js/Recharts (Data Visualization)

### Backend
- FastAPI (Python)
- PostgreSQL (Supabase)
- OpenAI GPT-4o API
- HuggingFace Transformers
- JWT Authentication

### Deployment
- Frontend: Vercel
- Backend: Railway
- Database: Supabase

## Project Structure

```
mind-coach-ai/
├── frontend/          # React frontend
├── backend/           # FastAPI backend
└── README.md
```

## Getting Started

### Prerequisites
- Node.js 16+ and npm
- Python 3.8+
- PostgreSQL (or Supabase account)

### Environment Variables

Create `.env` files in both frontend and backend directories:

**Backend (.env)**
```
DATABASE_URL=postgresql://...
OPENAI_API_KEY=your_openai_key
JWT_SECRET=your_jwt_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
```

**Frontend (.env)**
```
VITE_API_URL=http://localhost:8000
VITE_GOOGLE_CLIENT_ID=your_google_client_id
```

### Installation & Development

1. **Backend Setup**
```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

2. **Frontend Setup**
```bash
cd frontend
npm install
npm run dev
```

## API Endpoints

- `POST /auth/register` - User registration
- `POST /auth/login` - User login
- `GET /auth/google` - Google OAuth
- `POST /chat` - AI conversation
- `GET/POST /mood` - Mood tracking
- `GET/POST/PUT/DELETE /journal` - Journal entries
- `GET /tip` - Daily wellness tips

## License

MIT License
>>>>>>> f0d8f6a (Initial commit for mind-coach-ai project)
