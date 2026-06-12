# 🎁 Dovanu_traukimas - Gift Drawing Application

A joyful web application for drawing names/gifts from a hat for Christmas and special occasions.

## ✨ Features

- **Self-Identification**: Users enter their name without creating an account
- **Drawing System**: 
  - **One-to-One**: Each participant gets a unique gift assignment
  - **Many-to-Many**: Random gift assignments, can repeat
  - **Name Drawing**: Participants draw another participant's name
- **User History**: Returning users see their previous draw results
- **Email Notifications**: Draw results sent to user's email with occasion details and AI jokes
- **Admin Dashboard**: Create and manage drawing occasions
- **Google Authentication**: Secure admin access via Google OAuth

## 🏗️ Project Structure

```
Dovanu_traukimas/
├── frontend/                 # React application
│   ├── public/
│   ├── src/
│   │   ├── components/       # Reusable components
│   │   ├── pages/            # Page components
│   │   ├── services/         # API services
│   │   ├── context/          # React Context for state management
│   │   ├── styles/           # Global styles
│   │   ├── App.js
│   │   ├── App.css
│   │   └── index.js
│   ├── package.json
│   └── .env.example
├── backend/                  # Flask application (future)
│   ├── app.py
│   ├── requirements.txt
│   └── config.py
└── docs/                     # Documentation
```

## 🚀 Getting Started

### Frontend Setup (Local Development)

#### Prerequisites
- **Node.js** 16+ 
- **npm** or **yarn**

#### Installation

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create `.env` file for Google OAuth configuration:
   ```bash
   cp .env.example .env
   ```
   Update with your Google OAuth credentials.

4. Start the development server:
   ```bash
   npm start
   ```
   The app will open at `http://localhost:3000`

5. Stop the server:
   ```bash
   Press Ctrl + C
   ```

### Backend Setup (Future Phase)

```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

## 🎨 Design Philosophy

- **Lively and Joyful**: Bright colors, playful animations, cheerful UI
- **Reserved Expression**: Clean, organized layout without clutter
- **Friendly Tone**: Relaxed language with occasional humor
- **Accessible**: Intuitive navigation for all users
- **Responsive**: Works on desktop, tablet, and mobile

## 📋 Technology Stack

- **Frontend**: React 18+, React Router, Axios, Context API
- **Backend**: Python Flask, Flask-SQLAlchemy, Flask-CORS
- **Database**: PostgreSQL
- **Authentication**: Google OAuth 2.0
- **Styling**: CSS3 with animations
- **Email**: Flask-Mail integration
- **AI Jokes**: OpenAI API integration

## 📝 Development Roadmap

### Phase 1: Frontend Foundation ✓
- [x] Project setup and structure
- [ ] Self-identification page
- [ ] Drawing page with card mechanics
- [ ] User history page
- [ ] Admin dashboard UI
- [ ] Responsive design

### Phase 2: Backend & Database
- [ ] Flask API setup
- [ ] PostgreSQL database schema
- [ ] Authentication endpoints
- [ ] Drawing logic implementation
- [ ] Email service integration

### Phase 3: Integration
- [ ] Connect frontend to backend
- [ ] Google OAuth integration
- [ ] Email notifications with AI jokes
- [ ] Testing and bug fixes

### Phase 4: Deployment
- [ ] Local development optimization
- [ ] Hosting platform selection and setup
- [ ] Production deployment

## 📧 Support

For questions or issues, please open an issue in the repository.

---

*Made with ❤️ for joyful gift exchanges*
