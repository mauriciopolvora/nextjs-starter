# Modern Next.js Starter Template

A beautifully crafted, production-ready Next.js starter template with all the essential tools and best practices baked in.

## ✨ Features

### Core Framework
- **Next.js 16** with App Router for modern, scalable React applications
- **React 19** with the latest features and optimizations
- **React Compiler** enabled by default for improved performance
- **TypeScript** with strict type checking for maximum code safety

### Styling & UI
- **Tailwind CSS 4** with PostCSS for modern utility-first styling
- **TailwindCSS Merge** for intelligent class name merging
- **CVA (Class Variance Authority)** for composable component variants
- **Lucide React** with 500+ beautiful, customizable icons
- **Animation utilities** with tw-animate-css for smooth transitions

### Theme Management
- **Dark/Light mode support** with next-themes
- **System preference detection** with fallback to light theme
- **Smooth transitions** without hydration issues
- **Pre-built ModeToggle component** for easy theme switching

### Developer Experience
- **Biome** for fast, comprehensive linting and formatting
- **Husky** pre-commit hooks for code quality assurance
- **ESLint-inspired rules** with React and Next.js best practices
- **Accessibility-first** linting rules enforced by default
- **Path aliases** (`@/*`) for cleaner imports

### Fonts
- **Poppins** (400, 500) for UI text
- **JetBrains Mono** for code and monospace elements
- Optimized with Next.js Font Optimization

### Code Quality
- Strict TypeScript configuration with null checks
- Automatic import organization with Biome
- Comprehensive linting for Next.js and React patterns
- Accessibility compliance rules built-in

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ or Bun
- npm, yarn, pnpm, or bun package manager

### Installation

1. **Clone or use as template**
```bash
git clone <repository-url>
cd film-list-v2
```

2. **Install dependencies**
```bash
bun install
# or
npm install
```

3. **Start development server**
```bash
bun dev
# or
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the app.

## 📚 Available Scripts

| Command | Description |
|---------|-------------|
| `bun dev` | Start development server with hot reload |
| `bun build` | Build optimized production bundle |
| `bun start` | Start production server |
| `bun run lint` | Run Biome linter and formatter check |
| `bun run format` | Format code with Biome |

## 🏗️ Project Structure

```
src/
├── app/
│   ├── layout.tsx          # Root layout with theme provider
│   ├── page.tsx            # Home page
│   ├── globals.css         # Global styles
│   └── favicon.ico
├── components/
│   ├── theme-provider.tsx  # next-themes wrapper
│   └── mode-toggle.tsx     # Dark/light mode toggle button
└── lib/
    └── utils.ts            # Utility functions
```

## 🎨 Customization

### Colors & Theme
Edit your Tailwind configuration to customize the color scheme:
```bash
# Update tailwind.config.ts
```

### Fonts
Modify fonts in `src/app/layout.tsx`:
- Change font families
- Adjust font weights
- Configure subsets

### Icons
Browse available icons at [lucide.dev](https://lucide.dev) and import as needed:
```tsx
import { Heart, Star, Settings } from "lucide-react";
```

## 🔧 Configuration Files

- **`next.config.ts`** - Next.js configuration (React Compiler enabled)
- **`biome.json`** - Linter and formatter settings
- **`tsconfig.json`** - TypeScript compiler options
- **`components.json`** - shadcn/ui component registry (if using)
- **`postcss.config.mjs`** - PostCSS configuration for Tailwind

## 🧩 Components Ready to Use

### ModeToggle
A pre-built dark/light mode toggle component:
```tsx
import { ModeToggle } from "@/components/mode-toggle";

export default function Header() {
  return (
    <div>
      <ModeToggle />
    </div>
  );
}
```

### ThemeProvider
Wraps your app with theme management:
```tsx
import { ThemeProvider } from "@/components/theme-provider";

// Already configured in root layout
<ThemeProvider attribute="class" defaultTheme="system" enableSystem>
  {children}
</ThemeProvider>
```

## 📦 Dependencies

### Production
- `next` (16.0.0) - React framework
- `react` (19.2.0) - UI library
- `react-dom` (19.2.0) - React DOM utilities
- `next-themes` (0.4.3) - Theme management
- `tailwindcss` (4) - Utility CSS framework
- `lucide-react` (0.548.0) - Icon library
- `class-variance-authority` (0.7.1) - Component variants
- `clsx` (2.1.1) - Class name utilities
- `tailwind-merge` (3.3.1) - Smart class merging

### Development
- `@biomejs/biome` (2.3.0) - Linter & formatter
- `typescript` (5) - Type safety
- `@tailwindcss/postcss` (4) - Tailwind PostCSS
- `babel-plugin-react-compiler` (1.0.0) - React compilation
- `husky` (9.1.7) - Git hooks
- `tw-animate-css` (1.4.0) - Animation utilities

## ✅ Best Practices Included

- ✨ **Accessibility-first** - WCAG compliant components
- 🎯 **Type-safe** - Strict TypeScript configuration
- 📱 **Responsive** - Mobile-first CSS design
- ⚡ **Optimized** - React Compiler for performance
- 🛡️ **Secure** - Next.js security best practices
- 📊 **Linted** - Comprehensive code quality checks
- 🎨 **Dark mode** - Beautiful light and dark themes

## 🚀 Deployment

### Vercel (Recommended)
```bash
vercel deploy
```

### Docker
```dockerfile
FROM node:18-alpine
WORKDIR /app
COPY . .
RUN npm install
RUN npm run build
CMD ["npm", "start"]
```

### Other Platforms
This is a standard Next.js app and can be deployed to any platform that supports Node.js:
- Netlify
- AWS
- Google Cloud
- DigitalOcean
- Railway
- Render

## 📖 Learning Resources

- [Next.js Documentation](https://nextjs.org/docs) - Official Next.js docs
- [React Documentation](https://react.dev) - React guides and API reference
- [Tailwind CSS](https://tailwindcss.com/docs) - Utility-first CSS framework
- [TypeScript Handbook](https://www.typescriptlang.org/docs/) - TypeScript learning

## 🤝 Contributing

Feel free to fork and customize this starter for your projects!

## 📝 License

MIT License - Feel free to use this template for personal or commercial projects.

---

**Happy coding! 🚀**
