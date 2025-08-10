
# PropBot – AI-Powered Property Suggestion Platform

PropBot is a full-stack real estate platform that helps users discover, compare, and save properties with the assistance of an intelligent AI chatbot. The platform features a modern React.js frontend, a robust Node.js/Express backend, and a rule-based chatbot that guides users to their ideal home or investment property.

**Key Highlight:**
> PropBot includes an advanced property chatbot that understands user queries (like "3 BHK in Mumbai under 1 crore" or "Show me villas with a swimming pool") and suggests the best matching homes, making property search easy and interactive.


## 🎯 Features

### 🏡 Property Search & Discovery
- **Smart Search**: Find properties by location, price, type (apartment, villa, etc.), amenities, bedrooms, and more.
- **Compare Properties**: Add properties to a compare bar for side-by-side comparison.
- **Save Favorites**: Users can save and manage their favorite properties.
- **Detailed Listings**: Each property includes images, features, amenities, and pricing.

### 🤖 PropBot Chatbot
- **Conversational Search**: Ask for homes in natural language (e.g., "2 BHK in Delhi under 50 lakhs").
- **Personalized Suggestions**: Get property recommendations based on your needs.
- **Predefined & Custom Queries**: Use quick suggestions or type your own.
- **Friendly Guidance**: PropBot can greet, answer questions, and help refine your search.

### � User Features
- **Authentication**: Secure signup/login with JWT.
- **Profile Management**: View and update user details.
- **Saved Properties**: Access and manage your saved homes.

### 💬 Enlarged Chatbox Layout
- **Split-Screen Design**: Chatbox is displayed on the **left** side, and property results appear on the **right** side in full-screen view.
- **Real-Time Updates**: Property results update instantly as you chat.
- **Better User Experience**: Large view makes browsing and chatting smooth.


### 🎨 UI/UX
- **Modern, Responsive Design**: Works on all devices.
- **Intuitive Navigation**: Easy to browse, search, and interact.


## 🛠️ Tech Stack

**Frontend:**
- React.js, Redux Toolkit, React Router, Axios, CSS3

**Backend:**
- Node.js, Express.js, MongoDB, Mongoose, JWT, bcryptjs

**AI & Utilities:**
- Rule-based NLP chatbot (using compromise.js)
- Firebase Admin (for notifications, if enabled)


## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- npm or yarn

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the backend directory with the following variables:
   ```
   PORT=5000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   JWT_EXPIRE=7d
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

### Frontend Setup
1. Navigate to the Frontend directory:
   ```bash
   cd Frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the backend directory with the following variables:
   ```
   VITE_BASE_URL=your_backend_deployement_string
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

5. Open your browser and visit `http://localhost:5173`


## 📁 Project Structure

```
Travel-app/
├── backend/
│   ├── Controllers/          # Property, user, and chatbot controllers
│   ├── Modals/               # Mongoose models (User, etc.)
│   ├── Routes/               # API routes (property, user, chatbot)
│   ├── Utils/                # Error handling, JWT, Firebase, etc.
│   ├── data/                 # Property data (JSON)
│   ├── middleware/           # Auth, error, async handling
│   ├── config/               # Database config
│   ├── app.js, index.js      # Express app entry
│   └── package.json
├── Frontend/
│   ├── src/
│   │   ├── Components/       # UI components (Chatbot, CompareBar, etc.)
│   │   ├── Pages/            # Main pages (Home, Login, Signup, etc.)
│   │   ├── redux/            # Redux store, slices, API
│   │   ├── Context/          # React context (UserContext)
│   │   ├── assets/           # Images and static files
│   │   └── Utils/            # Frontend utilities
│   ├── public/               # Static assets
│   ├── package.json
│   └── vite.config.js
└── README.md
```


## 🔧 Key API Endpoints

### Property APIs
- `GET /api/property/all` – Get all properties
- `GET /api/property/:id` – Get property by ID
- `GET /api/property/filter` – Filter/search properties
- `POST /api/property/save` – Save a property (user)
- `POST /api/property/unsave` – Unsave a property (user)
- `GET /api/property/saved` – Get all saved properties (user)

### User APIs
- `POST /api/user/register` – Register
- `POST /api/user/login` – Login
- `POST /api/user/forgotreset-password` – Login
- `GET /api/user/profile` – Get user profile


## 🔐 Authentication & Security
- JWT-based authentication
- Secure password hashing
- Role-based access (user/admin)


## 🚀 Deployment

### Backend Deployment
1. Set up environment variables on your hosting platform
2. Configure MongoDB connection
3. Deploy to platforms Vercel

### Frontend Deployment
1. Build the project: `npm run build`
2. Deploy to platforms Vercel 



---
## 📄 License
