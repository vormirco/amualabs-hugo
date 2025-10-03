# AMUALABS Hugo Site

Component-based Hugo website for AMUALABS - AI Agents & Systems Integration.

## 🚀 Quick Start

```bash
# Install Hugo (if not installed)
brew install hugo

# Clone and start development
git clone <repository-url>
cd hugo-site
hugo server --buildDrafts

# Build for production
hugo --minify
```

## 🏗️ Architecture

### Component System
- **Partials**: Reusable components (header, footer, hero, pillars)
- **Shortcodes**: Complex elements (cards, metrics, CTAs)
- **Layouts**: Template inheritance (base → page-specific)
- **Data Files**: Content management (YAML)

### SCSS Organization
```
assets/scss/
├── base/           # Variables, reset, typography
├── components/     # UI components (buttons, cards, navigation)
├── layout/         # Layout components (header, footer, containers)
├── pages/          # Page-specific styles
└── utilities/      # Responsive, animations
```

## 📦 Deployment

### Cloudflare Pages (Production)
1. Connect GitHub repository to Cloudflare Pages
2. Build command: `hugo --minify`
3. Build output: `public`
4. Hugo version: `0.150.1`

### Local Development
```bash
hugo server --buildDrafts --port 1314
```

### Content Management
- Pages: `content/*.md` (Markdown + Front Matter)
- Data: `data/*.yaml` (Metrics, case studies, services)
- Assets: `themes/amualabs/assets/` (SCSS, JS, images)

## 🛠️ Features
- ✅ Component-based architecture
- ✅ Mobile-first responsive design
- ✅ SEO optimization (meta tags, schema, sitemap)
- ✅ Performance optimized (minified CSS/JS)
- ✅ Git-based deployment workflow
- 🔄 Micro tools integration (Hetzner VPS proxy)

## 🔗 Integration Points
- **Main Site**: Cloudflare Pages (`amualabs.com`)
- **Micro Tools**: Hetzner VPS (`amualabs.com/tools/*`)
- **Analytics**: To be configured
- **Forms**: To be integrated

## 📝 Content Updates
Update content by editing:
- `content/_index.md` - Homepage content
- `content/about.md` - About page
- `content/work.md` - Portfolio page
- `data/metrics.yaml` - Performance metrics
- `data/case_studies.yaml` - Case study data
