# AI Chatbot with GitHub Integration

This is an AI-powered chatbot built with Next.js, assistant-ui, and Google Gemini integration. The chatbot also includes GitHub API integration for repository management.

## Features

- 🤖 AI Chatbot powered by Google Gemini
- 🎨 Modern UI with assistant-ui components
- 🔧 GitHub API integration for repository operations
- 📱 Responsive design with sidebar navigation
- 🔄 Model switching capabilities
- 💬 Chat history and export functionality

## Tech Stack

- **Frontend**: Next.js 15, React, TypeScript
- **UI Components**: assistant-ui, Tailwind CSS, Radix UI
- **AI Integration**: Google Gemini API
- **GitHub Integration**: GitHub REST API
- **Development**: ESLint, PostCSS

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm/yarn/pnpm
- Google Gemini API key
- GitHub Personal Access Token (for GitHub features)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Shashank7275/ChatBot.git
cd ChatBot
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:

Create a `.env.local` file in the root directory and add:

```env
# Google Gemini API Key (required)
GOOGLE_GENERATIVE_AI_API_KEY=your_google_gemini_api_key_here

# OpenAI API Key (optional)
OPENAI_API_KEY=your_openai_api_key_here

# GitHub Personal Access Token (optional, for GitHub features)
GITHUB_TOKEN=your_github_token_here
```

**How to get API keys:**
- **Google Gemini**: Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
- **GitHub Token**: Go to GitHub Settings > Developer settings > Personal access tokens

4. Run the development server:
```bash
npm run dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser.

## GitHub Integration Features

The chatbot includes GitHub API integration that allows you to:

- View your repositories
- Check open issues
- Create new issues
- Create new repositories

To use GitHub features, make sure to add your GitHub Personal Access Token to the `.env.local` file.

## Project Structure

```
my-app/
├── app/                    # Next.js app directory
│   ├── api/               # API routes
│   │   ├── chat/         # AI chat endpoint
│   │   └── github/        # GitHub API integration
│   ├── assistant.tsx     # Main chatbot component
│   ├── layout.tsx        # Root layout
│   └── page.tsx          # Home page
├── components/            # React components
│   ├── assistant-ui/    # Assistant UI components
│   └── ui/               # UI components
├── lib/                   # Utility functions
└── test-*.js             # Test scripts for APIs
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run lint` - Run ESLint

## API Testing

The project includes several test scripts to verify API integrations:

- `test-google-correct.js` - Test Google Gemini API
- `test-chatbot.js` - Test chatbot API endpoint
- `test-github-*.js` - Test GitHub integration (coming soon)

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.
