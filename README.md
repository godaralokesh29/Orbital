# Orbital 🚀

A comprehensive **real-time collaboration platform** designed for modern development teams. Orbital combines video conferencing, live code editing, and interactive whiteboarding into a unified workspace, enabling seamless remote collaboration and pair programming.

## ✨ Features

### 🎥 Video Conferencing
- Real-time video and audio communication powered by **LiveKit**
- Crystal-clear HD video quality
- Built-in audio controls and muting capabilities
- Screen sharing support for presentations and live demos

### 💻 Live Code Editor
- Real-time synchronized code editing with multiple participants
- Syntax highlighting for multiple programming languages
- Integrated with **Sandpack** for live code preview and execution
- Line-by-line code synchronization
- Support for various file types and formats

### 🎨 Whiteboarding
- Interactive digital whiteboard for sketching and brainstorming
- Real-time drawing synchronization across all participants
- Shape tools and freehand drawing capabilities
- Powered by **Rough.js** for a natural sketching experience
- **XYFlow** integration for flowcharts and diagrams

### 🔐 Authentication & Security
- Secure Google OAuth authentication
- Session management with **NextAuth**
- User-specific permissions and access control
- Secure token-based WebSocket connections

### 💾 Data Management
- PostgreSQL database for persistent storage
- **Prisma ORM** for efficient database operations
- User profiles and session history
- Data persistence across browser sessions

### 🎯 User Experience
- Beautiful, responsive UI with **Tailwind CSS**
- Dark mode support with **next-themes**
- Smooth animations with **Framer Motion**
- Toast notifications for user feedback
- Accessible components with **Radix UI**

## 🛠️ Tech Stack

### Frontend
- **React 18** - UI library
- **Next.js 15** - React framework with server-side rendering
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **Framer Motion** - Animation library
- **Lucide React** - Icon library

### Backend & Real-time
- **Next.js API Routes** - Server-side logic
- **WebSockets (ws)** - Real-time communication
- **LiveKit** - Video/audio infrastructure
- **Axios** - HTTP client

### Database & ORM
- **PostgreSQL** - Relational database
- **Prisma** - Modern ORM for Node.js

### Authentication
- **NextAuth.js** - Authentication library
- **Google OAuth** - Third-party authentication

### Development Tools
- **Turbopack** - Fast JavaScript bundler
- **ESLint** - Code linting
- **TypeScript** - Type checking

### Additional Libraries
- **React Flow** - Diagram rendering
- **Sandpack** - Code sandbox and editor
- **React Split** - Resizable panel layout
- **React Markdown** - Markdown rendering
- **Class Variance Authority** - CSS-in-JS utilities

## 📋 Language Composition

- **TypeScript**: 98.3% - Core development language
- **CSS**: 1.3% - Styling
- **JavaScript**: 0.4% - Configuration and utilities

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn package manager
- PostgreSQL database
- Google OAuth credentials

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/godaralokesh29/Orbital.git
   cd Orbital
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   
   Create a `.env.local` file in the root directory:
   ```env
   # Database
   DATABASE_URL=postgresql://user:password@localhost:5432/orbital
   
   # NextAuth
   NEXTAUTH_URL=http://localhost:3000
   NEXTAUTH_SECRET=your-secret-key-here
   
   # Google OAuth
   GOOGLE_CLIENT_ID=your-google-client-id
   GOOGLE_CLIENT_SECRET=your-google-client-secret
   
   # LiveKit
   NEXT_PUBLIC_LIVEKIT_URL=your-livekit-server-url
   LIVEKIT_API_KEY=your-livekit-api-key
   LIVEKIT_API_SECRET=your-livekit-api-secret
   
   # Google AI (for ChatGPT-like features)
   NEXT_PUBLIC_GOOGLE_GENERATIVE_AI_KEY=your-google-ai-key
   ```

4. **Set up the database**
   ```bash
   npx prisma migrate dev
   ```

5. **Run the development server**
   ```bash
   npm run dev
   ```

   Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## 📦 Available Scripts

```bash
# Development
npm run dev              # Start development server with Turbopack

# Production
npm run build            # Build for production
npm start                # Start production server

# Code Quality
npm run lint             # Run ESLint for code linting
```

## 🏗️ Project Structure

```
Orbital/
├── app/                 # Next.js app directory
├── components/          # Reusable React components
├── lib/                 # Utility functions and helpers
├── prisma/              # Database schema and migrations
├── public/              # Static assets
├── styles/              # Global CSS and Tailwind config
├── types/               # TypeScript type definitions
└── package.json         # Dependencies and scripts
```

## 🔌 API Endpoints

The application provides various API endpoints for:
- User authentication and session management
- Real-time session creation and management
- WebSocket connections for live collaboration
- Video call signaling through LiveKit

## 🎨 Key Components

- **Video Room** - Real-time video conferencing component
- **Code Editor** - Collaborative code editing with Sandpack
- **Whiteboard** - Drawing canvas with XYFlow integration
- **Chat** - Real-time messaging system
- **User Management** - Profile and permission controls

## 🔒 Security Features

- Secure OAuth authentication with Google
- Session-based access control
- WebSocket token validation
- Database query parameterization with Prisma
- CORS protection
- Environment variable separation

## 🌐 Deployment

The project is configured for deployment on:
- **Vercel** - Recommended for Next.js applications
- **Docker** - Container-based deployment
- Any Node.js hosting platform

### Deployment Checklist
- [ ] Set up PostgreSQL database
- [ ] Configure environment variables on host
- [ ] Set up LiveKit server or use managed service
- [ ] Configure Google OAuth credentials
- [ ] Update NEXTAUTH_URL and NEXTAUTH_SECRET
- [ ] Build and deploy

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📋 Topics & Tags

- `chatgpt-api` - AI integration capabilities
- `googleauth` - OAuth authentication
- `livekit` - Real-time communication
- `postgressql` - Database
- `turborepo` - Build optimization

## 🐛 Known Issues

Please check the [Issues](https://github.com/godaralokesh29/Orbital/issues) tab for known bugs and feature requests.

## 📝 License

This project is currently unlicensed. Feel free to fork and use for your own purposes.

## 👤 Author

**Alokesh Godar**
- GitHub: [@godaralokesh29](https://github.com/godaralokesh29)

## 🙋 Support

If you encounter any issues or have questions, please:
1. Check the [Issues](https://github.com/godaralokesh29/Orbital/issues) page
2. Create a new issue with detailed information
3. Include your environment details and steps to reproduce

## 🎯 Roadmap

Potential future enhancements:
- [ ] Real-time collaborative debugging
- [ ] Version control integration
- [ ] Advanced analytics dashboard
- [ ] Mobile app support
- [ ] Plugin ecosystem
- [ ] Self-hosted deployment guide
- [ ] AI-powered code suggestions
- [ ] Recording and playback functionality

---

**Made with ❤️ by Alokesh Godar**

Star ⭐ this repository if you find it useful!
