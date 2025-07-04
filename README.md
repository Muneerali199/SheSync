
<img src="ssoc.png" alt="ssoc" width="800"/>

# SheSync - Next.js

# SheSync


SheSync is a comprehensive women's health and wellness platform built with **Next.js 14** and modern web technologies. The platform aims to provide a supportive environment for women to access health resources, connect with healthcare professionals, and engage with a community of like-minded individuals.

## 🚀 Features

- **AI-Powered Health Assistant**: Get instant answers to your health-related questions
- **Community Forum**: Connect with other women and share experiences
- **Educational Resources**: Access curated health and wellness information
- **Professional Consultation**: Connect with healthcare providers
- **Period Tracking**: Monitor and understand your menstrual cycle
- **PCOS Diagnosis Tool**: AI-powered symptom analysis for PCOS risk assessment
- **Symptom Analysis**: Comprehensive health symptom tracking and analysis
- **Shop**: Access health and wellness products
- **Parent Dashboard**: Secure family health monitoring with privacy controls

## 🛠️ Technologies Used

### Frontend

- **Next.js 14** - React framework with App Router
- **React 18** - Modern UI library with hooks and context
- **TypeScript** - Type-safe development
- **TailwindCSS** - Utility-first CSS framework
- **Framer Motion** - Animation library for smooth transitions
- **Clerk** - Authentication and user management
- **Google Maps API** - Location services for consultations
- **Google Generative AI** - AI-powered health insights

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **Clerk SDK** - Server-side authentication
- **CORS** - Cross-origin resource sharing

- React 18
- Vite
- TailwindCSS
- Framer Motion (for animations)
- React Router DOM
- Google Maps API
- Google Generative AI
- **Clerk Authentication**: Secure user authentication with Clerk


### UI Components
- **Headless UI** - Unstyled, accessible UI components
- **Radix UI** - Low-level UI primitives
- **Lucide React** - Beautiful icon set

## 📦 Installation

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/SheSync.git
cd SheSync
````


2. **Install dependencies:**

2. Install dependencies:


```bash
npm install
```


3. **Install backend dependencies:**
```bash
cd Backend
npm install
cd ..
```

4. **Environment Setup:**

Create `.env.local` file in the root directory:
```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
NEXT_PUBLIC_GOOGLE_MAPS_API_KEY=your_google_maps_api_key
NEXT_PUBLIC_GOOGLE_AI_API_KEY=your_google_ai_api_key
NEXT_PUBLIC_GEMINI_API_KEY=your_gemini_api_key
NEXT_PUBLIC_SERVER_URL=https://shesync.onrender.com/
```

Create `Backend/.env` file:
```env
MONGO_URL=your_mongodb_connection_string
PORT=3000
NODE_ENV=development
FRONTEND_URL=http://localhost:3000
CLERK_SECRET_KEY=your_clerk_secret_key
```

5. **Start the development servers:**

Frontend (Next.js):

3. Create a `.env` file in the root directory and add necessary environment variables:

```env
VITE_SERVER_URL=https://shesync.onrender.com/

VITE_GEMINI_API_KEY=AIzaSyDC_nwnZggf8CYID3qvJfazEE8KBnqd9Ro // Use new API key, this one is not working
VITE_CLERK_PUBLISHABLE_KEY=pk_test_YW11c2luZy1ob3JuZXQtOS5jbGVyay5hY2NvdW50cy5kZXYk

VITE_GOOGLE_MAPS_API_KEY=AIzaSyB5pTapWtBsb95f5qpxiadprABnynOIZdQ
```

4. Start the development server:


```bash
npm run dev
```

Backend (in a separate terminal):
```bash
cd Backend
npm run dev
```

## 🏗️ Project Structure

```

app/                             # Next.js App Router
├── (auth)/                      # Auth route group
│   ├── login/page.tsx          # Login page
│   └── signup/page.tsx         # Signup page
├── dashboard/page.tsx          # User dashboard
├── blogs/page.tsx              # Educational content
├── ecom/page.tsx               # E-commerce shop
├── tracker/page.tsx            # Period tracking
├── partner/page.tsx            # PCOS diagnosis
├── consultations/page.tsx      # Healthcare consultations
├── chatbot/page.tsx            # AI health assistant
├── symptomsanalyzer/page.tsx   # Symptom analysis
├── parents/page.tsx            # Parent dashboard
├── forums/page.tsx             # Community forums
├── team/page.tsx               # Team showcase
├── layout.tsx                  # Root layout
├── page.tsx                    # Home page
└── globals.css                 # Global styles

components/                      # Reusable UI components
├── common/                     # Shared components
│   ├── ErrorBoundary.tsx      # Error handling
│   ├── LoadingSpinner.tsx     # Loading states
│   └── ProtectedRoute.tsx     # Route protection
├── Landing.tsx                 # Landing page component
├── Dashboard.tsx               # Dashboard component
├── SideBar.tsx                 # Navigation sidebar
|__ Consultations.tsx           
└── [other components...]       # Feature components

context/                        # React context providers
└── ThemeContext.tsx           # Theme management

hooks/                          # Custom React hooks
├── useApi.ts                  # API interaction hook
└── useScreenSize.ts           # Responsive design hook

utils/                          # Utility functions
├── api.ts                     # API configuration
├── errorHandler.ts            # Error handling
├── validation.ts              # Form validation
└── gemini.ts                  # Google Gemini AI

config/                         # Configuration files
└── constants.ts               # App constants

Backend/                        # Backend server code
├── controllers/               # Route controllers
├── models/                    # Database models
├── routes/                    # API routes
├── middlewares/               # Custom middleware
├── config/                    # Configuration files
└── index.js                   # Server entry point
```

## 🔧 Key Features Overview

### 🏠 **Dashboard**
- Personalized health insights and cycle tracking
- Water intake monitoring
- Mood and symptom analysis
- Privacy controls for data sharing

### 📚 **Education Hub**
- Interactive health articles and blogs
- Gamified learning with progress tracking
- Expert-reviewed content
- Quiz system for knowledge validation

### 🛍️ **Shop**
- Curated health and wellness products
- Eco-friendly menstrual products
- Integrated cart and checkout system
- Product recommendations

### 📊 **Period Tracker**
- Comprehensive cycle monitoring
- Symptom and mood tracking
- Predictive analytics for next period
- Health insights and recommendations

### 🔬 **PCOS Diagnosis Tool**
- AI-powered symptom analysis
- Risk assessment with visual charts
- Personalized recommendations
- Medical disclaimer and guidance

### 🤖 **AI Health Assistant (Eve)**
- 24/7 health support chatbot
- Context-aware responses
- Integration with Google Gemini AI
- Personalized health advice

### 🩺 **Symptom Analyzer (HealthLens)**
- Multi-step symptom assessment
- Community insights and patterns
- Emergency symptom detection
- Lifestyle recommendations

### 👨‍👩‍👧‍👦 **Parent Dashboard**
- Secure family health monitoring
- Privacy-controlled data sharing
- Age-appropriate health insights
- Emergency alerts and notifications

### 💬 **Community Forums**
- Safe, moderated discussion spaces
- Expert Q&A sessions
- Anonymous posting options
- Community support groups

### 🏥 **Expert Consultations**
- Video and in-person appointments
- Healthcare provider directory
- Integrated booking system
- Location-based services

## 🔒 Security & Privacy

- **End-to-end encryption** for sensitive health data
- **GDPR compliant** data handling
- **Role-based access control** for family features
- **Secure authentication** with Clerk
- **Privacy controls** for data sharing preferences

## 🌐 Deployment

### Frontend (Next.js)
Deploy to Vercel (recommended) or Netlify:

```bash
# Build the application
npm run build

# Deploy to Vercel
npx vercel

# Or deploy to Netlify
npm run build && netlify deploy --prod --dir=.next
```

### Backend
Deploy to Render.com, Railway, or any Node.js hosting service.

## 🧪 Testing

Run the test suite:
```bash
npm test
```

Run tests with coverage:
```bash
npm run test:coverage
```

Type checking:
```bash
npm run type-check
```

## 📱 Mobile Responsiveness

SheSync is fully responsive and optimized for:
- **Mobile devices** (320px and up)
- **Tablets** (768px and up)
- **Desktop** (1024px and up)
- **Large screens** (1440px and up)

## 🔄 Migration from React to Next.js

This project has been successfully migrated from a React + Vite setup to Next.js 14 with the following improvements:

### ✅ What's New
- **App Router**: Modern file-based routing system
- **Server Components**: Better performance and SEO
- **TypeScript**: Full type safety across the application
- **Improved SEO**: Meta tags and structured data
- **Better Performance**: Automatic code splitting and optimization
- **Enhanced Developer Experience**: Better error handling and debugging

### 🔄 Migration Benefits
- **Better Performance**: Next.js optimizations and server-side rendering
- **Improved SEO**: Better search engine visibility
- **Enhanced Security**: Built-in security features
- **Scalability**: Better architecture for future growth
- **Developer Experience**: Improved tooling and debugging

src/
├── components/                    # Reusable UI components
│   ├── Landing.jsx              # Main landing page component
│   ├── Dashboard.jsx            # User dashboard interface
│   ├── ParentDashboard.jsx      # Parent-specific dashboard
│   ├── PartnerDashboard.jsx     # Partner-specific dashboard
│   ├── PeriodTracker.jsx        # Period tracking functionality
│   ├── SymptomAnalysis.jsx      # Health symptom analysis tool
│   ├── Chatbot.jsx              # AI-powered health assistant
│   ├── CommunityChat.jsx        # Community chat interface
│   ├── Forum.jsx                # Community forum component
│   ├── Blogs.jsx                # Health blog section
│   ├── Consultations.jsx        # Healthcare consultation booking
│   ├── Ecom.jsx                 # E-commerce shop interface
│   ├── Login.jsx                # User authentication
│   ├── Signup.jsx               # User registration
│   ├── Quiz.jsx                 # Health assessment quiz
│   ├── PrivacyForm.jsx          # Privacy policy form
│   └── ModernTeamShowcase.jsx   # Team member showcase
│
├── utils/                       # Utility functions and helpers
│   └── gemini.js               # Google Gemini AI integration
│
├── styles/                      # Global styles and CSS
│   └── index.css               # Main stylesheet
│
├── App.jsx                      # Main application component
├── main.jsx                     # Application entry point
└── index.css                    # Global styles

public/                          # Static assets
├── images/                      # Image assets
└── icons/                       # Icon assets

Backend/                         # Backend server code
├── controllers/                 # Route controllers
├── models/                      # Database models
├── routes/                      # API routes
└── config/                      # Configuration files
```

### Key Components Overview

#### Core Features

* **Landing Page**: Main entry point with feature showcase and navigation
* **Dashboard**: Personalized user interface with health metrics and quick actions
* **Period Tracker**: Menstrual cycle tracking and analysis
* **Symptom Analysis**: AI-powered health symptom assessment
* **Chatbot**: AI health assistant powered by Google Gemini

#### Community Features

* **Forum**: Community discussion platform
* **Community Chat**: Real-time chat functionality
* **Blogs**: Health and wellness articles
* **ModernTeamShowcase**: Healthcare professional profiles

#### User Management

* **Login/Signup**: User authentication and registration with **Clerk** authentication system
* **PrivacyForm**: Privacy policy and data handling
* **Quiz**: Initial health assessment

#### Healthcare Services

* **Consultations**: Healthcare provider booking system
* **Ecom**: Health and wellness product marketplace

#### Specialized Dashboards

* **ParentDashboard**: Features for parents/guardians
* **PartnerDashboard**: Features for partners/spouses

### Technology Stack Details

#### Frontend Architecture

* **React Components**: Modular, reusable UI components
* **State Management**: React hooks and context
* **Routing**: React Router for navigation
* **Styling**: TailwindCSS for responsive design
* **Animations**: Framer Motion for smooth transitions

#### Backend Integration

* **API Integration**: Axios for HTTP requests
* **Authentication**: Clerk middleware Authentication
* **Database**: MongoDB for data storage
* **Real-time Features**: WebSocket integration

#### Development Tools

* **Build Tool**: Vite for fast development
* **Code Quality**: ESLint for code linting
* **Version Control**: Git for source control
* **Package Management**: npm for dependencies


## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/amazing-feature`)
3. **Make your changes**
4. **Add tests** for new functionality
5. **Commit your changes** (`git commit -m 'Add some amazing feature'`)
6. **Push to the branch** (`git push origin feature/amazing-feature`)
7. **Open a Pull Request**

### Code Style Guidelines


- Follow the existing TypeScript and Next.js conventions
- Use meaningful variable and function names
- Add comments for complex logic
- Write unit tests for new features
- Ensure all tests pass before submitting a PR
- Use proper TypeScript types throughout

* Follow the existing code style
* Use meaningful variable and function names
* Add comments for complex logic
* Write unit tests for new features
* Ensure all tests pass before submitting a PR


## 📝 API Documentation

### Authentication Endpoints
```
POST /api/auth/clerk-webhook    # Clerk user creation/updates
GET  /api/auth/profile          # Get user profile
```

### Period Tracking Endpoints
```
POST /api/period/trackerdata           # Submit tracking data
GET  /api/period/periodtracking/:userId # Get period data
GET  /api/period/waterupdate/:userId    # Update water intake
```


### Forum Endpoints
```
POST /api/post/createPost       # Create new post
GET  /api/post/getPost          # Get all posts
GET  /api/post/like/:id         # Like a post
```

* Using welcoming and inclusive language
* Being respectful of differing viewpoints and experiences
* Gracefully accepting constructive criticism
* Focusing on what is best for the community
* Showing empathy towards other community members


## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments


- **Team WEB PIONEERS** for their dedication and hard work
- **Healthcare professionals** who provided guidance and expertise
- **Next.js team** for the amazing framework
- **Open-source community** for the amazing tools and libraries
- **Beta testers** who helped improve the platform

## 📞 Support

If you need help or have questions:
- **Documentation**: Check our comprehensive docs
- **Issues**: Open an issue on GitHub
- **Email**: Contact our support team
- **Community**: Join our Discord server

## 🚀 Future Roadmap

- **AI-powered meal planning** based on cycle phases
- **Wearable device integration** for automatic tracking
- **Telemedicine platform** expansion
- **Mental health resources** and counseling
- **Global expansion** with localized content
- **Research partnerships** for health studies
- **Progressive Web App (PWA)** features
- **Real-time notifications** and alerts

---

**Made with ❤️ for women's health and wellness using Next.js 14**

*SheSync - Empowering Women One Cycle at a Time*

* All contributors who have helped shape this project
* The open-source community for their invaluable tools and libraries
* Healthcare professionals who have provided guidance and expertise

## 📞 Support

If you need help or have questions, please:

* Open an issue in the GitHub repository
* Contact the maintainers
* Join our community forum

---
