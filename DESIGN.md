# Design System — Anthropic Theme

## Color Tokens

### Primary Colors
- **Dark**: `#141413` — Primary background, text on light
- **Light**: `#faf9f5` — Light backgrounds, fallback text color
- **Text Dark**: `#141413` — Primary text color on light backgrounds

### Neutral Palette
- **Mid Gray**: `#b0aea5` — Secondary text, muted UI
- **Light Gray**: `#e8e6dc` — Borders, subtle backgrounds
- **Border**: `#e8e6dc` — Consistent border color

### Accent Colors (Rotate by Section)
- **Orange**: `#d97757` — Experience section, primary CTA
- **Blue**: `#6a9bcc` — Projects section, secondary actions
- **Green**: `#788c5d` — Skills section, tertiary actions

## Typography

### Headings
- **Font Family**: Poppins (Arial fallback)
- **Weights**: Bold (700) for primary headings, Regular (400) for secondary
- **Sizes**: 24pt+ per Anthropic guidelines
- **Color**: `#141413` (dark) for all headings

### Body Text
- **Font Family**: Lora (Georgia fallback)
- **Weight**: Regular (400)
- **Size**: 16pt base (min 11pt for accessibility)
- **Color**: `#141413` (dark) on light backgrounds
- **Line Height**: 1.8 for readability

### Monospace (UI/Labels)
- **Font Family**: System monospace or Arial (fallback)
- **Use**: Labels, tags, small UI text

## Spacing Scale

### Vertical Spacing
- **Section padding**: 48px top/bottom (desktop), 32px (tablet), 16px (mobile)
- **List item padding**: 24px vertical, 0 horizontal
- **Gap between items**: 1rem

### Responsive Breakpoints
- **Desktop**: 1024px+ (3px accent borders, 48px padding)
- **Tablet**: 768–1023px (3px accent borders, 32px padding)
- **Mobile**: 375–767px (2px accent borders, 16px padding, hamburger nav)

## Component Patterns

### Section Accents
- **Accent Border**: 3px (desktop) or 2px (mobile) left border in section's assigned color
- **Purpose**: Visual organization, not decoration
- **Application**: Experience (orange), Projects (blue), Skills (green)

### Interactive Elements
- **Links**: Color matches section accent
- **Hover**: Underline appears on hover
- **Focus**: Visible 2px outline/ring (WCAG AA minimum)
- **Touch targets**: Minimum 44px on mobile

### Lists & Cards
- **Format**: Linear list layout (no cards for portfolio items)
- **Dividers**: Subtle line between items
- **Density**: Generous vertical spacing, left-aligned
- **Accents**: Left border only, no background fills

### Contact Section
- **Desktop**: Inline layout (email, phone, LinkedIn in row)
- **Mobile**: Stacked layout (single column)
- **Alignment**: Centered
- **Responsive**: Switch at 768px breakpoint

## Accessibility

### Color Contrast
- Dark (#141413) on light (#faf9f5): **17:1 ratio** (WCAG AAA)
- Meets all accessibility standards

### Keyboard Navigation
- All interactive elements keyboard-accessible
- Links/buttons: visible focus ring (2px minimum)
- Tab order: logical, top-to-bottom

### Semantic HTML
- `<h1>`: Page title (hero name)
- `<h2>`: Section headings (Experience, Projects, Skills)
- `<h3>`: Subsection headings (role titles)
- ARIA landmarks on major sections

### Touch Targets
- Minimum 44px height/width on mobile
- Adequate spacing between interactive elements
- No small, hard-to-tap buttons

## Mobile Navigation

### Sticky Mobile Nav
- Fixed position at top (mobile 375px+)
- Hamburger icon triggers menu
- Menu items: links to sections (Experience, Projects, Skills, Contact)
- Smooth scroll to anchor links
- Background: semi-transparent dark with blur

## Visual Hierarchy

### Hero Section
1. **Primary**: Name (largest, Poppins Bold)
2. **Secondary**: Headline (smaller, Poppins Regular)
3. **Tertiary**: Metrics in accent color boxes

### Section Structure
1. **Primary**: Section title (h2, Poppins Bold, dark)
2. **Secondary**: Item titles (h3, Poppins Regular)
3. **Tertiary**: Descriptions & details (Lora, body text)
4. **Accent**: Tags, categories (orange/blue/green left border)

## Font Fallback Chain

```
Headings:  Poppins, Arial, sans-serif
Body:      Lora, Georgia, serif
Monospace: 'Courier New', monospace
```

Ensures consistent rendering across all browsers and systems.

---

**Version**: 1.0  
**Last Updated**: May 14, 2026  
**Theme**: Anthropic Brand Guidelines
