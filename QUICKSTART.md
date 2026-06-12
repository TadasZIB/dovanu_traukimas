# 🎁 Dovanu_traukimas - Quick Start Guide

## 📋 What Was Just Created

Your React frontend is now ready with:

✅ **3 Pages**:
- 🎯 **Identification Page** - Users enter/select their name
- 🎴 **Drawing Page** - Interactive card drawing with email collection
- 📜 **History Page** - View user's draw history

✅ **Complete Design System**:
- Festive color palette (Red, Turquoise, Gold, Green)
- Smooth animations (card flip, bounce, fade-in)
- Fully responsive mobile layout
- Joyful but reserved aesthetic

✅ **State Management**:
- UserContext for user identification
- DrawingContext for drawing history

## 🚀 Get Started Locally

### Step 1: Prerequisites
Make sure you have installed:
- **Node.js 16+** - Download from https://nodejs.org/
- **npm** or **yarn** - Comes with Node.js

### Step 2: Install Dependencies
```bash
cd frontend
npm install
```

This downloads all React packages (~500MB, takes 2-5 minutes depending on internet).

### Step 3: Start Development Server
```bash
npm start
```

The app automatically opens at `http://localhost:3000`

### Step 4: Make Changes
- Edit files in `frontend/src/`
- The browser auto-refreshes when you save changes
- Open browser DevTools (F12) to test on mobile sizes

### Step 5: Stop Server
```bash
Press Ctrl + C
```

## 📁 Project Structure

```
frontend/
├── public/
│   └── index.html           # Main HTML file
├── src/
│   ├── pages/
│   │   ├── IdentificationPage.jsx    # Name entry
│   │   ├── IdentificationPage.css
│   │   ├── DrawingPage.jsx           # Card drawing
│   │   ├── DrawingPage.css
│   │   ├── HistoryPage.jsx           # History view
│   │   └── HistoryPage.css
│   ├── context/
│   │   ├── UserContext.jsx           # User state
│   │   └── DrawingContext.jsx        # Drawing state
│   ├── styles/
│   │   └── globals.css               # Design system & animations
│   ├── App.js                        # Main router
│   ├── App.css
│   └── index.js                      # React entry point
├── .env.example                      # Environment template
├── package.json                      # Dependencies
└── .gitignore

backend/
└── README.md                         # Future Flask setup
```

## 🎨 Colors Used

- **Primary Red**: `#FF6B6B` - Main buttons, headers
- **Secondary Turquoise**: `#4ECDC4` - Alternative actions
- **Gold**: `#FFD93D` - Highlights, accents
- **Christmas Green**: `#6BCB77` - Success states
- **Light backgrounds**: Soft pink and turquoise gradients

## 🔧 Next Steps (When Ready)

### Phase 2: Backend Setup
1. Create Flask API with routes
2. Setup PostgreSQL database
3. Implement drawing logic
4. Configure email service
5. Setup Google OAuth

### Phase 3: Integration
1. Connect frontend to backend API
2. Add Google login
3. Implement email notifications with AI jokes
4. Testing and deployment

## 🐛 Troubleshooting

**"Port 3000 already in use"**
```bash
# Use a different port
PORT=3001 npm start
```

**"npm: command not found"**
- Node.js is not installed. Download from https://nodejs.org/

**"Module not found"**
```bash
# Reinstall dependencies
rm -rf node_modules package-lock.json
npm install
```

## 💡 Tips

- Use browser DevTools (F12) to test responsive design
- All colors are CSS variables in `src/styles/globals.css`
- Animations are defined in `globals.css` with `@keyframes`
- Mock data is in each page component - will be replaced with API calls

## 📚 React Documentation
- React Docs: https://react.dev
- React Router: https://reactrouter.com/
- CSS Variables: https://developer.mozilla.org/en-US/docs/Web/CSS/--*

## 📝 Notes

- Currently, all data is stored in React state (localStorage would persist across sessions)
- Users are not actually saved - they exist only for the current session
- Email sending is mocked - will be implemented in backend phase
- AI jokes are hardcoded - will be fetched from OpenAI API in backend phase

---

**Happy drawing! 🎁 Let me know when you're ready to move to Phase 2 (Backend).**
