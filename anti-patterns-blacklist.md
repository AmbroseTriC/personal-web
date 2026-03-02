# AI UI Anti-Patterns Blacklist

When generating frontend UI code, **never** fall into these patterns. They are the telltale signs of generic, AI-generated design — instantly recognizable and devoid of personality.

---

## CRITICAL — Instant AI Detection

### 1. The Purple Gradient Plague
**Do not** use purple-to-blue or purple-to-pink gradients on white backgrounds. This is the single most recognizable AI aesthetic.
- Avoid: `linear-gradient(135deg, #667eea, #764ba2)`
- Avoid: `linear-gradient(to right, #6366f1, #a855f7, #ec4899)`
- Avoid: purple hero → white card grid → purple CTA footer

### 2. The Inter/System Font Default
**Do not** default to Inter, Roboto, system-ui, or Arial. These have zero typographic personality.
- Avoid: using the same font family for headlines and body with no pairing
- Avoid: identical weight/size ratios across every project
- Instead: choose a distinctive display font paired with a refined body font

### 3. Raw Tailwind Default Colors
**Do not** ship Tailwind's default palette without customization.
- Avoid: `bg-indigo-600 text-white rounded-lg shadow-md`
- Avoid: `bg-gray-50 border border-gray-200`
- Avoid: `text-gray-600` as universal body text color
- Avoid: mechanical spacing like p-4, p-6, p-8 with no rhythm

### 4. Unstyled shadcn/UI Components
**Do not** use raw shadcn/ui components with zero customization.
- Avoid: default zinc/slate color scheme unchanged
- Avoid: `border-border`, `bg-card`, `text-foreground` without overrides
- Avoid: output that looks like a component library documentation page

---

## HIGH — Very Common, Kills Originality

### 5. The 3-Column Card Grid
**Do not** default to three identical rounded cards in a row, each with icon + title + description.
- Avoid: `rounded-xl shadow-lg p-6` on identical cards
- Avoid: equal spacing with zero visual hierarchy
- Avoid: hover effect limited to `translateY(-4px)` + shadow increase

### 6. The Centered Hero Formula
**Do not** output the centered headline → subtitle → two buttons pattern every time.
- Avoid: `text-center max-w-3xl mx-auto` as automatic hero layout
- Avoid: "Get Started" (filled) + "Learn More" (outlined) button pair
- Avoid: gradient text on the headline with blurred circle decorations behind

### 7. Emoji & Lucide Icon Soup
**Do not** scatter random emojis or generic icons as section markers.
- Avoid: 🚀 Performance ⚡ Speed 🎨 Design 🔒 Security
- Avoid: Sparkles icon on everything
- Avoid: icons chosen for aesthetics rather than communication

### 8. The Fake SaaS Dashboard
**Do not** produce the sidebar + topbar + 4 stat cards + chart layout with fake data.
- Avoid: 4 stat cards in a row with green/red percentages
- Avoid: sidebar with "Dashboard, Analytics, Settings, Profile"
- Avoid: Recharts LineChart with smooth fake data that does nothing

### 9. The Space Grotesk Convergence
**Do not** converge on Space Grotesk, Poppins, Outfit, or Sora when trying to be "creative."
- These are the new Inter — slightly more interesting but equally overused in AI outputs
- Instead: do actual typographic research; pick fonts that match the specific project context

### 10. Mechanical Symmetry & Spacing
**Do not** make everything perfectly centered and symmetrical with uniform padding.
- Avoid: `mx-auto text-center` on everything
- Avoid: identical padding on all cards and sections
- Avoid: perfect 1:1:1 column ratios with zero visual tension
- Instead: use asymmetry, negative space, grid-breaking elements, and varied rhythm

---

## MEDIUM — Context-Dependent, Often Layered On

### 11. Gratuitous Glassmorphism
**Do not** apply `backdrop-blur` on everything over gradient backgrounds.
- Avoid: `bg-white/80 backdrop-blur-xl` as a universal card style
- Avoid: blurred circles behind glass cards with no consideration for readability
- Use frosted glass sparingly and only when it serves the design purpose

### 12. The Dark Mode Cliché
**Do not** default to `bg-gray-900` + white text + neon cyan/teal accents.
- Avoid: `bg-gray-900 text-white` as the automatic dark theme
- Avoid: cyan/teal glow effects and `border-cyan-400/50`
- Avoid: `from-gray-900 to-black` gradient backgrounds

### 13. Floating Blob Decorations
**Do not** place random blurred gradient circles behind content for "decoration."
- Avoid: `absolute -top-40 -right-40 w-80 h-80 bg-purple-300 rounded-full blur-3xl opacity-30`
- Avoid: multiple overlapping blurred circles with no compositional purpose
- Avoid: same blob placement and color across different projects

### 14. The Universal Hover Effect
**Do not** apply the same hover effect to every interactive element.
- Avoid: `hover:scale-105 transition-all duration-300` on everything
- Avoid: `hover:shadow-xl` (from shadow-md) as universal hover
- Avoid: `hover:-translate-y-1` on all cards
- Instead: vary hover behavior by context — some elements should dim, shift color, reveal content, or do nothing

### 15. The Fake Testimonial Block
**Do not** generate three testimonial cards with circular avatars, fake names, and generic praise.
- Avoid: circular avatar placeholder + "Jane Doe, CEO at TechCorp"
- Avoid: giant quotation marks as decoration
- Avoid: "This product changed my life!" with 5/5 stars, always exactly 3 testimonials

### 16. Gradient Text on Every Headline
**Do not** apply `bg-clip-text text-transparent bg-gradient-to-r` to every headline.
- Avoid: `from-purple-600 to-pink-600` or `from-blue-600 to-cyan-600` on all headings
- If everything is gradient, nothing stands out
- Reserve gradient text for one key element maximum, if used at all

---

## What To Do Instead

1. **Choose a bold, specific aesthetic direction** — brutalist, editorial, retro-futuristic, organic, luxury, industrial, playful — and commit fully
2. **Pick distinctive fonts** — research actual typefaces; pair a characterful display font with a clean body font
3. **Build a custom color palette** — derive colors from the project's context, not from Tailwind defaults
4. **Break the grid** — use asymmetry, overlap, diagonal flow, generous negative space, or controlled density
5. **Add atmosphere** — noise textures, geometric patterns, layered transparencies, dramatic shadows, custom cursors instead of generic blurred circles
6. **Vary interactions** — different hover states for different elements; scroll-triggered reveals; one well-orchestrated animation sequence instead of identical transitions everywhere
7. **Make it specific** — every design should feel like it was made for *this* project, not stamped from a template