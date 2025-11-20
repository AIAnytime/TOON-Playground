# 🎨 TOON Playground - Visual Reference Guide

## 🖼️ UI Layout Overview

```
┌─────────────────────────────────────────────────────────────────┐
│  🎯 HEADER (Gradient: Indigo → Purple)                          │
│  ┌──────────────────────────────────────┐  ┌──────────────┐    │
│  │ TOON Playground                      │  │ 40% Savings  │    │
│  │ Token-Oriented Object Notation       │  └──────────────┘    │
│  └──────────────────────────────────────┘                       │
└─────────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  📚 INFO BANNER (Light gradient)                                │
│  What is TOON? [Description]                                    │
│  ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐                  │
│  │ 📊     │ │ 🔁     │ │ ⚡      │ │ 🎯     │                  │
│  │Tabular │ │JSON    │ │40%     │ │LLM     │                  │
│  │Arrays  │ │Compat  │ │Fewer   │ │Optimiz │                  │
│  └────────┘ └────────┘ └────────┘ └────────┘                  │
└─────────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  🎮 EXAMPLES                                                     │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐          │
│  │ Simple   │ │ Product  │ │Analytics │ │ Nested   │          │
│  │ Users    │ │ Catalog  │ │ Data     │ │Structure │          │
│  │ [CLICK]  │ │ [CLICK]  │ │ [CLICK]  │ │ [CLICK]  │          │
│  └──────────┘ └──────────┘ └──────────┘ └──────────┘          │
└─────────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  ✏️ INPUT JSON DATA                                             │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ JSON Input                                      [Format]  │ │
│  ├───────────────────────────────────────────────────────────┤ │
│  │ {                                                         │ │
│  │   "users": [                                              │ │
│  │     {"id": 1, "name": "Alice"}                            │ │
│  │   ]                                                       │ │
│  │ }                                                         │ │
│  ├───────────────────────────────────────────────────────────┤ │
│  │ [🔄 Convert to All Formats]  [Clear]                     │ │
│  └───────────────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  📊 FORMAT COMPARISON                                            │
│  ┌──────────┐ ┌──────────┐ ┌──────────────┐                   │
│  │ JSON     │ │ YAML     │ │ TOON ⭐      │                   │
│  │ 100 toks │ │ 80 toks  │ │ 40 toks      │                   │
│  │ ████████ │ │ ██████   │ │ ████ ✨      │                   │
│  └──────────┘ └──────────┘ └──────────────┘                   │
│  ┌──────────┐ ┌──────────┐ ┌──────────────┐                   │
│  │ JSON     │ │ YAML     │ │ TOON         │                   │
│  │ [Copy]   │ │ [Copy]   │ │ [Copy]       │                   │
│  │ {...}    │ │ users:   │ │ users[2]{..} │                   │
│  │          │ │   - id:1 │ │   1,Alice    │                   │
│  └──────────┘ └──────────┘ └──────────────┘                   │
└─────────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  🤖 TEST WITH OPENAI                                            │
│  ┌──────────────────────┐  ┌──────────────────────────────┐   │
│  │ Your Question:       │  │ Response:                    │   │
│  │ [Text input]         │  │ [LLM Output]                 │   │
│  │                      │  │                              │   │
│  │ Format:              │  │ 📊 Tokens: 50 input          │   │
│  │ ○ JSON ○ YAML ● TOON │  │          30 output           │   │
│  │                      │  │                              │   │
│  │ [🤖 Send to OpenAI]  │  │                              │   │
│  └──────────────────────┘  └──────────────────────────────┘   │
└─────────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  📖 HOW IT WORKS                                                │
│  ┌─────────┐  ┌─────────┐  ┌─────────┐                        │
│  │ ①       │  │ ②       │  │ ③       │                        │
│  │ Declare │  │ Tabular │  │ Minimal │                        │
│  │ Once    │  │ Format  │  │ Syntax  │                        │
│  └─────────┘  └─────────┘  └─────────┘                        │
└─────────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  📄 FOOTER                                                       │
│  About TOON | Resources | Made with FastAPI                    │
└─────────────────────────────────────────────────────────────────┘
```

## 🎨 Color Palette

```
┌─────────────────┐
│ PRIMARY         │
│ #6366f1 ████    │  Indigo (buttons, accents)
│ #4f46e5 ████    │  Dark Indigo (hover)
│ #818cf8 ████    │  Light Indigo (highlights)
└─────────────────┘

┌─────────────────┐
│ SUCCESS         │
│ #10b981 ████    │  Green (TOON savings)
└─────────────────┘

┌─────────────────┐
│ BACKGROUNDS     │
│ #ffffff ████    │  Pure white
│ #f9fafb ████    │  Light gray
│ #f3f4f6 ████    │  Lighter gray
│ #e5e7eb ████    │  Border gray
└─────────────────┘

┌─────────────────┐
│ TEXT            │
│ #111827 ████    │  Primary text
│ #6b7280 ████    │  Secondary text
│ #9ca3af ████    │  Tertiary text
└─────────────────┘
```

## 📝 Typography Hierarchy

```
┌─────────────────────────────────────────┐
│ POPPINS (Headers)                       │
├─────────────────────────────────────────┤
│ H1: 2.5rem (40px)  • Weight 700        │
│ H2: 1.875rem (30px) • Weight 600       │
│ H3: 1.25rem (20px)  • Weight 600       │
└─────────────────────────────────────────┘

┌─────────────────────────────────────────┐
│ INTER (Body Text)                       │
├─────────────────────────────────────────┤
│ Body: 1rem (16px)    • Weight 400      │
│ Small: 0.875rem (14px) • Weight 400    │
│ Bold: varies         • Weight 600       │
└─────────────────────────────────────────┘

┌─────────────────────────────────────────┐
│ MONACO (Code)                           │
├─────────────────────────────────────────┤
│ Code: 0.875rem (14px) • Monospace      │
└─────────────────────────────────────────┘
```

## 📐 Component Specs

### Example Card
```
┌──────────────────────────┐
│ 📊 Simple Users          │  ← Poppins 1.125rem
│                          │
│ Basic user list -        │  ← Inter 0.875rem
│ perfect for TOON's       │     (secondary color)
│ tabular format           │
│                          │
│ [HOVER: Border indigo,   │
│  Shadow, Transform Y-2px]│
└──────────────────────────┘
  280px min-width
  Padding: 1.5rem
  Border: 2px solid
  Radius: 0.75rem
```

### Token Card
```
┌──────────────────────────┐
│ JSON      [Original]     │  ← Header
│                          │
│ 100 tokens              │  ← Poppins 2rem
│ ████████████████        │  ← Progress bar
│                          │
└──────────────────────────┘
  Background: Light gray
  Padding: 1.5rem
  Border-radius: 0.75rem
```

### Button Styles
```
┌─────────────────────┐
│ 🔄 Convert Formats  │  ← Primary button
└─────────────────────┘
  Background: #6366f1
  Color: white
  Padding: 1rem 1.5rem
  Font: Poppins 600
  
┌─────────────────────┐
│ Format              │  ← Secondary button
└─────────────────────┘
  Background: white
  Border: 1px #e5e7eb
  Color: #111827
```

## 🔄 User Flow Diagram

```
START
  ↓
┌─────────────────────┐
│ User opens page     │
└─────────────────────┘
  ↓
┌─────────────────────┐
│ Sees 4 examples     │
│ + input area        │
└─────────────────────┘
  ↓
  ├─→ OPTION A: Click example
  │   ↓
  │   ┌──────────────────────┐
  │   │ JSON auto-loads      │
  │   │ Conversion happens   │
  │   └──────────────────────┘
  │
  ├─→ OPTION B: Paste own JSON
  │   ↓
  │   ┌──────────────────────┐
  │   │ Click "Convert"      │
  │   └──────────────────────┘
  │
  ↓
┌─────────────────────┐
│ See comparison:     │
│ • Token counts      │
│ • Progress bars     │
│ • Format outputs    │
└─────────────────────┘
  ↓
  ├─→ Copy output
  │   ↓
  │   ┌──────────────────────┐
  │   │ Use in own project   │
  │   └──────────────────────┘
  │
  ├─→ Test with OpenAI
  │   ↓
  │   ┌──────────────────────┐
  │   │ Enter prompt         │
  │   │ Select format        │
  │   │ Send to API          │
  │   │ See response         │
  │   └──────────────────────┘
  │
  ↓
END (Understanding TOON!)
```

## 💫 Animation Details

### On Page Load
```
Header: Fade in + Slide down (0.5s)
Info Banner: Fade in (0.7s delay)
Examples: Stagger fade in (0.1s each)
Sections: Slide up on scroll
```

### On Convert Click
```
1. Button: Loading state (spinner)
2. Token bars: Animate width (0.6s ease)
3. Savings badges: Pop in (0.3s)
4. Code outputs: Fade in (0.4s)
```

### On Hover
```
Example cards: 
  - Border → indigo
  - Transform Y(-2px)
  - Shadow increase
  - Transition: 0.2s
  
Buttons:
  - Background darken
  - Shadow increase
  - Transition: 0.2s
```

### Toast Notifications
```
Enter: Slide from right (0.3s)
Stay: 3 seconds
Exit: Slide to right (0.3s)
```

## 📱 Responsive Breakpoints

```
Desktop (> 1024px):
  Container: 1400px max
  Grid: 3-4 columns
  Spacing: Full (2-3rem)

Tablet (768px - 1024px):
  Container: 100%
  Grid: 2 columns
  Spacing: Medium (1.5rem)

Mobile (< 768px):
  Container: 100%
  Grid: 1 column
  Spacing: Compact (1rem)
  Header: Reduced padding
  Font sizes: Slightly smaller
```

## 🎯 Interactive Elements

### Clickable
```
✓ Example cards (4)
✓ Convert button
✓ Format button
✓ Clear button
✓ Copy buttons (3)
✓ Send to OpenAI button
✓ Radio buttons (3)
```

### Input Fields
```
✓ JSON textarea (main input)
✓ Prompt textarea (LLM test)
✓ Format radio group
```

### Output/Display Only
```
✓ Token counts
✓ Progress bars
✓ Format outputs (3)
✓ LLM response
✓ Info sections
```

## 🎨 Visual Hierarchy

```
LEVEL 1 (Most Important)
  • Page title (TOON Playground)
  • Convert button
  • Token savings percentage

LEVEL 2 (Important)
  • Section headers
  • Example cards
  • Token comparison cards

LEVEL 3 (Supporting)
  • Descriptions
  • Feature badges
  • Code outputs

LEVEL 4 (Tertiary)
  • Footer
  • Small labels
  • Meta information
```

## 🌈 Success States

### Token Savings > 40%
```
Color: Success green (#10b981)
Badge: "🎉 40% savings vs JSON"
Bar: Green gradient
```

### Token Savings 20-40%
```
Color: Warning amber (#f59e0b)
Badge: "20% savings vs JSON"
Bar: Amber gradient
```

### Token Savings < 20%
```
Color: Primary indigo (#6366f1)
Badge: "Some savings vs JSON"
Bar: Indigo gradient
```

## 🎪 Special Effects

### Gradient Backgrounds
```css
Header: 
  linear-gradient(135deg, #6366f1 0%, #4f46e5 100%)

Info Banner:
  linear-gradient(135deg, #667eea15 0%, #764ba215 100%)

Success Card:
  linear-gradient(135deg, #10b98110 0%, #10b98105 100%)
```

### Shadows
```css
Cards: 
  box-shadow: 0 1px 3px rgba(0,0,0,0.1)

On Hover:
  box-shadow: 0 4px 6px rgba(0,0,0,0.1)

Header:
  box-shadow: 0 20px 25px rgba(0,0,0,0.1)
```

### Border Radius
```css
Small: 0.375rem (6px)
Default: 0.5rem (8px)
Large: 0.75rem (12px)
XL: 1rem (16px)
```

---

## 🎉 Visual Summary

Your TOON Playground features:

✨ **Modern gradient design** (indigo → purple)
🎨 **Beautiful typography** (Poppins + Inter)
📊 **Animated comparisons** (token bars, progress)
🎯 **Clear hierarchy** (visual importance levels)
💫 **Smooth interactions** (hover, click, scroll)
📱 **Responsive layout** (mobile, tablet, desktop)
🌈 **Consistent colors** (primary, success, text)
🎪 **Delightful effects** (shadows, gradients, animations)

**Status**: ✅ Production-ready visual design!
