# BoothBiz - Event Booth Management Platform

**BoothBiz** is a comprehensive event booth management and analytics platform built with React and Vite. It provides businesses and event organizers with powerful tools for managing booths, tracking visitor interactions, and generating detailed analytics reports with an intuitive, feature-rich interface.

**Live Demo:** [https://booth-biz.vercel.app](https://booth-biz.vercel.app)

---

## 📊 Project Stats

- **Language:** 99.5% JavaScript, 0.5% Other
- **Build Tool:** Vite 5.4.11
- **Framework:** React 18.3.1
- **State Management:** Redux Toolkit + Redux Persist
- **Styling:** Tailwind CSS 3.4.12
- **Backend:** Firebase
- **Repository:** Public
- **Created:** February 16, 2026
- **Last Updated:** February 16, 2026

---

## 🎯 Purpose

BoothBiz is designed to provide:
- **Booth Management** - Create, configure, and manage event booths
- **Visitor Tracking** - Monitor visitor interactions and engagement
- **Analytics Dashboard** - Visual insights into booth performance
- **Real-time Updates** - Live data synchronization with Firebase
- **Responsive Design** - Works seamlessly across devices
- **User Authentication** - Secure booth owner access and management

---

## 🛠️ Technology Stack

### Core Framework & Runtime
- **React 18.3.1** - UI library for building user interfaces
- **Vite 5.4.11** - Next-generation build tool with HMR
- **JavaScript (ES Module)** - 99.5% of codebase
- **Node.js** - JavaScript runtime

### State Management
- **Redux Toolkit 2.2.8** - Modern Redux with simplified syntax
- **React Redux 9.1.2** - Official React bindings for Redux
- **Redux Persist 6.0.0** - Persist Redux store to local storage
- **Redux Thunk 3.1.0** - Middleware for async actions

### Backend & Database
- **Firebase 10.14.1** - Backend-as-a-service platform
  - Authentication (Email/Password, Google, etc.)
  - Firestore Database (Real-time NoSQL)
  - Cloud Storage
  - Cloud Functions support

### Forms & Validation
- **React Hook Form 7.53.0** - Performant form management
- **React Modal 3.16.1** - Modal/dialog components

### Styling & Layout
- **Tailwind CSS 3.4.12** - Utility-first CSS framework
- **PostCSS 8.4.47** - CSS transformations
- **Autoprefixer 10.4.20** - Automatic vendor prefixes

### UI Components & Icons
- **Lucide React 0.445.0** - Modern SVG icon library
- **React Icons 5.3.0** - Additional icon sets
- **React Feather 2.0.10** - Feather icon library
- **FontAwesome 6.6.0** - FontAwesome icons with React
- **shadcn 1.0.0** - Pre-built accessible components

### Animations & Visualization
- **Framer Motion 11.5.6** - React animation library
- **Recharts 2.12.7** - Composable charting library for analytics

### Routing & Navigation
- **React Router DOM 6.26.2** - Client-side routing
- **React Router Hash Link 2.4.3** - Hash-based navigation

### Utilities
- **Lodash 4.17.21** - Utility functions
- **lodash.debounce 4.0.8** - Debounce function
- **UUID 10.0.0** - Generate unique identifiers

---

## 📁 Project Structure

```
booth-biz/
├── src/
│   ├── components/              # React components
│   │   ├── common/              # Shared components
│   │   ├── layout/              # Layout components
│   │   ├── booths/              # Booth-related components
│   │   ├── analytics/           # Analytics components
│   │   ├── dashboard/           # Dashboard components
│   │   └── forms/               # Form components
│   ├── pages/                   # Page components
│   ├── store/                   # Redux store and slices
│   │   ├── slices/              # Redux slices
│   │   ├── thunks/              # Async thunks
│   │   └── store.js             # Store configuration
│   ├── services/                # Firebase services
│   │   ├── auth.js              # Authentication
│   │   ├── booths.js            # Booth operations
│   │   ├── analytics.js         # Analytics data
│   │   └── firebase.js          # Firebase config
│   ├── hooks/                   # Custom React hooks
│   ├── utils/                   # Utility functions
│   ├── styles/                  # Global styles
│   ├── App.jsx                  # Root component
│   └── main.jsx                 # Entry point
├── public/                      # Static assets
├── Final Output/                # Built/exported files
├── index.html                   # HTML entry point
├── vite.config.js               # Vite configuration
├── tailwind.config.js           # Tailwind CSS config
├── postcss.config.js            # PostCSS config
├── eslint.config.js             # ESLint rules
├── package.json                 # Dependencies
└── README.md                    # This file
```

---

## 🎨 Key Features

### 1. **Booth Management**
- Create and configure event booths
- Set booth details (name, description, location)
- Manage booth status (active, inactive, archived)
- Booth customization options
- Multi-booth support

### 2. **Visitor Tracking**
- Log visitor interactions
- Track visit time and duration
- Capture visitor information
- Record engagement level
- Visit history and timeline

### 3. **Analytics Dashboard**
- Visual performance metrics
- Real-time visitor counts
- Charts and graphs using Recharts
- Time-series analytics
- Comparative analysis
- Export analytics data

### 4. **Real-time Synchronization**
- Firebase Firestore integration
- Real-time data updates
- Cloud sync across devices
- Persistent storage
- Offline capability with Redux Persist

### 5. **User Authentication**
- Email/password login
- Secure session management
- User roles and permissions
- Protected routes
- Remember user sessions

### 6. **Responsive Design**
- Mobile-first approach
- Tablet and desktop optimization
- Touch-friendly interface
- Accessible navigation
- Works offline with local cache

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ or higher
- npm or yarn
- Firebase account (for backend)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/SmitSolanki-303/BoothBiz.git
   cd BoothBiz
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure Firebase:**
   - Create a `.env.local` file:
   ```env
   VITE_FIREBASE_API_KEY=your_api_key
   VITE_FIREBASE_AUTH_DOMAIN=your_auth_domain
   VITE_FIREBASE_PROJECT_ID=your_project_id
   VITE_FIREBASE_STORAGE_BUCKET=your_storage_bucket
   VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
   VITE_FIREBASE_APP_ID=your_app_id
   ```

4. **Run development server:**
   ```bash
   npm run dev
   ```

5. **Open in browser:**
   ```
   http://localhost:5173
   ```

---

## 📝 Development Scripts

```bash
# Development server with HMR
npm run dev

# Production build
npm run build

# Preview production build
npm run preview

# Run ESLint
npm run lint
```

---

## 📊 State Management (Redux)

### Redux Structure

```
store/
├── slices/
│   ├── authSlice.js       # Authentication state
│   ├── boothsSlice.js     # Booths data
│   ├── analyticsSlice.js  # Analytics data
│   ├── uiSlice.js         # UI state
│   └── ...
├── thunks/
│   ├── authThunks.js      # Async auth operations
│   ├── boothThunks.js     # Async booth operations
│   └── ...
└── store.js               # Store configuration
```

### Redux Persist

Configured to persist:
- Authentication state
- User preferences
- Booth data cache
- Analytics cache

---

## 🔐 Firebase Configuration

### Authentication
- Email/Password auth
- Custom claims for roles
- Session persistence
- Password reset flow

### Firestore Database
```
users/
├── {userId}/
│   ├── profile
│   ├── booths (subcollection)
│   └── settings

booths/
├── {boothId}/
│   ├── details
│   ├── visitors (subcollection)
│   ├── analytics (subcollection)
│   └── status

analytics/
├── {boothId}/
│   ├── {date}/
│   │   ├── visitor_count
│   │   ├── engagement_score
│   │   └── ...
```

---

## 📈 Analytics Features

### Metrics Tracked
- Total visitors
- Unique visitors
- Average visit duration
- Peak visitor times
- Engagement scores
- Conversion metrics
- Daily/Weekly/Monthly trends

### Visualization
- Line charts (trends)
- Bar charts (comparisons)
- Pie charts (distribution)
- Custom date ranges
- Real-time updates

---

## 🎨 UI/UX Components

### Layout Components
- Navbar with navigation
- Sidebar for menu
- Dashboard layout
- Card-based design
- Modal dialogs
- Toast notifications

### Form Components
- Text inputs
- Select dropdowns
- Date pickers
- Checkboxes
- Toggle switches
- Form validation

### Analytics Components
- Dashboard widgets
- Chart components
- Statistics cards
- Progress indicators
- Data tables

---

## ⚙️ Configuration Files

### `vite.config.js`
```javascript
// Vite configuration
// React plugin for HMR
// Environment variables
```

### `tailwind.config.js`
```javascript
// Tailwind CSS theme
// Color palette
// Custom utilities
```

### `eslint.config.js`
```javascript
// ESLint rules
// React-specific rules
// Code quality standards
```

---

## 🔄 Firebase Integration

### Authentication Service
```javascript
// src/services/auth.js
- signUp(email, password)
- signIn(email, password)
- signOut()
- getCurrentUser()
- updateProfile()
```

### Booth Service
```javascript
// src/services/booths.js
- createBooth(boothData)
- updateBooth(boothId, data)
- deleteBooth(boothId)
- getBooth(boothId)
- listBooths(userId)
```

### Analytics Service
```javascript
// src/services/analytics.js
- recordVisit(boothId, visitData)
- getAnalytics(boothId, dateRange)
- generateReport(boothId)
```

---

## 📱 Responsive Breakpoints

```
Mobile: < 640px
Tablet: 640px - 1024px
Desktop: > 1024px
```

---

## ♿ Accessibility Features

- ARIA labels and descriptions
- Semantic HTML
- Keyboard navigation
- Focus management
- Color contrast compliance
- Screen reader support
- Form validation messages

---

## 🚢 Deployment

### Vercel (Recommended)
```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel
```

### Environment Variables on Vercel
Set Firebase credentials in Vercel dashboard under:
- Project Settings → Environment Variables

### Build for Production
```bash
npm run build
```

Output is in the `dist/` directory.

---

## 🎯 Best Practices

### Component Development
1. Keep components small and reusable
2. Use functional components with hooks
3. Extract complex logic to custom hooks
4. Implement error boundaries
5. Use React.memo for optimization

### State Management
1. Use Redux slices for organization
2. Separate async logic in thunks
3. Keep selectors close to usage
4. Normalize data in state
5. Use Redux DevTools for debugging

### Firebase Operations
1. Use async/await for clarity
2. Implement proper error handling
3. Add loading states
4. Debounce rapid updates
5. Cache frequently accessed data

### Styling
1. Use Tailwind utilities
2. Avoid inline styles
3. Maintain consistent spacing
4. Follow design system
5. Mobile-first approach

---

## 🐛 Troubleshooting

### Firebase Connection Issues
```bash
# Check Firebase config
# Verify API keys in .env.local
# Check Firebase console permissions
```

### Redux State Issues
```bash
# Use Redux DevTools extension
# Check action dispatches
# Verify slice reducers
```

### Build Errors
```bash
# Clear cache
rm -rf node_modules dist
npm install

# Rebuild
npm run build
```

---

## 📚 Learn More

### Official Documentation
- [React Documentation](https://react.dev)
- [Vite Documentation](https://vitejs.dev)
- [Redux Documentation](https://redux.js.org/)
- [Firebase Documentation](https://firebase.google.com/docs)
- [Tailwind CSS](https://tailwindcss.com/docs)
- [React Router](https://reactrouter.com/)
- [React Hook Form](https://react-hook-form.com/)

### Helpful Resources
- [Redux Toolkit Guide](https://redux-toolkit.js.org/)
- [Firestore Security Rules](https://firebase.google.com/docs/firestore/security/start)
- [Recharts Examples](https://recharts.org/examples)
- [React Hooks Guide](https://react.dev/reference/react/hooks)

---

## 🤝 Contributing

### Code Style
- Use ES6+ syntax
- Follow naming conventions
- Write readable code
- Add comments for complex logic
- Keep functions small and focused

### Pull Request Process
```bash
# Create feature branch
git checkout -b feature/your-feature

# Make changes
git add .

# Commit
git commit -m "feat: add new feature"

# Push
git push origin feature/your-feature
```

---

## 📄 License

No license specified. Check repository for details.

---

## 👤 Author

**Smit Solanki**
- GitHub: [@SmitSolanki-303](https://github.com/SmitSolanki-303)
- Email: smitsolanki303@gmail.com
- Portfolio: [GitHub Profile](https://github.com/SmitSolanki-303)

---

## 🙏 Acknowledgments

Built with modern web technologies:
- [React](https://react.dev) - UI library
- [Vite](https://vitejs.dev) - Build tool
- [Redux Toolkit](https://redux-toolkit.js.org/) - State management
- [Firebase](https://firebase.google.com/) - Backend services
- [Tailwind CSS](https://tailwindcss.com/) - Styling
- [Recharts](https://recharts.org/) - Data visualization
- [React Router](https://reactrouter.com/) - Routing

---

## 🗺️ Roadmap

- [ ] Advanced analytics with machine learning
- [ ] Multi-language support (i18n)
- [ ] Theme customization
- [ ] Export to PDF/Excel
- [ ] Email notifications
- [ ] SMS alerts
- [ ] Integration with event platforms
- [ ] Mobile app (React Native)

---

**Status:** Active Development  
**Last Updated:** February 16, 2026  
**Repository:** [GitHub](https://github.com/SmitSolanki-303/BoothBiz)  
**Live Demo:** [https://booth-biz.vercel.app](https://booth-biz.vercel.app)
