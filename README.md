# SkillBridge 🚀
### AI-Powered Interview Preparation Platform

**SkillBridge** is an AI-powered interview preparation platform that helps job seekers prepare for technical interviews through personalized interview reports, skill-gap analysis, and structured preparation roadmaps.

Instead of following a generic preparation plan, users can generate interview preparation reports based on their target role and resume or self-description.

## ✨ Features

- **User Authentication** — Secure registration and login using JWT-based authentication and password hashing.
- **AI-Powered Interview Preparation** — Generate personalized interview preparation reports using Google's Gemini API.
- **Resume-Based Analysis** — Use resume uploads or a self-description to provide context for preparation.
- **Skill-Gap Analysis** — Identify relevant skills and areas that need improvement.
- **Interview Questions** — Generate technical and behavioral interview questions.
- **Personalized Roadmap** — Get a structured, multi-day preparation plan.
- **Dashboard & History** — Access previously generated interview reports.
- **PDF Generation** — Generate downloadable PDF documents using Puppeteer.
- **Database Integration** — Store user information and interview reports in MongoDB.

## 🛠️ Tech Stack

| Layer | Technologies |
|---|---|
| Frontend | React, Vite, Sass, Axios |
| Backend | Node.js, Express.js |
| Database | MongoDB, Mongoose |
| Authentication | JWT, bcrypt |
| AI Integration | Google Gemini API |
| PDF Generation | Puppeteer |
| Development Tools | Git, GitHub, ESLint, npm |

## 🏗️ Project Structure

```text
SkillBridge/
├── Backend/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── middlewares/
│   │   ├── models/
│   │   ├── routes/
│   │   └── services/
│   ├── server.js
│   ├── package.json
│   └── .env.example
├── Frontend/
│   ├── public/
│   ├── src/
│   │   ├── features/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── package.json
│   └── vite.config.js
└── README.md
```

## ⚙️ Getting Started

### Prerequisites

Make sure you have the following installed:

- Node.js and npm
- A MongoDB database (local or MongoDB Atlas)
- A Google Gemini API key

### 1. Clone the repository

```bash
git clone https://github.com/shauryat6324534/SkillBridge.git
cd SkillBridge
```

### 2. Configure the backend

```bash
cd Backend
npm install
```

Create a `.env` file in the `Backend` directory using `.env.example` as a reference.

```env
PORT=3000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_strong_jwt_secret
GOOGLE_GENAI_API_KEY=your_gemini_api_key
```

Replace the placeholder values with your own credentials. Never commit your actual `.env` file or API keys.

Start the backend:

```bash
npm run dev
```

If the development script is unavailable, check `Backend/package.json` for the available start command.

### 3. Configure the frontend

Open a second terminal:

```bash
cd Frontend
npm install
npm run dev
```

Open the local URL displayed by Vite, usually:

**http://localhost:5173**

Ensure the backend is running on port `3000` and that the frontend's API configuration points to the correct backend URL.

## 🔄 How It Works

1. **Authenticate:** Register or log in to your account.
2. **Provide Context:** Upload a resume or describe your background and target role.
3. **Generate a Report:** The backend processes the request and uses the Gemini API to generate personalized preparation content.
4. **Analyze Skills:** Review the skill-gap breakdown and interview questions.
5. **Follow the Roadmap:** Use the preparation plan to organize your learning.
6. **Access Reports:** Retrieve saved reports from the dashboard and generate PDF documents.

## 🔐 Security

- Password hashing with bcrypt.
- JWT-based authentication.
- HttpOnly authentication cookies.
- Environment variables for sensitive configuration.
- Git ignore rules for environment files and installed dependencies.

**Security note:** Keep API keys, database credentials, and production secrets private. Configure appropriate CORS, cookie, and database access policies before deploying the application.

## 🧪 Verification

The project has been tested locally for the following workflows:

- User login and authentication cookie exchange.
- AI-powered interview report generation.
- Report retrieval and dashboard history.
- PDF generation endpoint.
- Frontend linting and production build.

Actual results may depend on your environment, API credentials, and database configuration.

## 🔮 Future Improvements

- Mock interview sessions with real-time feedback.
- Interview performance tracking and progress analytics.
- More AI provider options.
- Personalized learning resources for identified skill gaps.
- Cloud deployment and automated testing.

## 👨‍💻 Author

**Shaurya Binjola**

Computer Science & Engineering Student

[GitHub Profile](https://github.com/shauryat6324534)

---

*SkillBridge — Bridge the gap between your current skills and your career goals.*