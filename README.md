# GREAN Energy - Interactive Solar Inverter Demo

A cutting-edge Next.js application showcasing GREAN's solar energy solutions with an interactive 3D inverter demonstration, comprehensive energy management system, and responsive design optimized for all devices.

## 🚀 Deployment Ready

This project has been cleaned up and optimized for production deployment:
- ✅ All unused components and files removed
- ✅ TypeScript errors resolved
- ✅ Build process optimized
- ✅ Responsive design verified across all devices
- ✅ Navigation and functionality tested
- ✅ Netlify configuration ready
- ✅ GitHub deployment prepared

## Features

- Dashboard for energy production and consumption metrics
- Interactive visualizations of energy data
- User management and preferences
- Mobile-responsive design
- Dark/light mode support

## Technologies Used

- [Next.js](https://nextjs.org/) - React framework
- [React](https://reactjs.org/) - UI library
- [TailwindCSS](https://tailwindcss.com/) - Utility-first CSS framework
- [Radix UI](https://www.radix-ui.com/) - Headless UI components
- [Recharts](https://recharts.org/) - Composable charting library
- [Zustand](https://github.com/pmndrs/zustand) - State management
- [GSAP](https://greensock.com/) - Animation library
- [Framer Motion](https://www.framer.com/motion/) - Animation library

## Getting Started

### Prerequisites

- Node.js 18.0.0 or later
- npm or yarn

### Installation

1. Clone the repository

   ```
   git clone https://github.com/yourusername/grean-energy.git
   cd grean-energy
   ```

2. Install dependencies

   ```
   npm install
   # or
   yarn install
   ```

3. Configure environment variables

   ```
   cp .env.example .env.local
   # Edit .env.local with your Spline scene URL
   ```

4. Run the development server

   ```
   npm run dev
   # or
   yarn dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## Build for Production

```bash
# Standard build
npm run build

# Production build (optimized for deployment)
npm run build:production

# Clean build (removes cache first)
npm run build:clean
```

## Deployment

### Netlify Deployment

This project is optimized for Netlify deployment with the following configuration:

**Quick Deploy:**

1. Connect your Git repository to Netlify
2. Build settings are automatically configured via `netlify.toml`:
   - Build command: `npm run build:production`
   - Publish directory: `out`
   - Node.js version: 18
3. Configure environment variables (see `.env.example`)
4. Deploy!

**Automatic Configuration:**
- ✅ Next.js plugin enabled
- ✅ Build optimizations configured
- ✅ Redirects for SPA routing
- ✅ API routes support

**Environment Variables Required:**

- `NEXT_PUBLIC_SPLINE_SCENE`: Your Spline 3D scene URL
- `NODE_ENV`: `production`

For detailed deployment instructions, see [DEPLOYMENT.md](./DEPLOYMENT.md).

## Project Cleanup

✅ **Project has been thoroughly cleaned and optimized!**

**Recent comprehensive cleanup included:**
- ✅ Removed backup files (page.tsx.bak)
- ✅ Consolidated mobile detection hooks (eliminated duplication)
- ✅ Merged CSS globals files (app/globals.css + styles/globals.css → styles/globals.css)
- ✅ Eliminated theme provider duplication (useBrandTheme now wraps useTheme)
- ✅ Removed redundant responsive.css file (integrated into globals.css)
- ✅ Fixed Tailwind config references to non-existent directories
- ✅ Cleaned up build artifacts and temporary files
- ✅ Optimized bundle size and eliminated conflicts

To perform additional cleanup:

```bash
npm run clean && npm install
```

## Documentation

📚 **Comprehensive documentation is available in the [docs/](./docs/) folder:**

- **[Project Reports](./docs/README.md)**: Cleanup, upgrades, and enhancement reports
- **[Component Documentation](./docs/README.md)**: Detailed component implementation guides
- **[Technical Guides](./docs/README.md)**: Performance optimization and build documentation
- **[Brand Guidelines](./docs/grean-world-brand-assets-v2.0-complete/)**: Complete brand asset library and design system
- **Component Documentation**: Inline JSDoc comments throughout the codebase

**Quick Links:**
- [Brand Implementation Report](./docs/BRAND_GUIDELINES_LIVE_IMPLEMENTATION.md) - Complete implementation details
- [Cleanup Report](./docs/CLEANUP_REPORT.md) - Project optimization details
- [Component Upgrades](./docs/COMPONENT_UPGRADE_REPORT.md) - Recent component improvements
- [GreenIntro Enhancement](./docs/GREENINTRO_ENHANCEMENT_SUMMARY.md) - Visual enhancement details

## 🎨 Brand Guidelines

**GREAN WORLD Brand Guidelines** - Available in the docs folder:

### **🎯 Brand Standards:**
- **Primary Color**: `#3DD56D` (GREAN Green)
- **Secondary Color**: `#2bb757` (Forest Green)
- **Accent Color**: `#23A455` (Deep Green)
- **Typography**: Complete Tailwind-based hierarchy
- **Components**: Official GreanButton and GreanCard implementations
- **Themes**: Dual light/dark mode support with automatic switching

### **🚀 Quick Implementation:**
```jsx
import { GreanButton } from '@/components/ui/grean-button'
import { GreanCard } from '@/components/ui/grean-card'

// Use official brand components
<GreanButton variant="primary" size="lg">Get Started</GreanButton>
<GreanCard pattern="dots" gradient>Content</GreanCard>
```

## Key Features

### 3D Interactive Model

- **Spline Integration**: Interactive 3D energy system visualization
- **Real-time Animations**: Dynamic energy flow and component interactions
- **Error Handling**: Robust error recovery with user-friendly messages
- **Performance Optimized**: Efficient loading and rendering

### Energy System Components

- **Solar Panels**: Interactive solar energy generation nodes
- **Inverters**: Power conversion system visualization
- **Smart Switches**: Controllable energy distribution points
- **Battery Storage**: Energy storage level indicators

### User Experience

- **Responsive Design**: Optimized for desktop, tablet, and mobile
- **Audio Feedback**: Sound effects for system interactions
- **Loading States**: Professional loading animations
- **Error Recovery**: "Try Again" functionality for failed loads

## 🚀 Deployment

### GitHub Deployment

1. **Push to GitHub**:
   ```bash
   git add .
   git commit -m "Production ready: Cleaned up project for deployment"
   git push origin main
   ```

### Netlify Deployment

1. **Connect to Netlify**:
   - Go to [Netlify](https://netlify.com)
   - Click "New site from Git"
   - Connect your GitHub repository

2. **Build Settings**:
   - Build command: `npm run netlify:build`
   - Publish directory: `.next`
   - Node version: `22`

3. **Environment Variables** (if needed):
   - `NODE_ENV=production`
   - `NEXT_TELEMETRY_DISABLED=1`

4. **Deploy**:
   - Click "Deploy site"
   - Your site will be available at `https://your-site-name.netlify.app`

### Manual Deployment Check

Run the deployment check script before deploying:
```bash
npm run deploy:check
```

This will verify all required files and configurations are in place.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Benefits of Cleanup

- **Reduced Package Size**: Smaller `node_modules` folder
- **Faster Installation**: Fewer packages to download and install
- **Reduced Security Risks**: Fewer dependencies means fewer potential vulnerabilities
- **Better Maintainability**: Clearer understanding of the project's actual dependencies
- **Improved Build Performance**: Less code to process during builds
