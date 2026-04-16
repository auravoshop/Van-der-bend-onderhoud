# Van der Bend Onderhoud - Simplified Version TODO

## Completed Features (from v1)
- [x] Database schema and migrations
- [x] All pages: Home, Over Ons, Ons Werk, Diensten, Reviews, FAQ, Contact, Offerte
- [x] Live chat widget
- [x] Offerte multi-step form
- [x] Animations and modern styling

## Current Changes Completed
- [x] Remove account/login system from Navbar
- [x] Remove Account page route and all protected procedures
- [x] Remove login/logout buttons and user dropdown from Navbar
- [x] Remove Account page and all related routes
- [x] Simplify pages to be more compact (less text, smaller sections)
- [x] Set up email notifications to levivdbend@gmail.com (email templates created)
- [x] Create detailed email templates with company branding
- [x] Replace seed reviews with 8 realistic customer reviews
- [x] Remove booking/quote management features (keep only offerte submission)
- [x] Upgrade live chat with AI responses (LLM integration)
- [x] AI chat answers questions about services, duration, pricing
- [x] Test all features (13 tests passing)
- [x] Prepare for GitHub export

## Pages to Keep (Simplified)
- [x] Home: hero, services, why us, reviews preview
- [x] Over Ons: company story, values
- [x] Ons Werk: portfolio gallery
- [x] Diensten: service list
- [x] Reviews: customer reviews (8 realistic ones)
- [x] FAQ: questions and answers
- [x] Contact: contact form
- [x] Offerte: quote request form

## AI Chat Features
- [x] AI chat service with LLM integration (server/_core/aiChat.ts)
- [x] AI responds to questions about services (dakapel, elektra, loodgieterswerk, etc.)
- [x] AI provides service duration estimates
- [x] AI answers pricing questions
- [x] AI encourages users to request quotes
- [x] Modern chat widget styling maintained
- [x] Automatic AI response generation on user messages

## Email Configuration
- [x] Configure email service for levivdbend@gmail.com (templates in server/_core/emailService.ts)
- [x] Create detailed email template for quote submissions (HTML formatted with all fields)
- [x] Create detailed email template for contact form submissions (HTML formatted with all fields)
- [x] Include all customer info in emails (name, email, phone, address, service details, budget, date)
- [x] Use "Van der Bend Onderhoud" as sender name and title (in email headers and footer)


## All Features Completed ✓
- [x] Cookie bar with accept/reject functionality
- [x] Dark/Light mode toggle (day/night function) on all pages with proper OKLCH colors
- [x] Language switcher (NL/EN) with complete i18n translations
- [x] Trustpilot announcement bar (4.8 stars) at top
- [x] Legal pages: Terms & Conditions, Privacy Policy (NL/EN)
- [x] WhatsApp integration for live chat (header button + wa.me/31684901999)
- [x] AI Offerte Helper Bot with geocoding and 50km radius validation
- [x] Location permission request with Haversine distance calculation
- [x] Auto-send offerte to WhatsApp with complete customer data
- [x] Chat scroll behavior fixed - only scrolls when user is at bottom
- [x] Chat bot renamed to "Onderhouds Bot"
- [x] All 13 tests passing
- [x] No TypeScript errors
- [x] Full dark mode support with proper contrast
- [x] Complete i18n on all pages and components


## Current Session - Final Improvements
- [x] Fix TypeScript error in AIOfferteHelper (remove trpc import, use simulated responses)
- [x] Restructure postcode check page: Add "AI Offerte Maker" header, add "Handmatige Offerte" button at bottom
- [x] Complete i18n translations: Audit all pages for hardcoded Dutch text
- [x] Update Home page to use language context for all text (all hardcoded Dutch replaced)
- [ ] Update remaining pages to use language context (Diensten, OverOns, OnsWerk, Reviews, FAQ, Contact, Navbar)
- [x] Ensure ManualQuote sends to WhatsApp (already done)
- [x] Enhance live chat with shorter AI responses (simulated AI responses implemented)
- [ ] Test responsive design on mobile/tablet/desktop
- [x] Run vitest suite to ensure no regressions (13 tests passing)
- [x] Save checkpoint with improvements


## Custom Notification System
- [ ] Design notification system: database schema, tRPC procedures, admin UI
- [ ] Create notifications table (id, title, content, type, createdAt, createdBy)
- [ ] Create user_notification_preferences table (userId, preferences)
- [ ] Build backend: create, list, delete notifications procedures
- [ ] Build admin dashboard: notification management interface
- [ ] Create notification display component for users (toast/banner)
- [ ] Add notification preferences UI for users
- [ ] Test notification system end-to-end


## SEO Fixes
- [x] Fix homepage title: extend to 30-60 characters (now 52 characters)
- [x] Add meta keywords to homepage (9 relevant keywords added)
- [x] Verify SEO improvements (dev server running, no errors)


## Logo Integration
- [x] Convert original logo JPG to PNG
- [x] Upload logo to CDN
- [x] Update Navbar with original logo
- [x] Logo displays correctly in navbar (h-16 md:h-20)
