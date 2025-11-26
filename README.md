# Creative Technologist Portfolio

A scroll-based narrative portfolio website with generative p5.js visuals that evolve as you tell your story.

## 🚀 Quick Start

1. **Open `index.html` in a browser**
   - No build process needed
   - Works locally or deployed

2. **Customize Your Content**
   - Edit text directly in `index.html`
   - Replace placeholder project cards
   - Update contact links

## 📁 File Structure

```
portfolio/
├── index.html              # Main HTML structure
├── css/
│   ├── reset.css          # CSS reset
│   ├── main.css           # Core styles & design system
│   └── responsive.css     # Mobile/tablet breakpoints
├── js/
│   ├── path-sketch.js     # p5.js generative path
│   ├── scroll-controller.js # Scroll tracking & state management
│   └── ui.js              # Navigation & interactions
└── README.md
```

## ✏️ Customization Guide

### 1. Update Your Information

**In `index.html`, find and replace:**

- `Your Name` → Your actual name
- `Creative Technologist` → Your title/role
- Email, LinkedIn, GitHub links in the contact section

### 2. Add Your Story

**Replace placeholder text in the Story section:**

The story is divided into 4 blocks:
1. **Where I Started** - Your technical background
2. **The Questions** - What made you curious about creative work
3. **The Transformation** - Your journey into digital media
4. **Where I Am Now** - Your current position/philosophy

### 3. Add Your Projects

**Each project card needs:**
- Project image (replace `.project-placeholder`)
- Title
- Description (1-2 sentences)
- Tags (technology/category)

**Example:**
```html
<article class="project-card">
    <div class="project-image">
        <img src="assets/projects/your-project.jpg" alt="Project Name">
    </div>
    <div class="project-info">
        <h3 class="project-title">Living History</h3>
        <p class="project-description">Interactive p5.js experience bringing century-old media to life.</p>
        <div class="project-tags">
            <span class="tag">Creative Coding</span>
            <span class="tag">p5.js</span>
        </div>
    </div>
</article>
```

## 🎨 Design System

### Colors

The site uses a **high-contrast black/white base** with **accent colors that evolve:**

- **Structure** (0-25% scroll): Electric Blue `#00A8FF`
- **Friction** (25-50% scroll): Warm Orange `#FF6B35`
- **Flow** (50-75% scroll): Cyan `#00FFC8` + Magenta `#FF0080`
- **Synthesis** (75-100%): Blended gradient

### Typography

- **Headlines**: Inter Display (700 weight)
- **Body**: Inter (400 weight)
- **Tags/Labels**: JetBrains Mono (monospace)

### Spacing

The site uses a consistent spacing scale:
- xs: 8px
- sm: 16px
- md: 32px
- lg: 64px
- xl: 128px

## 🎭 The Generative Path

The p5.js background path transforms through **4 visual states** matching your narrative:

### State 1: Structure
- Straight, grid-aligned lines
- Minimal movement
- Blue accent
- **Represents:** Early technical career

### State 2: Friction
- Curved lines (sine waves)
- Mild Perlin noise
- Blue → Orange gradient
- Occasional breaks/gaps
- **Represents:** Questions and tension

### State 3: Flow
- Organic curves
- High Perlin noise
- Particle trails
- Mouse-responsive
- Cyan + Magenta colors
- **Represents:** Creative transformation

### State 4: Synthesis
- Smooth flowing waves
- All colors blended
- Balanced structure + fluidity
- **Represents:** Integrated identity

## 🔧 Advanced Customization

### Modify the p5.js Path

Edit `js/path-sketch.js`:

- `numPoints`: Number of points in the path (default: 100)
- `amplitude`: Height of waves
- `frequency`: Speed of oscillation
- Color transitions in `updateColors()`
- Movement algorithms in `updatePathPoints()`

### Adjust Scroll Behavior

Edit `js/scroll-controller.js`:

- Scroll smoothness
- Section transition timing
- Navigation dot update logic

### Add Project Interactions

Edit `js/ui.js`:

- Project card click handlers
- Custom animations
- Additional interactive elements

## 📱 Responsive Design

The site is mobile-first and fully responsive:
- Tablet: ≤768px
- Mobile: ≤480px
- Landscape adjustments included

## 🚢 Deployment

### Option 1: GitHub Pages
1. Push to GitHub
2. Enable Pages in repo settings
3. Deploy from main branch

### Option 2: Netlify/Vercel
1. Drag & drop the folder
2. Instant deployment
3. Custom domain support

### Option 3: Traditional Hosting
1. Upload all files via FTP
2. Maintain folder structure
3. Ensure all paths are relative

## 🔮 Future Enhancements

**Ready to add later:**
- [ ] AI Story Guide (chat interface)
- [ ] Project case study pages
- [ ] A-Frame/Three.js 3D elements
- [ ] Blog section
- [ ] Dark/light mode toggle
- [ ] Analytics integration

## 🐛 Troubleshooting

**p5.js not loading?**
- Check internet connection (uses CDN)
- Verify p5.js script tag in HTML

**Path not animating?**
- Open browser console for errors
- Check that `scroll-controller.js` loads after `path-sketch.js`

**Layout broken on mobile?**
- Clear browser cache
- Check responsive.css is loading

## 📝 License

Personal portfolio template - feel free to customize and use for your own work.

---

**Need help?** Check browser console for errors or review the code comments.
