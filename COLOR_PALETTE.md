# Cloud Native IT Solutions - Color Palette Reference

## 🎨 Primary Brand Colors

### CNIT Primary - Sky Blue
**Hex**: `#0EA5E9`
**RGB**: `rgb(14, 165, 233)`
**CSS Variable**: `var(--cnit-primary)`

**Usage**:
- Primary buttons
- Active states
- Links
- Tab indicators
- Sidebar selections
- Primary icons

**Preview**:
```
████████████  #0EA5E9
```

---

### CNIT Secondary - Purple
**Hex**: `#8B5CF6`
**RGB**: `rgb(139, 92, 246)`
**CSS Variable**: `var(--cnit-secondary)`

**Usage**:
- Secondary buttons
- Gradient endings
- Accent elements
- Hover states
- Icons

**Preview**:
```
████████████  #8B5CF6
```

---

### CNIT Accent - Green
**Hex**: `#10B981`
**RGB**: `rgb(16, 185, 129)`
**CSS Variable**: `var(--cnit-accent)`

**Usage**:
- Success states
- Positive indicators
- Dashboard widgets
- Completion badges
- Growth metrics

**Preview**:
```
████████████  #10B981
```

---

### CNIT Dark - Slate
**Hex**: `#0F172A`
**RGB**: `rgb(15, 23, 42)`
**CSS Variable**: `var(--cnit-dark)`

**Usage**:
- Sidebar background
- Text colors
- Borders
- Shadows
- Header backgrounds

**Preview**:
```
████████████  #0F172A
```

---

### CNIT Light - Almost White
**Hex**: `#F8FAFC`
**RGB**: `rgb(248, 250, 252)`
**CSS Variable**: `var(--cnit-light)`

**Usage**:
- Page backgrounds
- Card backgrounds
- Light sections
- Input backgrounds

**Preview**:
```
████████████  #F8FAFC
```

---

## 🌈 Gradient

### CNIT Gradient
**CSS**: `linear-gradient(135deg, #0EA5E9 0%, #8B5CF6 100%)`
**CSS Variable**: `var(--cnit-gradient)`

**Usage**:
- Primary buttons
- Hero sections
- Special highlights
- Premium features

**Preview**:
```
████████████  Gradient from Sky Blue to Purple
```

---

## 🎭 Supporting Colors

### Gray Scale
```
#1F272E  ████  Gray 900 - Darkest text
#505A62  ████  Gray 700 - Secondary text
#98A1A9  ████  Gray 500 - Muted text
#C0C6CC  ████  Gray 400 - Borders
#DCE0E3  ████  Gray 300 - Light borders
#F4F5F6  ████  Gray 100 - Subtle backgrounds
```

### Semantic Colors
```
#10B981  ████  Success - Green
#F59E0B  ████  Warning - Orange
#EF4444  ████  Danger - Red
#3B82F6  ████  Info - Blue
```

---

## 📊 Color Usage Matrix

| Element | Primary | Secondary | Accent | Dark | Light |
|---------|---------|-----------|--------|------|-------|
| Buttons | ✅ | ✅ | ⚪ | ⚪ | ⚪ |
| Links | ✅ | ⚪ | ⚪ | ⚪ | ⚪ |
| Sidebar | ⚪ | ⚪ | ⚪ | ✅ | ⚪ |
| Content BG | ⚪ | ⚪ | ⚪ | ⚪ | ✅ |
| Success | ⚪ | ⚪ | ✅ | ⚪ | ⚪ |
| Hover | ✅ | ✅ | ⚪ | ⚪ | ⚪ |
| Active | ✅ | ⚪ | ⚪ | ⚪ | ⚪ |

---

## 🎯 Color Combinations

### High Contrast (WCAG AAA)
✅ **Dark on Light**:
- `#0F172A` on `#F8FAFC` - Contrast ratio: 16.5:1

✅ **Primary on White**:
- `#0EA5E9` on `#FFFFFF` - Contrast ratio: 3.2:1 (Large text only)

✅ **Primary on Dark**:
- `#0EA5E9` on `#0F172A` - Contrast ratio: 5.2:1

### Recommended Pairs
```
Primary + Light     #0EA5E9 + #F8FAFC
Secondary + Light   #8B5CF6 + #F8FAFC
Accent + Dark       #10B981 + #0F172A
Dark + Light        #0F172A + #F8FAFC
```

---

## 🖌️ Color Tints & Shades

### Primary Variations (Sky Blue)
```
Lighter:  #67C3F3  (Hover backgrounds)
Light:    #38B6F0  (Hover states)
Base:     #0EA5E9  (Primary)
Dark:     #0B82B8  (Pressed states)
Darker:   #086088  (Dark mode primary)
```

### Secondary Variations (Purple)
```
Lighter:  #B99DF9  (Hover backgrounds)
Light:    #A17EF7  (Hover states)
Base:     #8B5CF6  (Secondary)
Dark:     #6F4AC5  (Pressed states)
Darker:   #533894  (Dark mode secondary)
```

---

## 💡 Usage Guidelines

### DO ✅
- Use Primary (Sky Blue) for main actions
- Use Accent (Green) for success states
- Use Secondary (Purple) sparingly for special features
- Maintain color consistency across pages
- Use gradients for premium features

### DON'T ❌
- Don't use too many colors on one page
- Don't use Primary on Primary (low contrast)
- Don't override brand colors without reason
- Don't use colors without semantic meaning
- Don't ignore accessibility guidelines

---

## 🔧 Implementation Examples

### CSS
```css
/* Primary Button */
.btn-primary {
    background: var(--cnit-gradient);
    color: white;
}

/* Link */
a {
    color: var(--cnit-primary);
}

/* Success Message */
.alert-success {
    background: var(--cnit-accent);
    color: white;
}
```

### HTML with Inline Styles
```html
<!-- Primary Button -->
<button style="background: #0EA5E9; color: white;">
    Click Me
</button>

<!-- Success Badge -->
<span style="background: #10B981; color: white; padding: 4px 8px;">
    Success
</span>
```

### JavaScript/jQuery
```javascript
// Apply primary color dynamically
$('.element').css('color', 'var(--cnit-primary)');

// Apply gradient
$('.banner').css('background', 'var(--cnit-gradient)');
```

---

## 🌓 Dark Mode Alternatives

If implementing dark mode in the future:

```
Primary:    #38B6F0  (Lighter for dark backgrounds)
Secondary:  #A17EF7  (Lighter for dark backgrounds)
Accent:     #34D399  (Lighter for dark backgrounds)
Background: #0F172A  (Dark slate)
Surface:    #1E293B  (Lighter slate for cards)
Text:       #F8FAFC  (Almost white)
```

---

## 📱 Platform Specific

### iOS
```swift
// UIColor
let primary = UIColor(hex: "0EA5E9")
let secondary = UIColor(hex: "8B5CF6")
let accent = UIColor(hex: "10B981")
```

### Android
```xml
<!-- colors.xml -->
<color name="cnit_primary">#0EA5E9</color>
<color name="cnit_secondary">#8B5CF6</color>
<color name="cnit_accent">#10B981</color>
```

### React Native
```javascript
export const colors = {
  primary: '#0EA5E9',
  secondary: '#8B5CF6',
  accent: '#10B981',
  dark: '#0F172A',
  light: '#F8FAFC'
};
```

---

## 🎨 Design Tool Setup

### Figma
```
Create color styles:
- CNIT/Primary/Base → #0EA5E9
- CNIT/Secondary/Base → #8B5CF6
- CNIT/Accent/Base → #10B981
- CNIT/Dark → #0F172A
- CNIT/Light → #F8FAFC
```

### Adobe XD
```
Add to Assets panel:
- Primary: #0EA5E9
- Secondary: #8B5CF6
- Accent: #10B981
```

### Sketch
```
Create color variables:
- cnit-primary = #0EA5E9
- cnit-secondary = #8B5CF6
- cnit-accent = #10B981
```

---

## 📊 Accessibility Scores

### WCAG Compliance
```
Primary on White:     AA (Large text) ⚠️
Primary on Dark:      AAA ✅
Accent on White:      AA ✅
Accent on Dark:       AAA ✅
Dark on Light:        AAA ✅
```

### Recommendations
- For small text (< 18px), use Dark on Light
- For large text (> 18px), Primary/Accent on White is acceptable
- Always test with contrast checker tools

---

## 🔍 Color Picker Values

### For Photoshop/Illustrator
```
Primary:    C=94 M=29 Y=0 K=0
Secondary:  C=46 M=63 Y=0 K=0
Accent:     C=90 M=0 Y=30 K=0
```

### For Pantone
```
Primary:    Closest to Pantone 298 C
Secondary:  Closest to Pantone 2665 C
Accent:     Closest to Pantone 3395 C
```

---

## 📚 Resources

- [Coolors Palette](https://coolors.co/0ea5e9-8b5cf6-10b981-0f172a-f8fafc)
- [Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [Color Blind Simulator](https://www.color-blindness.com/coblis-color-blindness-simulator/)

---

**Last Updated**: 2025-12-10
**Version**: 1.0.0
**Company**: Cloud Native IT Solutions
