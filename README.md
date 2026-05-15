# File Converter

A comprehensive, modern web-based file conversion and processing tool built with **Next.js 15**, **React 19**, and **TypeScript**.

## ✨ Features

### Core Conversions
- 🖼️ **Image Conversion** - Convert between JPG, PNG, GIF, WebP, etc.
- 🎵 **Audio Conversion** - Convert MP3, WAV, and more formats
- 🎬 **Video Conversion** - Convert MP4, MOV, MKV, and more
- 📄 **Document Conversion** - Convert DOC, DOCX, XLS, XLSX, CSV, TXT, PDF

### Advanced Features
- 🔄 **Batch Converting** - Convert multiple files at once
- 📦 **File Compression** - Reduce file sizes intelligently
- 🔗 **File Merge** - Combine multiple files into one
- ✂️ **File Split** - Split large files
- 🏷️ **Watermarking** - Add watermarks to images
- 🎨 **Image Editor** - Edit images directly in the browser
- 📄 **PDF Editor** - Edit and manipulate PDFs
- 🎵 **Audio Merger** - Merge multiple audio files
- ✂️ **Video Cutter** - Cut and trim videos
- 📱 **QR Generator** - Generate QR codes

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ or npm/yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/tun0Flex/file-converter.git
cd file-converter

# Install dependencies
npm install
# or
yarn install

# Create environment file
cp .env.local.example .env.local

# Start development server
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) to see the application.

## 📁 Project Structure

```
file-converter/
├── app/                      # Next.js App Router
│   ├── layout.tsx           # Root layout
│   ├── page.tsx             # Home page
│   ├── converter/           # Main converter pages
│   ├── features/            # Feature pages (batch, compress, etc.)
│   ├── tools/               # Tool pages (editor, merger, etc.)
│   ├── pricing/             # Pricing page
│   ├── about/               # About page
│   ├── contact/             # Contact page
│   └── api/                 # API routes (future)
│
├── components/              # React components
│   ├── shared/              # Shared components (Header, Footer, etc.)
│   ├── converter/           # Converter-specific components
│   ├── tools/               # Tool-specific components
│   └── ui/                  # shadcn/ui components
│
├── lib/                     # Core utilities and business logic
│   ├── converters/          # Converter implementations
│   ├── processors/          # File processing utilities
│   ├── utils/               # Utility functions
│   ├── hooks/               # Custom React hooks
│   ├── store/               # Zustand stores
│   └── config/              # Configuration files
│
├── public/                  # Static assets
│   ├── images/              # Image assets
│   └── icons/               # Icon assets
│
├── styles/                  # Global styles
│   ├── globals.css          # Global styles
│   ├── variables.css        # CSS variables
│   └── animations.css       # Animation definitions
│
├── types/                   # TypeScript type definitions
│   ├── conversion.ts        # Conversion types
│   ├── file.ts              # File types
│   └── index.ts             # Type exports
│
└── config files
    ├── package.json         # Dependencies
    ├── tsconfig.json        # TypeScript config
    ├── tailwind.config.ts   # Tailwind CSS config
    ├── postcss.config.js    # PostCSS config
    ├── next.config.js       # Next.js config
    ├── .eslintrc.json       # ESLint config
    ├── .prettierrc           # Prettier config
    └── .env.local.example   # Environment template
```

## 🛠️ Technology Stack

### Frontend
- **Next.js 15** - React framework with App Router
- **React 19** - UI library
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **Framer Motion** - Animations

### File Processing
- **FFmpeg.wasm** - Video/audio processing
- **pdf-lib** - PDF manipulation
- **pdfjs-dist** - PDF viewing
- **jsPDF** - PDF generation
- **Konva** - Canvas manipulation
- **xlsx** - Excel file handling
- **Mammoth** - Word document conversion

### State Management & Utils
- **Zustand** - State management
- **React Query** - Data fetching
- **Zod** - Schema validation
- **Lucide React** - Icons

## 📝 Available Scripts

```bash
# Development
npm run dev              # Start development server

# Production
npm run build            # Build for production
npm run start            # Start production server

# Code Quality
npm run lint             # Run ESLint with auto-fix
npm run type-check       # Check TypeScript types
npm run format           # Format code with Prettier
```

## 🔧 Configuration

### Environment Variables

Copy `.env.local.example` to `.env.local` and update:

```env
# API Configuration
NEXT_PUBLIC_APP_NAME=File Converter
NEXT_PUBLIC_APP_URL=http://localhost:3000

# File Upload Limits
NEXT_PUBLIC_MAX_FILE_SIZE=104857600  # 100MB in bytes
NEXT_PUBLIC_ALLOWED_FORMATS=jpg,png,gif,webp,pdf,mp3,wav,mp4,mov,mkv,doc,docx,xls,xlsx,csv,txt

# FFmpeg WASM
NEXT_PUBLIC_FFMPEG_CORE_URL=https://cdn.jsdelivr.net/npm/@ffmpeg/core@0.12.6/dist/umd/ffmpeg.js
```

## 🎨 Customization

### Theming

Edit `tailwind.config.ts` to customize colors and theme:

```typescript
colors: {
  primary: '#3B82F6',
  secondary: '#10B981',
  danger: '#EF4444',
  warning: '#F59E0B',
}
```

## 📦 Dependencies Summary

- **Next.js & React** - Core framework
- **File Processing** - FFmpeg, pdf-lib, xlsx, konva
- **UI** - Tailwind CSS, Framer Motion, Lucide Icons
- **State** - Zustand, React Query
- **Validation** - Zod
- **Development** - TypeScript, ESLint, Prettier

## 🚀 Deployment

The project is configured for deployment on:
- Vercel (recommended for Next.js)
- Netlify
- Self-hosted Node.js servers

```bash
npm run build
npm run start
```

## 📄 License

MIT

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Support

For issues and questions, please open an issue on GitHub.

---

**Built with ❤️ using Next.js and modern web technologies**
