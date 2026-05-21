# GiveBack IITJ

A **React-based donation portal** for the Indian Institute of Technology Jodhpur (IITJ). Built to facilitate alumni and supporter contributions with dedicated flows for donors in India, the USA, and other countries.

## What It Does

GiveBack IITJ provides a clean, modern web interface for making donations to IIT Jodhpur. It supports multiple donation pathways, showcases impact statistics, features testimonials, and includes animated UI components for an engaging donor experience.

## Features

| Feature | Description |
|---------|-------------|
| 🎠 **Impact Carousel** | Auto-rotating carousel highlighting donation impact stories |
| 📊 **Animated Statistics** | Animated counters showing total donations, donors, projects funded |
| 💳 **Multi-region Donation** | Separate flows for India, USA, and Rest of World |
| 🏦 **Payment Methods** | Bank transfer, cheque/draft, and online options |
| 🗣️ **Testimonials** | Alumni and donor voices with FAQ-style accordion |
| 🃏 **Interactive Cards** | Hover-reveal cards with gradient animations |
| 🎨 **Tailwind CSS** | Responsive, utility-first styling |

## Tech Stack

- **React 18** — UI framework
- **React Router DOM** — Client-side routing
- **Tailwind CSS** — Styling
- **Framer Motion** — Scroll animations and entrance effects
- **Lucide React** — Icons

## Project Structure

```
giveback/
├── public/
│   ├── assets/
│   │   ├── card.jpg          # Card background image
│   │   ├── globe.jpg         # Rest of world flag
│   │   ├── india.png         # India flag
│   │   └── usan.png          # USA flag
│   └── index.html
├── src/
│   ├── App.js                # Router configuration
│   ├── components/
│   │   ├── Navbar.jsx
│   │   ├── Carousel.jsx      # Impact stories carousel
│   │   ├── WhyGive.jsx       # Reasons to donate
│   │   ├── StatsSection.jsx  # Animated donation counters
│   │   ├── Card.jsx          # Interactive hover card
│   │   ├── Donate.jsx        # Donation options (India/USA/Other)
│   │   ├── IndiaDonate.jsx   # India-specific donation flow
│   │   ├── OtherCountriesDonate.jsx
│   │   ├── BankTransferForm.jsx
│   │   ├── ChequeDraftForm.jsx
│   │   ├── Testimonials.jsx  # Donor FAQ/Testimonials
│   │   ├── Footer.jsx
│   │   └── Card.jsx
│   └── data/
│       ├── carousel.js       # Carousel content data
│       ├── stats.js          # Statistics numbers
│       └── navItem.js        # Navigation items
└── package.json
```

## Pages

| Route | Description |
|-------|-------------|
| `/` | Landing page with carousel, stats, cards, testimonials |
| `/donate` | Donation region selection (India / USA / Other) |
| `/donate/in/Annual-Gift-Programme` | India donation form |
| `/donate/oc/Annual-Gift-Programme` | Other countries donation form |

## Getting Started

```bash
cd giveback
npm install
npm start
# → http://localhost:3000
```

## Build

```bash
npm run build
# Deploy build/ folder to static hosting (Netlify, Vercel, GitHub Pages)
```

## Design Highlights

- **Red accent color** (`#910707`) — tied to IIT Jodhpur branding
- **Smooth scroll animations** — Framer Motion `inView` triggers for counting stats
- **Card hover states** — Gradient overlays and shadow transitions
- **Responsive grid** — Cards and donation options stack on mobile
