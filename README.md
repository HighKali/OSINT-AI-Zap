# OSINT AI Zap 🚀

## La piattaforma OSINT AI più avanzata e completa

### Funzionalità chiave

- **Ricerca OSINT multi-fonte (Hunter.io, ipinfo, social, domini, email, etc.)**
- **Scraping serverless (Vercel/Netlify/Cloudflare Workers)**
- **Agente AI (GPT-4/HuggingFace, plug&play, history, multi-lingua, prompt specializzati)**
- **Login/social login GitHub OAuth, JWT, dashboard utente**
- **Bookmark, cronologia, preferenze, esportazione, dark/light mode**
- **Gestione team/collaboratori, ruoli, API key, rate limit**
- **Logging avanzato, analytics, GDPR/privacy**
- **API pubblica documentata**
- **Test automatici, CI/CD, Docker ready**
- **Responsive, accessibilità, SEO**

---

## Deploy e setup

### 1. Frontend (GitHub Pages)

- Forka o clona questo repo.
- Personalizza `index.html`, `style.css`, `script.js` nella root.
- Attiva GitHub Pages dalla branch main.
- Sito live su `https://tuo-username.github.io/osint-ai-zap`.

### 2. Backend serverless (Vercel/Netlify/Cloudflare)

- Crea directory `/api` con i file backend.
- Deploya su Vercel, imposta env:
  - `GITHUB_CLIENT_ID`
  - `GITHUB_CLIENT_SECRET`
  - `HUNTER_API_KEY` (e altre)
  - `JWT_SECRET`
  - `IPINFO_TOKEN` (opzionale)
- Ottieni la URL tipo `https://osint-ai-zap-backend.vercel.app/api/osint-scrape`
- Modifica frontend per puntare a questa URL.

### 3. OAuth GitHub

- Crea una app su https://github.com/settings/developers
- Imposta redirect URI su `/api/github-oauth` del backend
- Aggiorna client_id nel frontend

### 4. Logging, analytics, team

- `/api/analytics` per logging GDPR compliant
- `/api/admin` gestione ruoli, blacklist, ban, audit

### 5. Test, CI/CD

- Test con `npm test`
- Lint con `npm run lint`
- Deploy automatico GitHub Actions (opzionale)

---

## Supera la concorrenza

- Scraping multi-fonte, AI integrato, dark mode, dashboard, logging, team, API pubblica, test automatici
- Pronto per scaling e custom branding
- Massima privacy e sicurezza

---

## Come contribuire

- Forka, proponi PR, apri issue
- Documentazione API e moduli su `/docs`
- Team e ruoli gestibili via admin

---

## License

MIT

---

Creato da HighKali, 2025
