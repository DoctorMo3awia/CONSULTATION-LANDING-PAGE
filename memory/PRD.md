# Product Requirements Document - دكتور معاوية Health Audit Funnel

## Original Problem Statement
Build a full Arabic funnel for a doctor-led premium online consultation targeting busy high-value men (28-45) in UAE/Gulf. The service is an Executive Health & Performance Audit priced at $119 with manual payment via PayPal and post-payment Calendly booking.

## Core Requirements

### Target Audience
- Men 28-45 in UAE/GCC
- Entrepreneurs, executives, high-responsibility jobs
- Pain points: low energy, brain fog, stress, poor sleep, weight gain, health anxiety

### Offer Deliverables
1. 45-minute Google Meet consultation (Arabic) with Dr. Moawia
2. Blood test review and interpretation
3. Personalized 30-day medical-grade plan (sleep, caffeine, nutrition, exercise, travel, focus)
4. PDF summary within 24 hours
5. 7 days WhatsApp support (two daily reply windows)

### Price & Payment Flow
- $119 USD
- Limited slots: 6/week
- Payment: PayPal link (https://www.paypal.com/ncp/payment/2BKK55L2RNQHY)
- Post-payment: Coach manually emails Calendly link + evaluation form

## Architecture & Tech Stack

### Frontend
- React 19 with React Router (CRA)
- Shadcn UI components
- Custom CSS design system (App.css)
- RTL Arabic support
- Responsive design

### Pages
1. **Landing Page** (`/`) - Hero, target audience, testimonials, FAQ, CTA
2. **Offer Details** (`/offer`) - Service breakdown, doctor credentials, deliverables, pricing
3. **Booking Page** (`/booking`) - Payment instructions, PayPal button, benefits
4. **Ramadan Special** (`/ramadan`) - Seasonal offer with 8 common mistakes

### Design System (Elegant Executive Blue)
**Colors:**
- Hero gradient: #0f172a → #1e3a8a → #2563eb
- Header/Footer: Navy (#0c1a3a / rgba(15,23,42,0.95))
- Page background: #f8fafc
- Cards: #ffffff with #e2e8f0 borders
- Primary blue: #1e40af
- Text: #0f172a, #334155, #64748b

**Buttons:**
- Primary: Blue gradient, squared corners (0.5rem)
- Secondary: White with blue border
- Light: White (for dark backgrounds)
- Outline-light: Transparent with white border

## What's Been Implemented

### Completed (Feb 2025)
1. 4-page Arabic funnel with full RTL support
2. Dr. Moawia branding and professional photo
3. Real testimonials (عبدالرحمن, ماجد, عمر)
4. PayPal payment integration (external link)
5. WhatsApp integration (wa.me/971555519451)
6. Ramadan special offer page
7. **Elegant executive blue color scheme** - applied across all pages
8. Dark navy header and footer
9. Blue gradient hero sections
10. Section dividers for visual hierarchy
11. data-testid attributes on all interactive elements
12. Mobile responsive design (tested at 375x812)

### Testing Status
- Frontend testing: 100% pass (iteration_1.json)
- All 4 pages verified
- Navigation flows verified
- External links verified
- Mobile responsiveness verified

## Prioritized Backlog

### P1 - High Priority
- [ ] SEO optimization (meta tags, Open Graph)
- [ ] Privacy policy page
- [ ] Terms of service page

### P2 - Nice to Have
- [ ] Analytics integration (Google Analytics)
- [ ] A/B testing for headlines
- [ ] Dashboard for booking management
- [ ] Testimonial video embeds
- [ ] Before/after photo gallery

## File Structure
```
/app/frontend/src/
├── pages/
│   ├── Landing.jsx
│   ├── Offer.jsx
│   ├── Booking.jsx
│   └── Ramadan.jsx
├── components/ui/ (Shadcn components)
├── App.js (Router)
├── App.css (Executive Blue design system)
└── index.css (Tailwind base)
```

## Key External Links
- PayPal: https://www.paypal.com/ncp/payment/2BKK55L2RNQHY
- WhatsApp: https://wa.me/971555519451
- Calendly: https://calendly.com/drmoawia/consultation

---
**Last Updated:** February 10, 2026
**Status:** Color scheme redesign complete. Frontend MVP polished.
