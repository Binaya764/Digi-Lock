Digi-lock/
├── hardware/               # ESP32 / Arduino C++ code
│   ├── src/
│   │   └── main.cpp        # Primary logic for fingerprint sensing & Wi-Fi
│   └── libraries/          # Specific sensor libraries (AS608, etc.)
├── server/                 # Node.js + Express Backend
│   ├── config/             # Database (MongoDB) & Environment configs
│   ├── controllers/        # Logic for authentication and logs
│   ├── models/             # Mongoose schemas (User, AccessLog)
│   ├── routes/             # API endpoints (e.g., /api/auth, /api/users)
│   ├── middleware/         # API Key or JWT validation
│   └── server.js           # Entry point for the backend
├── client/                 # React Frontend (Vite-based)
│   ├── src/
│   │   ├── components/     # Reusable UI (Navbar, LogTable, UserCard)
│   │   ├── pages/          # Dashboard, Login, User Management
│   │   ├── services/       # API call functions (Axios/Fetch)
│   │   └── App.jsx
│   └── public/
├── docs/                   # Circuit diagrams and API documentation
├── .gitignore              # Ignore node_modules, .env, and build files
└── README.md               # Setup instructions for the team
