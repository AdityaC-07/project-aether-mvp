# 🧠 PROJECT AETHER - AI-Powered Debate & Synthesis System

An intelligent platform for comprehensive document analysis and context synthesis using cutting-edge AI models.

## Features

- **📄 PDF Analysis**: Upload and analyze PDF documents for key arguments and synthesis
- **💬 Context Input**: Submit raw text/context for AI-powered analysis
- **📊 Interactive Results**: Visualize factors, positions, and synthesis with charts
- **📥 Report Generation**: Download analysis results as professional PDF reports
- **⚡ Real-time Processing**: Streaming results with loading indicators
- **🎨 Modern UI**: Built with Material-UI for professional appearance

## Tech Stack

- **Frontend**: React 19 + Vite (Fast build, HMR)
- **UI Framework**: Material-UI v7
- **Charts**: Recharts
- **API Client**: Axios + React Query
- **Deployment**: Vercel

## Quick Start

### Prerequisites
- Node.js 16+
- npm or yarn

### Installation

```bash
cd aether-frontend
npm install
```

### Development

```bash
npm run dev
```

Opens at `http://localhost:3000` with HMR enabled.

### Production Build

```bash
npm run build
```

Creates optimized build in `dist/` directory.

### Preview Production Build

```bash
npm run preview
```

## Environment Configuration

Create `.env` for development or `.env.production` for production:

```
VITE_API_BASE=http://localhost:8000
```

## Deployment

### Vercel (Recommended)

1. Connect GitHub repository to Vercel
2. Set environment variable `VITE_API_BASE` to your backend API URL
3. Deploy automatically on push

Vercel configuration is in `vercel.json` - no additional setup needed.

## Project Structure

```
aether-frontend/
├── src/
│   ├── components/     # Reusable UI components
│   ├── pages/          # Page components
│   ├── services/       # API services
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html          # Entry HTML
├── vite.config.js      # Vite configuration
├── vercel.json         # Vercel configuration
└── package.json
```

## API Endpoints

The frontend expects the following backend API:

- `POST /analyze-pdf` - Analyze PDF documents
- `POST /analyze` - Analyze context/text
- `POST /analyze-pdf-report` - Generate PDF report from PDF analysis
- `POST /analyze-context-report` - Generate PDF report from context analysis

## Contributing

This is a hackathon MVP. Feel free to submit issues or improvements!

## License

MIT
