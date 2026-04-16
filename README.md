# Van der Bend Onderhoud - Website

Een moderne, geanimeerde website voor Van der Bend Onderhoud met offerte systeem, reviews, en contact formulier.

## Functies

- **Responsive Design**: Werkt perfect op desktop, tablet en mobiel
- **Offerte Systeem**: Multi-stap formulier voor offerteaanvragen
- **Reviews**: 8 realistische klantreviews met sterrenrating
- **Live Chat Widget**: Directe communicatie met klanten
- **Contact Formulier**: Eenvoudige contactmogelijkheid
- **FAQ**: Veelgestelde vragen met zoekfunctie
- **Portfolio**: Galerij van uitgevoerde werkzaamheden
- **Animaties**: Framer Motion animaties voor een modern uiterlijk

## Technologie Stack

- **Frontend**: React 19, Tailwind CSS 4, Framer Motion
- **Backend**: Express 4, tRPC 11
- **Database**: MySQL (via Drizzle ORM)
- **Styling**: Tailwind CSS met custom Van der Bend branding

## Installatie & Lokale Ontwikkeling

```bash
# Dependencies installeren
pnpm install

# Development server starten
pnpm dev

# Tests uitvoeren
pnpm test

# Production build
pnpm build
pnpm start
```

## Omgevingsvariabelen

De volgende omgevingsvariabelen zijn vereist:

- `DATABASE_URL`: MySQL verbindingsstring
- `JWT_SECRET`: Session signing secret
- `VITE_APP_ID`: Manus OAuth app ID
- `OAUTH_SERVER_URL`: OAuth server URL
- `BUILT_IN_FORGE_API_KEY`: API key voor backend services
- `VITE_FRONTEND_FORGE_API_KEY`: API key voor frontend services

## Email Configuratie

Offertes en contactformulieren worden verstuurd naar: **levivdbend@gmail.com**

Email templates zijn geformateerd met bedrijfsnaam "Van der Bend Onderhoud" en bevatten volledige klantinformatie.

**Opmerking**: De huidige implementatie logt emails naar console. Voor productie moet een email service provider (SendGrid, Mailgun, SMTP) worden geïntegreerd in `server/_core/emailService.ts`.

## Database Schema

- **users**: Gebruikersaccounts
- **quotes**: Offerteaanvragen
- **reviews**: Klantreviews
- **faq**: Veelgestelde vragen
- **contact**: Contactformulier inzendingen
- **chat_messages**: Live chat berichten

## GitHub Export

Om de code naar GitHub te exporteren:

1. **Via Manus UI**: Klik op "Settings" → "GitHub" en volg de stappen
2. **Handmatig**: 
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Van der Bend Onderhoud website"
   git remote add origin https://github.com/USERNAME/van-der-bend.git
   git branch -M main
   git push -u origin main
   ```

## Hosting Opties

### Manus Hosting (Aanbevolen)
- Ingebouwde hosting met custom domain support
- Automatische SSL certificaten
- Geen extra configuratie nodig

### Externe Hosting
- **Vercel**: Optimaal voor Next.js/React
- **Netlify**: Eenvoudige deployment
- **Railway**: Full-stack hosting met database
- **Render**: Serverless functions + database

## Tests

Alle tests worden uitgevoerd met Vitest:

```bash
pnpm test
```

Huidige test coverage:
- Auth logout flow
- Quote submission validation
- Review submission
- Contact form submission
- Input validation

## Toekomstige Verbeteringen

- Admin dashboard voor chat replies
- Loading skeleton states
- Email service provider integratie
- Geavanceerde analytics
- Multi-language support

## Support

Voor vragen of problemen, neem contact op via:
- Email: levivdbend@gmail.com
- Telefoon: +31 6 12 34 56 78

---

**Versie**: 1.0.0  
**Laatst bijgewerkt**: April 2026
