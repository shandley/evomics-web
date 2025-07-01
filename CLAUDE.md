# Evomics Web Components

## Project Overview
This repository contains standalone interactive web components for evomics.org, designed to enhance user experience through modern, data-driven interfaces. These components are built to be embedded within the existing WordPress site while leveraging GitHub Pages for hosting.

## Current Components

### 1. Interactive FAQ System ✅ (In Development)
- **Purpose**: Replace static FAQ page with smart, searchable interface
- **Status**: Primary development focus
- **Features**: Search, filtering, voting, view tracking
- **Location**: `/src/apps/faq`

### 2. Budget Calculator 💰 (Planned)
- **Purpose**: Help participants estimate workshop costs
- **Status**: Next in queue
- **Features**: Currency conversion, accommodation options, travel estimates
- **Location**: `/src/apps/budget-calculator`

### 3. Workshop Countdown Dashboard ⏰ (Planned)
- **Purpose**: Create urgency and track important deadlines
- **Status**: Phase 1 completion
- **Features**: Live countdowns, milestone tracking, social sharing
- **Location**: `/src/apps/countdown`

## Technology Stack
- **Framework**: React 18 with TypeScript
- **Styling**: CSS Modules + Tailwind CSS (planned)
- **Search**: Fuse.js for fuzzy search
- **Icons**: Lucide React
- **Routing**: React Router v6
- **Deployment**: GitHub Pages

## Development Commands

```bash
# Install dependencies
npm install

# Start development server
npm start

# Build for production
npm run build

# Run tests
npm test

# Deploy to GitHub Pages
npm run deploy
```

## Project Structure

```
evomics-web/
├── src/
│   ├── apps/                    # Individual applications
│   │   ├── faq/                # Interactive FAQ system
│   │   ├── budget-calculator/  # Workshop budget calculator
│   │   └── countdown/          # Countdown dashboard
│   ├── shared/                 # Shared resources
│   │   ├── components/         # Reusable UI components
│   │   ├── hooks/             # Custom React hooks
│   │   ├── styles/            # Global styles and themes
│   │   └── types/             # TypeScript type definitions
│   └── App.tsx                # Main app router
└── public/                    # Static assets
```

## Integration with WordPress

Components are designed to be embedded via Web Components or iframes:

```html
<!-- Example WordPress integration -->
<div id="evomics-faq"></div>
<script src="https://shandley.github.io/evomics-web/faq-embed.js"></script>
```

## Design Principles
- **Standalone**: Each component works independently
- **Responsive**: Mobile-first design approach
- **Accessible**: WCAG 2.1 AA compliance
- **Performance**: Lazy loading and code splitting
- **Maintainable**: Clear component structure and documentation

## Data Management
- FAQ data: JSON files in `/src/apps/faq/data/`
- Budget data: Static configuration files
- Countdown data: Workshop dates from JSON

## Deployment
The site is automatically deployed to GitHub Pages on push to main branch:
- URL: https://shandley.github.io/evomics-web/

## Component Status

| Component | Status | Priority | Complexity |
|-----------|--------|----------|------------|
| FAQ System | 🟡 In Progress | High | Medium |
| Budget Calculator | 📋 Planned | High | Medium |
| Countdown Dashboard | 📋 Planned | Medium | Low |

## Related Projects
- **evomics-faculty**: Faculty directory and workshop archives (https://github.com/shandley/evomics-faculty)
- **evomics.org**: Main WordPress site

## Development Guidelines

### Component Creation
1. Create new directory in `/src/apps/`
2. Include README.md with component documentation
3. Use shared components from `/src/shared/`
4. Implement responsive design
5. Add to main router in App.tsx

### Code Style
- Use TypeScript for type safety
- Follow React best practices
- Implement error boundaries
- Write unit tests for utilities
- Use semantic HTML

### Performance
- Implement lazy loading for routes
- Optimize images and assets
- Use React.memo for expensive components
- Monitor bundle size

## Future Components
Based on GITHUB_PAGES_COMPONENTS.md:
- Alumni Success Stories
- Workshop Photo Gallery
- Prerequisites Checker
- Certificate Verification

## Contact
For questions or contributions, please open an issue or pull request.