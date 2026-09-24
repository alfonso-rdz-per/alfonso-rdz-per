# Alfonso Rodriguez Perez

Computer Science student at **UTEP** and founder of **[EasyTap](https://easytap.mx)**, a technology
company that develops software products, NFC solutions and workflow automation for businesses
across Mexico, with a primary focus on Guanajuato and Querétaro.

I design and ship full-stack software end to end, from database schema and security to
deployment, for real users: my university engineering team, restaurants, and client businesses.

**B.S. in Computer Science, Minor in Psychology** · The University of Texas at El Paso\
GPA 4.0/4.0 · Expected graduation: December 2027 · El Paso, TX

---

## Current projects

### ASCE Concrete Canoe · UTEP — Team management platform

**Project Engineer** for the 2027 competition and **sole developer** of the team's software.

Replaces paper sign-in sheets with a secure, phone-based attendance system: the first module
of a platform that will grow into a team and project management tool.

- Rotating QR codes signed with HMAC (new code every 10 s); members check in with their phone
  camera, with no app and no student accounts
- Admin panel for members, sessions, attendance rates, manual corrections and an audit log
- PostgreSQL with Row Level Security, rate limiting and a nonce-based CSP;
  ~800 unit, UI and database tests running in CI

`Next.js` `TypeScript` `Supabase` `PostgreSQL` `Vitest` `Playwright` `Vercel`

**Status:** Attendance module live · platform in development\
[Repository](https://github.com/alfonso-rdz-per/asce-concrete-canoe-utep) · [Live site](https://concretecanoe.easytaps.org)

### SBARRA — Customer feedback SaaS for restaurants (EasyTap)

Customers tap an NFC tag, or scan a QR code, to rate the server who helped them.
Managers follow the results in a dashboard and are alerted when something goes wrong.

**Built**
- NFC-first feedback flow with QR fallback; no app or account needed for customers
- Per-employee ratings, rankings and trends in a business dashboard
- Email and WhatsApp alerts to managers on negative reviews (queued, retried, deduplicated)
- Multi-tenant SaaS architecture: tenant isolation with Row Level Security, subscription plans
  and multiple locations per business

**In development**
- AI-powered analysis of customer feedback
- Customer recovery workflows after a negative experience

`Next.js` `TypeScript` `Supabase` `PostgreSQL` `WhatsApp Cloud API` `Resend` `Vercel`

**Status:** In development · private codebase · [sbarra.easytaps.org](https://sbarra.easytaps.org)

### ASCE Steel Bridge · UTEP — Team website

Building the website for UTEP's ASCE Steel Bridge team for the 2027 competition.

**Status:** Under construction · not yet published

---

## Featured projects

*Public repositories are portfolio versions: client work is anonymized, and EasyTap's production
code stays private.*

### [Travel Itinerary & Proposal Generator](https://github.com/alfonso-rdz-per/travel-itinerary-generator)

Internal tool built for a travel agency. Agents enter the trip essentials; an LLM drafts
day-by-day itineraries and sales proposals, and the app exports branded, ready-to-send PDFs.

- LLM output constrained to a JSON schema and validated with Zod
- Custom PDF rendering: cover page, letterhead, page numbering, embedded fonts
- Supabase Auth with Row Level Security, autosaving editor, Unsplash photo search

`Next.js` `TypeScript` `Supabase` `OpenRouter / Gemini` `react-pdf`

### EasyTap — NFC platform

NFC cards and stickers that turn a table, counter or package into a one-tap link to a
business's menu, social media or Google reviews.

- **[easytap-nfc-server](https://github.com/alfonso-rdz-per/easytap-nfc-server)**: redirect
  backend running in production, handling 800+ NFC taps/redirections per day across all tags.
  Each tag resolves (`/tap/:id`) to a destination the business manages in Google Sheets, so it
  can be changed without reprogramming the tag.
- **[easytap-landing](https://github.com/alfonso-rdz-per/easytap-landing)**: animated marketing
  site built with Next.js, Tailwind CSS and Framer Motion.

`Node.js` `Express` `Google Sheets API` `Next.js` `Framer Motion`

### [Excel Access Control](https://github.com/alfonso-rdz-per/excel-access-control)

Login system for Excel workbooks, built for a client: hashed credentials, account expiration and
locked sheets. Includes **SHA-256 implemented from scratch in VBA**, verified against the
FIPS 180-4 test vectors.

`VBA` `Excel`

---

## Background

- **Project Engineer**, ASCE Concrete Canoe Team, UTEP (2027 competition)
- **Founder**, EasyTap: software products, NFC solutions and automation for businesses in Mexico
- **Participant**, [Olimpiada de Informática del Estado de Guanajuato (OIEG)](https://www.cimat.mx/oieg/),
  2022–2023: competitive programming in C++

## Tech

- **Languages:** TypeScript, JavaScript, SQL, VBA · C++ (OIEG) · Python, Java (UTEP coursework)
- **Web:** Next.js, React, Tailwind CSS, Node.js, Express
- **Data:** Supabase (PostgreSQL, Auth, Row Level Security), Zod
- **Testing & delivery:** Vitest, Playwright, GitHub Actions, Vercel
- **APIs:** LLM APIs (OpenRouter / Gemini), WhatsApp Cloud API, Google Sheets API, Unsplash

## Contact

poncho242410@gmail.com · +1 (915) 526-4750
