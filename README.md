# Startupy

Plateforme Next.js qui accompagne les entrepreneurs tunisiens de l'idée au financement.

## Stack

- Next.js 15 (App Router) · TypeScript · Tailwind CSS v4
- Zustand (profil fondateur + progression)
- Vitest (scoring & déblocage d'étapes)

## Démarrage

```bash
npm install
npm run dev
```

Ouvrir [http://localhost:3000](http://localhost:3000).

## Scripts

| Commande | Description |
|----------|-------------|
| `npm run dev` | Serveur de développement |
| `npm run build` | Build production |
| `npm test` | Tests unitaires (roadmap / score) |

## Routes

| Route | Description |
|-------|-------------|
| `/` | Landing |
| `/diagnostic` | Questionnaire adaptatif |
| `/dashboard` | Roadmap + score de préparation |
| `/roadmap/[step]` | Détail d'étape + critères de déblocage |
| `/chatbot` | Assistant juridique (4 blocs + sources) |
| `/investisseurs` | Dealflow startups |
| `/login` | Placeholder auth |

## Logique métier

- **Roadmap adaptative** — étapes conditionnelles selon diagnostic (société, devises, international, cofondateurs, objectif levée)
- **Déblocage** — critères de complétion obligatoires ; message explicite si éléments manquants
- **Score** — préparation multi-critères (0–100), explicitement non financier
