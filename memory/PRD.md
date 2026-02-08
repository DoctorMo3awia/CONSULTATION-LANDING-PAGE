# Product Requirements Document - دكتور معاوية Health Audit Funnel

## Original Problem Statement
Build a full Arabic funnel for a doctor-led premium online consultation targeting busy high-value men (28-45) in UAE/Gulf. The service is an Executive Health & Performance Audit priced at $119 with manual payment via bank transfer.

## Core Requirements

### Target Audience
- Men 28-45 in UAE/GCC
- Entrepreneurs, executives, high-responsibility jobs
- Pain points: low energy, brain fog, stress, poor sleep, weight gain, health anxiety
- Desired outcomes: higher energy, better focus, improved physique, reduced health anxiety

### Offer Deliverables
1. 60-minute Google Meet consultation (Arabic) with Dr. Moawia
2. Blood test review and interpretation
3. Personalized 30-day medical-grade plan:
   - Sleep + caffeine strategy
   - Nutrition rules for restaurants/dinners
   - Minimum effective dose training plan
   - Travel plan + focus protocol
4. PDF summary within 24 hours
5. 7 days WhatsApp support (two daily reply windows)

### Price & Constraints
- $119 USD
- Limited slots: 6/week
- Payment: Bank transfer only (no payment gateway)
- Booking confirmed after proof of transfer

## Architecture & Tech Stack

### Frontend
- React 19 with React Router
- Shadcn UI components
- Tailwind CSS with warm-ai design system
- RTL Arabic support
- Responsive design (mobile-first)

### Pages Implemented
1. **Landing Page** (`/`) - Hero, testimonials, target audience, FAQ
2. **Offer Details** (`/offer`) - Full service breakdown, doctor credentials, deliverables
3. **Booking Page** (`/booking`) - Form preview, payment instructions, red-flag symptoms
4. **Ramadan Special** (`/ramadan`) - Seasonal offer with 8 common mistakes

### Design System (Warm-AI)
**Colors:**
- Background: #FFF9F2 (warm cream)
- Cards: #FFFFFF
- Text: #232323, #353535
- Accent colors: Purple, Blue, Orange, Pink, Green (pastel versions)
- Gradients: Warm peach/cream tones

**Typography:**
- SF Mono for buttons and UI elements
- Responsive clamp() sizing
- Arabic-optimized line heights

**Components:**
- Pill/capsule buttons (border-radius: 2rem)
- Glass-morphism effects for secondary elements
- Voice cards with hover animations
- Fixed header with backdrop blur

## What's Been Implemented (Dec 2025)

### ✅ Completed Features
1. 4-page Arabic funnel with full RTL support
2. Dr. Moawia branding and professional photo integrated
3. Real testimonials from existing clients (عبدالرحمن, ماجد, عمر)
4. Warm-ai design system fully implemented
5. Responsive navigation and routing
6. WhatsApp integration placeholders
7. Google Form booking flow
8. Ramadan special offer page with 8 mistakes breakdown
9. Complete WhatsApp automation scripts
10. Payment instructions and booking confirmation flow

### 📄 Documentation Created
1. `/app/whatsapp_scripts.md` - Complete WhatsApp messaging automation
2. `/app/memory/PRD.md` - This document

## Prioritized Backlog

### P0 - Critical (Before Launch)
- [ ] Replace WhatsApp number placeholder (971XXXXXXXXX) with real number
- [ ] Add actual Google Form URL in Booking page
- [ ] Add bank transfer details in WhatsApp scripts
- [ ] Test all page transitions and CTAs
- [ ] Mobile responsive testing

### P1 - High Priority
- [ ] Backend for form submissions tracking
- [ ] Email notifications after form submission
- [ ] Analytics integration (Google Analytics or Mixpanel)
- [ ] A/B testing setup for headlines
- [ ] SEO optimization (meta tags, Open Graph)

### P2 - Nice to Have
- [ ] Dashboard for booking management
- [ ] Automated WhatsApp Business API integration
- [ ] Calendar integration for slot management
- [ ] Testimonial video embeds
- [ ] Before/after photo gallery
- [ ] Arabic blog for SEO content

## Next Action Items

1. **Update Placeholders:**
   - WhatsApp number in all pages
   - Google Form URL
   - Bank account details

2. **Content Review:**
   - Review all Arabic copy with native speaker
   - Verify medical disclaimers
   - Confirm pricing and slot availability

3. **Testing:**
   - Test complete user journey from landing to booking
   - Mobile device testing (iOS/Android)
   - RTL layout verification
   - WhatsApp link functionality

4. **Launch Preparation:**
   - Set up domain and hosting
   - Configure email for notifications
   - Prepare launch social media posts
   - Create tracking links for ad campaigns

## Technical Notes

### File Structure
```
/app/frontend/src/
├── pages/
│   ├── Landing.jsx
│   ├── Offer.jsx
│   ├── Booking.jsx
│   └── Ramadan.jsx
├── components/ui/ (Shadcn components)
├── App.js (Router configuration)
├── App.css (Warm-ai design system)
└── index.css (Tailwind base)
```

### Environment Variables
- `REACT_APP_BACKEND_URL` - Backend API URL (currently unused, frontend-only)

### Key Design Decisions
1. **Frontend-only first approach:** Rapid deployment without backend complexity
2. **Manual payment flow:** Avoids payment gateway compliance issues in initial MVP
3. **External Google Form:** Leverages existing tools, reduces development time
4. **WhatsApp-based support:** Familiar channel for Gulf audience
5. **Warm-ai aesthetics:** Professional medical credibility with approachable warmth

## Success Metrics (Post-Launch)

### Conversion Funnel
- Landing page visit → Offer page: Target 40%
- Offer page → Booking form: Target 25%
- Form submission → Payment: Target 60%
- Overall conversion: 6% (6 bookings from 100 visitors)

### User Engagement
- Average time on site: >3 minutes
- Bounce rate: <50%
- Mobile vs Desktop: Track ratio
- WhatsApp inquiries vs direct bookings

### Revenue
- Target: 6 consultations/week = $714/week
- Monthly recurring: $3,000+
- Upsell opportunities: Follow-up packages, group programs

## Legal & Compliance

### Disclaimers Present
- "Health education and guidance, not medical diagnosis"
- Red-flag symptoms warning with urgent care instructions
- Clear scope of service (consultation, not treatment)
- Privacy notice for form data

### Required Updates
- Privacy policy page
- Terms of service
- Refund policy (48-hour cancellation)
- Data protection compliance (GDPR/UAE laws)

---

**Document Version:** 1.0  
**Last Updated:** February 8, 2025  
**Status:** Frontend MVP Complete, Ready for Content Review
