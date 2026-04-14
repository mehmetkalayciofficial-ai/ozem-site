# Claude Code Prompt — B2B Pharmaceutical Supply Website

Aşağıdaki promptu Claude Code'a yapıştırabilirsin. Gerekli yerleri kendi müşterinin bilgileriyle güncelle.

---

## PROMPT

```
Build a complete, production-grade, single-page website for a B2B pharmaceutical supply company. The site must feel premium, trustworthy, and institutional — like a company that supplies medications to clinics and healthcare facilities in underserved regions worldwide. This is NOT a consumer-facing pharmacy. It is a licensed pharmaceutical distributor serving healthcare institutions.

## Brand & Identity

- Company Name: [MÜŞTERİ FİRMA ADI]
- Tagline: "Reliable Pharmaceutical Supply for Healthcare Institutions"
- Logo: Use a clean SVG placeholder logo (pill/cross/molecule icon + company name in a refined typeface)
- Industry Tone: Clinical trust, institutional authority, global reach

## Design Direction

**Aesthetic: Medical-Institutional Luxury** — Think McKinsey meets Pfizer. Clean, spacious, confident. Not a trendy startup and not a generic pharmacy.

- **Color Palette**: Deep navy (#0A1628) as primary, white/off-white (#F8F9FA) backgrounds, accent in teal (#0D9488) or a medical blue-green. Subtle warm gray for secondary text.
- **Typography**: Use Google Fonts — a refined serif for headings (e.g., "DM Serif Display" or "Playfair Display") paired with a clean sans-serif for body (e.g., "Plus Jakarta Sans", "Outfit", or "General Sans"). NO Inter, Roboto, or Arial.
- **Layout**: Generous whitespace, asymmetric grid sections, full-width hero. Content should breathe.
- **Visual Details**: Subtle gradient overlays, fine border lines as section dividers, soft shadows, micro-animations on scroll (fade-up, stagger reveals). A frosted glass effect on the navbar on scroll.
- **Imagery**: Use CSS-generated abstract shapes, gradients, or geometric patterns as visual accents (no stock photos needed). Consider a world map visualization (SVG or CSS) showing supply regions.

## Page Structure (Single Page, Smooth Scroll)

### 1. Navigation Bar
- Fixed top, transparent → frosted glass on scroll
- Links: About, Products, Regions, Compliance, Contact
- CTA button: "Request a Quote" (scrolls to contact section)
- Placeholder logo on the left

### 2. Hero Section
- Large headline: "Trusted Pharmaceutical Supply for Global Healthcare"
- Subheadline: "We partner with licensed manufacturers to deliver essential medications to clinics and healthcare facilities in underserved markets."
- Two CTAs: "Explore Our Catalog" (ghost button) + "Get in Touch" (solid button)
- Abstract background: subtle animated gradient mesh or geometric pattern
- Key stats bar below hero: "X+ Countries Served | X+ Healthcare Partners | FDA/EMA Compliant Supply Chain"

### 3. About Section
- Company overview: Who we are, what we do
- Emphasis on: licensed operations, cold-chain logistics, regulatory compliance
- Layout: Text on one side, decorative SVG/illustration element on the other (molecule structure, supply chain diagram, or abstract medical graphic)
- Subtitle: "Bridging the Gap in Global Pharmaceutical Access"

### 4. Product Catalog Section
- Title: "Therapeutic Areas & Product Portfolio"
- Display as elegant card grid (NOT an e-commerce product listing)
- Categories (example cards):
  - Metabolic & Endocrine (GLP-1 receptor agonists, insulin analogs)
  - Cardiovascular
  - Oncology Support
  - Immunology
  - Rare & Specialty Medications
- Each card: Category icon (SVG), category name, brief description, "Inquire About Availability" link
- **Important**: No prices, no "buy now" buttons, no specific drug brand names on the main display. Keep it category-level. Individual product details available upon inquiry.
- Small note below: "Full product catalog available upon request for verified healthcare institutions."

### 5. Supply Regions Section
- Title: "Where We Operate"
- SVG world map with highlighted regions (Middle East, Africa, Central Asia, Southeast Asia, Latin America — pick regions that make sense)
- Or: Elegant grid of region cards with country flags/icons
- Brief text about logistics capabilities, cold-chain, last-mile delivery

### 6. Compliance & Credentials Section
- Title: "Regulatory Compliance & Quality Assurance"
- Grid or timeline of compliance points:
  - Licensed pharmaceutical distribution
  - GDP (Good Distribution Practice) compliant
  - Cold-chain certified logistics
  - Partnerships with WHO-prequalified / FDA-approved / EMA-approved manufacturers
  - Full traceability & batch documentation
- Trust badges / certification icons (placeholder SVGs)
- Note: "All documentation and licenses available upon request for institutional partners."

### 7. How It Works Section
- Title: "Partnership Process"
- 4-step horizontal process:
  1. "Initial Inquiry" — Contact us with your institution's needs
  2. "Verification" — We verify your healthcare institution credentials
  3. "Custom Quote" — Receive a tailored supply proposal
  4. "Reliable Delivery" — Scheduled, compliant pharmaceutical delivery
- Clean numbered steps with icons and connecting lines

### 8. Contact / Request a Quote Section
- Title: "Start a Supply Inquiry"
- Subtitle: "Available exclusively for licensed healthcare institutions, clinics, and hospital groups."
- Form fields:
  - Institution Name
  - Contact Person & Title
  - Country / Region
  - Email
  - Phone (optional)
  - Therapeutic Area of Interest (dropdown)
  - Message / Specific Requirements (textarea)
  - Checkbox: "I confirm this inquiry is on behalf of a licensed healthcare institution"
- The form doesn't need to actually submit — just show a success toast/modal on "submit"
- Alternative contact: Email address + WhatsApp business number (placeholders)

### 9. Footer
- Company name & tagline
- Quick links (same as nav)
- Legal links: Privacy Policy, Terms of Service, Compliance
- Disclaimer text: "This website and its services are intended solely for licensed healthcare professionals and institutions. We do not sell medications directly to individual consumers. All products are sourced from licensed, regulatory-approved manufacturers."
- Copyright line

## Technical Requirements

- Single HTML file with embedded CSS and JS (no framework needed, or React if you prefer)
- Fully responsive (mobile-first)
- Smooth scroll behavior
- Scroll-triggered fade-in animations (use IntersectionObserver, no heavy libraries)
- CSS variables for all colors, spacing, typography
- Semantic HTML5 elements
- Accessible: proper contrast ratios, ARIA labels, keyboard navigation
- Performance: no external images, all visuals via CSS/SVG
- Dark/light sections alternating for visual rhythm

## What to AVOID

- No e-commerce functionality (no cart, no checkout, no prices)
- No specific drug brand names prominently displayed
- No medical claims or efficacy statements
- No "buy now" or "order" language — use "inquire", "request", "partner"
- No stock photos of pills or medications
- No generic template aesthetics — this should feel custom-designed
- No purple gradient AI-slop aesthetic

## Quality Bar

This should look like it was designed by a top-tier agency. Every pixel matters. Typography should be beautiful. Spacing should be intentional. Animations should be smooth and tasteful. The overall impression should be: "This is a serious, well-funded, legitimate pharmaceutical supply operation."
```

---

## Kullanım Notları

1. `[MÜŞTERİ FİRMA ADI]` kısmını gerçek firma adıyla değiştir
2. İstatistikler (X+ Countries vs.) gerçek verilerle güncellenebilir
3. Bölgeler müşterinin gerçek operasyon bölgelerine göre ayarlanabilir
4. Terapötik alan kategorileri müşterinin ürün portföyüne göre düzenlenebilir
5. Site çıktıktan sonra müşterin lisans/sertifika bilgilerini ekleyebilirsin
