# Cloud Native IT Solutions - ERP Branding Guide

## 🎨 Overview

This document explains how the **Oracle Redwood-inspired** Cloud Native IT Solutions branding has been implemented in your ERPNext system, featuring modern glassmorphism effects and a professional pastel color palette.

---

## 📁 Files Modified/Created

### ✅ Modified Files
1. **[hooks.py](design_app/hooks.py)**
   - Updated app metadata with company information
   - Added new CSS file for branding

2. **[css_varaibles.scss](design_app/public/css/css_varaibles.scss)**
   - Added CNIT brand color variables (Oracle Redwood-inspired)
   - Updated primary brand color to Modern Purple-Blue (#667EEA)
   - Added secondary Deep Purple (#764BA2) and Modern Green accent (#48BB78)

3. **[style.css](design_app/public/css/style.css)**
   - Updated tab colors to CNIT primary
   - Fixed active state colors

4. **[script.js](design_app/public/js/script.js)**
   - Added accessibility attributes
   - Improved HTML semantics

### ✅ New Files Created
1. **[cnit-branding.css](design_app/public/css/cnit-branding.css)** (940+ lines)
   - Oracle Redwood-inspired glassmorphism theme
   - Pastel color palette implementation
   - Modern UI elements (glass cards, gradient text, animations)
   - Responsive and accessible design

2. **[cnit-logo-white.svg](design_app/public/images/cnit-logo-white.svg)**
   - White logo for dark sidebar
   - **PLACEHOLDER - Replace with your actual logo**

3. **[cnit-logo.svg](design_app/public/images/cnit-logo.svg)**
   - Dark logo for light backgrounds
   - **PLACEHOLDER - Replace with your actual logo**

---

## 🎨 Brand Color Palette - Oracle Redwood Inspired

### Primary Colors
```css
--cnit-primary: #667EEA;     /* Modern Purple-Blue - Innovation & Tech */
--cnit-secondary: #764BA2;   /* Deep Purple - Professional Elegance */
--cnit-accent: #48BB78;      /* Modern Green - Growth/Success */
--cnit-dark: #2D3748;        /* Slate Gray - Professional */
--cnit-light: #F7FAFC;       /* Almost White - Clean */
```

### Gradient
```css
--cnit-gradient: linear-gradient(135deg, #667EEA 0%, #764BA2 100%);
```

### Pastel Colors for Glassmorphism
```css
--pastel-blue: #A8D5E2;      /* Dashboard Widget 1 */
--pastel-purple: #C5B9E8;    /* Dashboard Widget 3 */
--pastel-pink: #FFB5C2;      /* Accent Elements */
--pastel-green: #B8E6D5;     /* Dashboard Widget 2 */
--pastel-peach: #FFD4B2;     /* Accent Elements */
--pastel-yellow: #FFF4A3;    /* Highlights */
```

### Glassmorphism Variables
```css
--glass-bg: rgba(255, 255, 255, 0.95);           /* Background */
--glass-border: rgba(255, 255, 255, 0.18);       /* Border */
--glass-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.15);  /* Shadow */
```

### Usage Examples
- **Primary Purple-Blue (#667EEA)**: Buttons, links, active states, gradients
- **Secondary Deep Purple (#764BA2)**: Gradients, sidebar backgrounds
- **Accent Modern Green (#48BB78)**: Success states, positive indicators
- **Slate Gray (#2D3748)**: Text, dark elements
- **Pastel Colors**: Dashboard widgets, cards, glass effects
- **Light (#F7FAFC)**: Backgrounds, content areas

---

## 🖼️ Logo Placement

### Where Logos Appear

#### 1. Sidebar Logo (White Version)
- **Location**: Top of left sidebar
- **File**: `cnit-logo-white.svg`
- **Size**: Auto-scaled to 90% width within glass card
- **Background**: Purple-blue gradient (#667EEA to #764BA2) with glassmorphism effect

#### 2. Mobile Menu Logo
- **Location**: Top navbar on mobile
- **File**: Uses Frappe's `app_logo_url`
- **Size**: 55px width

#### 3. Login Page (Optional)
- **File**: Configure in Frappe's Website Settings
- **Recommendation**: Use `cnit-logo.svg` (dark version)

### How to Replace Placeholder Logos

**Replace the placeholder SVG files with your actual company logos:**

```bash
# Navigate to images directory
cd design_app/public/images/

# Replace with your logos (keep same filenames)
# Option 1: Copy your logo files
cp /path/to/your/logo-white.svg cnit-logo-white.svg
cp /path/to/your/logo-dark.svg cnit-logo.svg

# Option 2: If you have PNG files, convert them
# (Install ImageMagick first: brew install imagemagick)
convert your-logo-white.png cnit-logo-white.svg
convert your-logo-dark.png cnit-logo.svg
```

**Logo Requirements:**
- **Format**: SVG preferred (scalable, crisp at any size)
- **Fallback**: PNG (300 DPI minimum)
- **White Logo**: For dark backgrounds (sidebar)
- **Dark Logo**: For light backgrounds (login, reports)
- **Dimensions**: 200x80px recommended (will scale automatically)
- **Transparent Background**: Required for best results

---

## 🎯 Branding Applied To - Oracle Redwood Design

### 1. Sidebar Navigation (Glassmorphism)
- ✅ **Purple-blue gradient background** (#667EEA to #764BA2)
- ✅ **Glass-effect user card** with backdrop blur and rounded corners
- ✅ Logo displayed within glass card
- ✅ Company tagline below user info
- ✅ **Menu items as glass cards** with hover animations
- ✅ Smooth transitions and scaling effects
- ✅ Box shadows for depth perception

### 2. Tabs & Navigation
- ✅ Active tabs use Modern Purple-Blue (#667EEA)
- ✅ Smooth hover transitions with brand colors
- ✅ Border highlights in primary color

### 3. Dashboard Widgets (Glass Cards)
- ✅ **Glass-effect cards** with backdrop blur
- ✅ **Gradient text for numbers**:
  - Widget 1: Pastel Blue to Primary Purple-Blue
  - Widget 2: Pastel Green to Accent Green
  - Widget 3: Pastel Purple to Secondary Purple
- ✅ Colored top borders (3px) for visual distinction
- ✅ Hover effects with subtle glow and scale
- ✅ Rounded corners (20px) for modern look

### 4. Buttons & Controls
- ✅ **Primary buttons**: Purple-blue gradient with shine animation
- ✅ **Secondary buttons**: Glass effect with borders
- ✅ Hover states with scale transformation (1.05x)
- ✅ Focus states with CNIT primary glow
- ✅ Smooth transitions (all properties 0.3s ease)

### 5. Forms & Inputs
- ✅ **Rounded inputs** (12px border-radius)
- ✅ **Pastel background gradients** for containers
- ✅ Focus borders: CNIT primary with 3px width
- ✅ Focus glow: CNIT primary with transparency
- ✅ Validation states with brand colors

### 6. Tables
- ✅ **Pastel gradient headers** (blue to purple)
- ✅ **Glass-effect rows** with hover states
- ✅ Rounded corners (15px)
- ✅ Border styling with glass borders

### 7. Modals & Dialogs
- ✅ **Glassmorphism effect** with backdrop blur
- ✅ Rounded corners (25px)
- ✅ Box shadows for elevation
- ✅ Smooth animations

### 8. Scrollbars
- ✅ Custom scrollbar with CNIT gradient
- ✅ Hover state in primary color
- ✅ Smooth transitions

### 9. Page Background
- ✅ **Subtle pastel gradient** for main content area
- ✅ Multi-color gradient (light gray → pastel blue → pastel purple)
- ✅ Clean, professional appearance

### 10. Footer
- ✅ Company copyright notice
- ✅ Subtle gradient background
- ✅ Professional styling with opacity

---

## 🚀 Installation & Setup

### Step 1: Install the App
```bash
# Navigate to your Frappe bench
cd /path/to/frappe-bench

# Install the app (if not already installed)
bench --site your-site-name install-app design_app

# Clear cache and build assets
bench --site your-site-name clear-cache
bench build --app design_app
```

### Step 2: Replace Logo Files
```bash
# Copy your actual logo files to replace placeholders
cp /path/to/your/logo-white.svg apps/design_app/design_app/public/images/cnit-logo-white.svg
cp /path/to/your/logo-dark.svg apps/design_app/design_app/public/images/cnit-logo.svg
```

### Step 3: Configure System Settings
```bash
# Set your company logo in Frappe
bench --site your-site-name set-config app_logo_url "/assets/design_app/images/cnit-logo.svg"
```

### Step 4: Restart and Clear Cache
```bash
# Restart Frappe
bench restart

# Clear browser cache or hard refresh (Ctrl+Shift+R / Cmd+Shift+R)
```

---

## 🎨 Customization Guide

### Changing Brand Colors

Edit [css_varaibles.scss](design_app/public/css/css_varaibles.scss) (Lines 5-11):

```scss
--cnit-primary: #YOUR_PRIMARY_COLOR;
--cnit-secondary: #YOUR_SECONDARY_COLOR;
--cnit-accent: #YOUR_ACCENT_COLOR;
```

Then rebuild:
```bash
bench build --app design_app
bench restart
```

### Modifying Company Tagline

Edit [cnit-branding.css](design_app/public/css/cnit-branding.css) (Line 28):

```css
.userlogo .emailtext::after {
    content: 'Your Custom Tagline Here';
}
```

### Updating Footer Text

Edit [cnit-branding.css](design_app/public/css/cnit-branding.css) (Line 201):

```css
.layout-footer::after {
    content: '© 2025 Your Company Name | Custom Text';
}
```

### Adjusting Logo Size

Edit [cnit-branding.css](design_app/public/css/cnit-branding.css) (Lines 18-24):

```css
.userlogo::before {
    width: 90%;        /* Adjust percentage */
    height: 70px;      /* Adjust height */
}
```

---

## 📱 Responsive Design

The branding is fully responsive and adapts to:

### Desktop (> 768px)
- Full sidebar with logo and company info
- All branding elements visible
- Smooth transitions and hover effects

### Tablet (768px - 1024px)
- Collapsible sidebar
- Logo scales appropriately
- Touch-friendly interactive elements

### Mobile (< 768px)
- Compact sidebar
- Smaller logo in navbar
- Optimized footer text
- Mobile menu for navigation

---

## ♿ Accessibility Features

### Implemented Accessibility
- ✅ ARIA labels on interactive elements
- ✅ High contrast mode support
- ✅ Reduced motion support for animations
- ✅ Keyboard navigation friendly
- ✅ Screen reader compatible
- ✅ Focus indicators on all interactive elements
- ✅ Semantic HTML structure

### Testing Accessibility
```bash
# Use browser DevTools Lighthouse
# Check for: Accessibility score > 90
# Test keyboard navigation (Tab, Enter, Esc keys)
# Test with screen reader (NVDA, JAWS, VoiceOver)
```

---

## 🖨️ Print Styles

When printing documents:
- Branding elements are hidden
- Content is optimized for paper
- Colors are adjusted for black & white printing
- Logo watermark removed (configurable)

---

## 🔧 Troubleshooting

### Logo Not Showing
**Problem**: Logo placeholder not displaying

**Solutions**:
1. Check file path is correct: `/assets/design_app/images/cnit-logo-white.svg`
2. Clear cache: `bench --site your-site clear-cache`
3. Rebuild assets: `bench build --app design_app`
4. Check file permissions: `chmod 644 design_app/public/images/*.svg`
5. Verify SVG is valid (open in browser directly)

### Colors Not Updating
**Problem**: Brand colors not changing

**Solutions**:
1. Clear browser cache (Ctrl+Shift+R)
2. Rebuild CSS: `bench build --app design_app`
3. Check CSS specificity (use !important if needed)
4. Verify SCSS compiled: Check for errors in console

### Styles Not Loading
**Problem**: Custom styles not applied

**Solutions**:
1. Verify hooks.py includes CSS files
2. Check file names match exactly
3. Rebuild: `bench build --app design_app`
4. Check browser console for 404 errors
5. Verify app is installed: `bench --site your-site list-apps`

### Footer Not Showing
**Problem**: Company footer not visible

**Solutions**:
1. Check if page has `.layout-footer` element
2. Scroll to bottom of page
3. Verify cnit-branding.css is loaded
4. Check browser inspector for CSS conflicts

---

## 📊 Performance Considerations

### CSS Optimization
- Variables used for consistency and performance
- Minimal use of !important
- Efficient selectors
- Transitions use GPU-accelerated properties

### Image Optimization
- SVG logos = vector-based (no quality loss)
- Minimal file sizes
- No external font dependencies
- Lazy loading for images

### Best Practices
- Keep logo files under 50KB
- Use SVG format when possible
- Optimize images before uploading
- Test on slow connections

---

## 🔒 Security Notes

### File Permissions
```bash
# Ensure proper permissions
chmod 644 design_app/public/css/*.css
chmod 644 design_app/public/images/*
```

### Content Security Policy
If you have strict CSP, add:
```
img-src 'self' data: blob:;
style-src 'self' 'unsafe-inline';
```

---

## 📚 Additional Resources

### Frappe Documentation
- [Custom Apps](https://frappeframework.com/docs/user/en/tutorial/custom-app)
- [Theming](https://frappeframework.com/docs/user/en/desk/theming)
- [Hooks](https://frappeframework.com/docs/user/en/python-api/hooks)

### Design Tools
- [Figma](https://figma.com) - Design mockups
- [Coolors](https://coolors.co) - Color palette generator
- [SVG Editor](https://www.svgviewer.dev/) - Edit SVG files online

### Support
For issues or questions:
- Email: info@cloudnative-it.com
- Documentation: [Your docs URL]
- GitHub: [Your repo URL]

---

## 📝 Changelog

### Version 2.0.0 (2025-12-10) - Oracle Redwood Design
- ✅ **Complete redesign** with Oracle Redwood inspiration
- ✅ **Glassmorphism effects** throughout the interface
- ✅ **Pastel color palette** for modern professional look
- ✅ **Purple-blue gradient sidebar** (#667EEA to #764BA2)
- ✅ **Glass-effect cards** for dashboard widgets
- ✅ **Gradient text** for numbers and headings
- ✅ **Rounded corners** (12px-25px) for modern aesthetic
- ✅ **Shine animations** on buttons
- ✅ **Hover transformations** with scale effects
- ✅ **Backdrop blur effects** (blur(10px))
- ✅ **940+ lines of custom CSS**

### Version 1.0.0 (2025-12-10)
- ✅ Initial branding implementation
- ✅ CNIT color palette applied (original Sky Blue theme)
- ✅ Logo placeholders created
- ✅ Responsive design implemented
- ✅ Accessibility features added
- ✅ Documentation completed

---

## 🎯 Next Steps

### Recommended Enhancements

1. **Replace Placeholder Logos**
   - Priority: HIGH
   - Action: Replace SVG files with actual company logos

2. **Test Across Devices**
   - Priority: HIGH
   - Action: Test on desktop, tablet, mobile

3. **User Feedback**
   - Priority: MEDIUM
   - Action: Gather feedback from team members

4. **Additional Pages**
   - Priority: MEDIUM
   - Action: Brand login page, email templates

5. **Dark Mode**
   - Priority: LOW
   - Action: Implement dark theme variant

6. **Animation Polish**
   - Priority: LOW
   - Action: Add micro-interactions

---

## ✅ Checklist

Use this checklist to ensure complete branding:

- [ ] App metadata updated in hooks.py
- [ ] Brand colors defined in css_varaibles.scss
- [ ] Logo files replaced with actual company logos
- [ ] Tested on desktop browser
- [ ] Tested on mobile device
- [ ] Tested on tablet
- [ ] Accessibility verified
- [ ] Print styles tested
- [ ] All team members trained
- [ ] Documentation reviewed
- [ ] Performance optimized
- [ ] Security verified

---

**Last Updated**: 2025-12-10
**Version**: 1.0.0
**Company**: Cloud Native IT Solutions

---

For technical support or customization requests, contact your development team.
