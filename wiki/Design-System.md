# Design System Guidelines

## Color Palette

### Primary Colors
```css
:root {
  --primary-green: #2EA44F;     /* Brand color */
  --primary-dark: #24292E;      /* Text color */
  --primary-light: #FFFFFF;     /* Background */
  --accent-blue: #0366D6;       /* Links */
}
```

### Status Colors
```css
:root {
  --success: #28A745;
  --warning: #FFA500;
  --error: #DC3545;
  --info: #17A2B8;
}
```

## Typography

### Font Stack
```css
:root {
  --system-fonts: -apple-system, BlinkMacSystemFont, 'Segoe UI', 
                  Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
  --mono-fonts: SFMono-Regular, Consolas, 'Liberation Mono', Menlo, monospace;
}
```

### Text Sizes
```css
:root {
  --text-xs: 0.75rem;    /* 12px */
  --text-sm: 0.875rem;   /* 14px */
  --text-base: 1rem;     /* 16px */
  --text-lg: 1.125rem;   /* 18px */
  --text-xl: 1.25rem;    /* 20px */
  --text-2xl: 1.5rem;    /* 24px */
}
```

## Components

### Buttons
```html
<!-- Primary Button -->
<button class="btn btn-primary">
  View Project
</button>

<!-- Secondary Button -->
<button class="btn btn-secondary">
  Learn More
</button>
```

```css
.btn {
  padding: 0.5rem 1rem;
  border-radius: 6px;
  font-weight: 500;
  transition: all 0.2s;
}

.btn-primary {
  background: var(--primary-green);
  color: var(--primary-light);
}

.btn-secondary {
  border: 1px solid var(--primary-green);
  color: var(--primary-green);
}
```

### Cards
```html
<article class="card">
  <img src="preview.webp" alt="Project Preview">
  <div class="card-content">
    <h3>Project Title</h3>
    <p>Project description</p>
  </div>
</article>
```

```css
.card {
  border: 1px solid #e1e4e8;
  border-radius: 6px;
  overflow: hidden;
  transition: transform 0.2s;
}

.card:hover {
  transform: translateY(-4px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}
```

## Layout

### Grid System
```css
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
}
```

### Spacing Scale
```css
:root {
  --space-1: 0.25rem;   /* 4px */
  --space-2: 0.5rem;    /* 8px */
  --space-3: 0.75rem;   /* 12px */
  --space-4: 1rem;      /* 16px */
  --space-6: 1.5rem;    /* 24px */
  --space-8: 2rem;      /* 32px */
}
```

## Brand Elements

### GitHub Corner
```html
<a href="https://github.com/Lovingthemoo-74" class="github-corner">
  <svg width="80" height="80" viewBox="0 0 250 250">
    <!-- SVG path data -->
  </svg>
</a>
```

### Contact Badge
```html
<div class="contact-badge">
  <img src="https://img.shields.io/badge/-lovingthemoo%40gmail.com-lightgrey?logo=gmail" alt="Email">
</div>
```

## Responsive Design

### Breakpoints
```css
:root {
  --mobile: 375px;
  --tablet: 768px;
  --laptop: 1024px;
  --desktop: 1280px;
}

@media (min-width: 768px) {
  /* Tablet styles */
}

@media (min-width: 1024px) {
  /* Desktop styles */
}
```

## Animation

### Transitions
```css
:root {
  --transition-fast: 150ms ease;
  --transition-normal: 250ms ease;
  --transition-slow: 350ms ease;
}

.animated-element {
  transition: all var(--transition-normal);
}
```

## Contact Information
For design system inquiries:
- GitHub: [@Lovingthemoo-74](https://github.com/Lovingthemoo-74)
- Email: [lovingthemoo@gmail.com](mailto:lovingthemoo@gmail.com)