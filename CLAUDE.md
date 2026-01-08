# Guac & Roll - Website Rebuild Documentation

## Project Overview

**Guac & Roll** is a vibrant Mexican food truck website featuring an online ordering system. This rebuild enhances the original website with modern code, responsive design, and properly organized assets.

### Goals
- Fix all broken asset paths from original code
- Create a clean, maintainable codebase
- Enhance visual design while maintaining brand identity
- Ensure responsive design across all devices
- Implement smooth animations and micro-interactions

---

## File Structure

```
guac&roll_claude/
├── index.html              # Main website file
├── CLAUDE.md               # This documentation
├── README.md               # Quick start guide
├── css/
│   └── styles.css          # Main stylesheet
├── js/
│   └── main.js             # JavaScript functionality
└── assets/
    ├── video/
    │   └── hero-background.mp4
    └── images/
        ├── guac_and_roll_logo_only.png
        ├── hero/
        │   ├── mexican-flags.png
        │   ├── flavor-tour-button.png
        │   ├── Chicken Tacos.png
        │   ├── Fish Tacos.png
        │   ├── Carne Asada Burrito.png
        │   ├── Flautas.png
        │   └── cropped image.png
        ├── nav/
        │   ├── Tacos.png
        │   ├── Burritos.png
        │   ├── Bowl.png
        │   ├── Guac and Chips.png
        │   └── Horchata.png
        ├── contact/
        │   └── food-truck-capitol.png
        └── menu/
            ├── tacos/
            │   ├── Cancun Crunch Taco.png
            │   ├── Acapulco Heat.png
            │   ├── Taco Santana.png
            │   ├── Mana Mango Taco.png
            │   ├── Tulum Verde-af80-4261-8243-5f450a9d14ab_3.png
            │   ├── CDMX Taco.png
            │   └── Baja Rocker Taco.png
            ├── burritos/
            │   ├── The Santana Solo.png
            │   ├── The Mana Mix Tour.png
            │   ├── The Acapulco Wave.png
            │   ├── The Guadalajara Groove.png
            │   └── Viva Veggie Tour.png
            ├── bowls/
            │   ├── The Riviera Maya Bowl.png
            │   ├── Oxacan Ember Bowl.png
            │   └── Rock & Verde Bowl.png
            ├── sides/
            │   ├── Guac & Roll Chips.png
            │   ├── Fiesta Fries.png
            │   ├── Cabo Elote Cup.png
            │   └── Rockstar Salsa Trio.png
            └── drinks/
                ├── Jalisco Jam Horchata.png
                ├── Lime & Roll Agua Fresca.png
                ├── Mango Mana Refresher.png
                └── Cafe Tacvba Cold Brew.png
```

---

## Asset Mapping

### Original Broken Paths → Fixed Local Paths

| Original Path | Fixed Path |
|--------------|------------|
| `https://cdn.prod.website-files.com/.../logo.png` | `assets/images/guac_and_roll_logo_only.png` |
| `Mex luch truck.mp4` | `assets/video/hero-background.mp4` |
| `mx flags.png` | `assets/images/hero/mexican-flags.png` |
| `mex button.png` | `assets/images/hero/flavor-tour-button.png` |
| `Untitled-20251217-140842-8470.png` | `assets/images/contact/food-truck-capitol.png` |

### Menu Item Images

#### Tacos
| Item | Image Path |
|------|------------|
| Cancun Crunch Taco | `assets/images/menu/tacos/Cancun Crunch Taco.png` |
| Acapulco Heat | `assets/images/menu/tacos/Acapulco Heat.png` |
| Taco Santana | `assets/images/menu/tacos/Taco Santana.png` |
| Mana Mango Taco | `assets/images/menu/tacos/Mana Mango Taco.png` |
| Tulum Verde | `assets/images/menu/tacos/Tulum Verde-af80-4261-8243-5f450a9d14ab_3.png` |
| CDMX Street Classic | `assets/images/menu/tacos/CDMX Taco.png` |
| Baja Rocker | `assets/images/menu/tacos/Baja Rocker Taco.png` |

#### Burritos
| Item | Image Path |
|------|------------|
| The Santana Solo | `assets/images/menu/burritos/The Santana Solo.png` |
| The Mana Mix Tour | `assets/images/menu/burritos/The Mana Mix Tour.png` |
| The Acapulco Wave | `assets/images/menu/burritos/The Acapulco Wave.png` |
| The Guadalajara Groove | `assets/images/menu/burritos/The Guadalajara Groove.png` |
| Viva Veggie Tour | `assets/images/menu/burritos/Viva Veggie Tour.png` |

#### Bowls
| Item | Image Path |
|------|------------|
| The Riviera Maya Bowl | `assets/images/menu/bowls/The Riviera Maya Bowl.png` |
| Oaxacan Ember Bowl | `assets/images/menu/bowls/Oxacan Ember Bowl.png` |
| Rock & Verde Bowl | `assets/images/menu/bowls/Rock & Verde Bowl.png` |

#### Sides
| Item | Image Path |
|------|------------|
| Guac & Roll Chips | `assets/images/menu/sides/Guac & Roll Chips.png` |
| Fiesta Fries | `assets/images/menu/sides/Fiesta Fries.png` |
| Cabo Elote Cup | `assets/images/menu/sides/Cabo Elote Cup.png` |
| Rockstar Salsa Trio | `assets/images/menu/sides/Rockstar Salsa Trio.png` |

#### Drinks
| Item | Image Path |
|------|------------|
| Jalisco Jam Horchata | `assets/images/menu/drinks/Jalisco Jam Horchata.png` |
| Lime & Roll Agua Fresca | `assets/images/menu/drinks/Lime & Roll Agua Fresca.png` |
| Mango Mana Refresher | `assets/images/menu/drinks/Mango Mana Refresher.png` |
| Cafe Tacvba Cold Brew | `assets/images/menu/drinks/Cafe Tacvba Cold Brew.png` |

---

## Design Guidelines

### Color Palette

| Color Name | Hex Code | Usage |
|------------|----------|-------|
| Deep Black | `#020617` | Background, cards |
| Dark Navy | `#0f172a` | Secondary backgrounds |
| Forest Green | `#14532d` | Accents, headers |
| Lime Green | `#22c55e` | Primary buttons, CTAs |
| Cyan | `#22d3ee` | Category labels |
| Rose/Pink | `#fb7185` | Category titles, remove buttons |
| Lime Yellow | `#bef264` | Prices |
| Orange | `#fb923c` | Spicy badge |
| Green | `#4ade80` | Vegetarian badge |
| Yellow | `#facc15` | Item tags |

### Typography

- **Primary Font**: `system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif`
- **Headings**: Bold (700-800 weight)
- **Body**: Regular (400 weight)
- **Sizes**: Responsive using `clamp()` for fluid scaling

### Border Radius Scale

| Size | Value | Usage |
|------|-------|-------|
| Small | `0.7rem` | Images, small buttons |
| Medium | `1rem` | Cards on mobile |
| Large | `1.2rem` | Category cards |
| Full | `999px` | Buttons, badges |

### Shadows

```css
/* Card shadow */
box-shadow: 0 18px 40px rgba(15, 23, 42, 0.9);

/* Modal shadow */
box-shadow: 0 25px 70px rgba(15, 23, 42, 0.95);
```

---

## Component Architecture

### 1. Navigation Bar
- Fixed position at top
- Logo (center on mobile)
- Links: Home, Menu, Contact us
- Hamburger menu on mobile

### 2. Hero Section
- Full-screen video background
- Overlay with fade-in animation (3s delay)
- Blur effect (5s delay)
- "Start the Flavor Tour" animated button
- Cards carousel on tablet/mobile

### 3. Pre-Menu Section
- "Mexican Flavor on Tour" heading
- 5 food card grid with wave animation
- Floating animation after entrance

### 4. Menu Sections
- Categories: Tacos, Burritos, Bowls, Sides, Drinks
- Two-column grid on desktop
- Single column on tablet/mobile
- Each item has: image, name, tags, description, price, quantity controls

### 5. Shopping Cart
- Sliding drawer from right
- Item management (add, remove, quantity)
- Subtotal, tax (8.75%), tip selection, total
- Checkout button

### 6. Contact Section
- Hours, location, phone, email
- Food truck image
- Google Maps link
- Call/Email buttons

### 7. Modals
- Nutrition details modal
- Checkout/Order summary modal
- Category picker modal (mobile)

---

## JavaScript Features

### Cart System
- LocalStorage persistence
- Add/remove items
- Quantity adjustment
- Tax calculation (8.75%)
- Tip selection (0%, 10%, 15%, 20%, custom)

### Animations
- Hero CTA pop-in (3s delay)
- Card wave entrance animation
- Floating cards after load
- Button micro-interactions
- Smooth scroll navigation

### Modals
- Nutrition information display
- Checkout confirmation
- Menu category picker (mobile)

---

## Responsive Breakpoints

| Breakpoint | Device | Notes |
|------------|--------|-------|
| > 1200px | Desktop | Two-column menu, full cards grid |
| 991px - 1200px | Tablet Landscape | Single column menu, carousel |
| 768px - 991px | Tablet Portrait | Adjusted spacing |
| < 768px | Mobile | Full-width cart, stacked layout |
| < 478px | Small Mobile | Compact menu items |
| Landscape + max-height: 500px | Mobile Landscape | Special handling |

---

## Build & Run Instructions

### Development
```bash
# Navigate to project directory
cd guac&roll_claude

# Open in browser (macOS)
open index.html

# Or use a local server
python3 -m http.server 8000
# Then visit http://localhost:8000
```

### Production Deployment
1. Optimize images (compress PNGs)
2. Minify CSS/JS files
3. Upload to hosting provider
4. Update any absolute URLs if needed

---

## Enhancement Notes

### Improvements Made
1. **Organized Asset Structure**: All assets properly categorized
2. **Local Asset Paths**: No dependency on CDN URLs
3. **Clean Code**: Separated CSS and JS from HTML
4. **Responsive Design**: Works on all devices
5. **Performance**: Optimized animations with `will-change`
6. **Accessibility**: Proper button types, focus states

### Future Enhancements (Suggestions)
- Image lazy loading
- Service worker for offline support
- Payment gateway integration
- Analytics tracking
- SEO meta tags optimization

---

## Contact Information (Demo)

- **Hours**: Thu-Fri: 6:00 PM - 11:00 PM, Sat: 4:00 PM - 11:00 PM
- **Location**: 117 J St, Sacramento, CA 95814
- **Phone**: 888-888-8888
- **Email**: support@guacandroll.com

---

*Built with Claude Code - January 2026*
