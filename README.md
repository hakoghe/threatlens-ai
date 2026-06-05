# ThreatLens AI

AI-powered threat intelligence and phishing detection platform.

ThreatLens AI analyzes URLs, emails, and domains to detect phishing,
brand impersonation, and related threats, and produces analyst-style
investigation reports backed by machine-learning models.

## Status

Early development — see the roadmap below.

## Features (planned)

- URL scanner with risk and confidence scoring
- Email scanner for `.eml` / `.msg` files
- Threat intelligence engine (domain age, SSL, DNS, WHOIS, reputation)
- Brand impersonation detection with similarity scoring
- AI investigation reports
- Threat intelligence search (domains, URLs, IPs, emails, hashes)
- Analytics dashboard
- Documented public API
- Chrome browser extension

## Tech stack

- **Frontend:** React, TypeScript, Tailwind CSS
- **Backend:** Python, FastAPI
- **Machine learning:** scikit-learn, XGBoost
- **Database:** PostgreSQL
- **Auth:** JWT
- **Containerization:** Docker
- **CI/CD:** GitHub Actions

## Architecture

A modular monolith with clean internal boundaries
(API → services → repositories), a separate offline ML training
pipeline, and a Chrome extension client. See `docs/architecture.md`.

## Getting started

> Full setup instructions arrive in Phase 2.

```bash
cp .env.example .env   # then fill in local values
```

## Roadmap

- [x] Phase 1 — Architecture, repository, folder structure
- [ ] Phase 2 — FastAPI backend
- [ ] Phase 3 — PostgreSQL
- [ ] Phase 4 — Authentication
- [ ] ... (phases 5–15)

## License

MIT — see [LICENSE](./LICENSE).