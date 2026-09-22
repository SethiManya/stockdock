# StockDock
### Storefront prototype · Next.js · React · Firebase

StockDock is a team-built storefront prototype for browsing products and exploring a store interface. This is **Manya Sethi's portfolio fork** of [JoltedGeo/StockDockPrototype](https://github.com/JoltedGeo/StockDockPrototype), with the original commit history and contributor credit preserved.

## My contribution

I worked on the product discovery experience:

- Built product-name and category search over a sample catalogue.
- Redesigned the homepage with a hero section, product cards, category sections, and responsive layouts.
- Connected the Products navigation to the search page.
- Added a Firestore export to the existing Firebase setup.

[View my implementation commit](https://github.com/JoltedGeo/StockDockPrototype/commit/24495bc570186d99436ea611251441c18dc09036)

| Area | Code |
| --- | --- |
| Product search | [app/search/page.js](app/search/page.js) |
| Homepage | [app/page.js](app/page.js) |
| Navigation | [app/components/Header.js](app/components/Header.js) |
| Firebase initialization | [app/utils/firebase.js](app/utils/firebase.js) |

The complete application is a team project. The features listed above describe my individual contribution.

## Technology

Next.js 16 · React 19 · JavaScript · Tailwind CSS · Firebase Authentication · Firestore

## Run locally

Use a Node.js version supported by Next.js 16 and npm.

```bash
git clone https://github.com/SethiManya/stockdock.git
cd stockdock
npm install
```

Create `.env.local` in the project root and fill these variables with the web-app configuration from **your own Firebase project**:

```dotenv
NEXT_PUBLIC_FIREBASE_API_KEY=
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=
NEXT_PUBLIC_FIREBASE_PROJECT_ID=
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=
NEXT_PUBLIC_FIREBASE_APP_ID=
NEXT_PUBLIC_FIREBASE_MEASUREMENT_ID=
```

Configure the Firebase sign-in providers you intend to use, then start the app:

```bash
npm run dev
```

Open [localhost:3000](http://localhost:3000).

## Development checks

```bash
npm run lint
npm run build
```

These are the repository's available check commands; this documentation update does not certify a passing build or lint result.

## Prototype scope

Product discovery was implemented against sample product data. This repository is presented as a learning and portfolio prototype, not a production commerce service. Authentication and other Firebase-backed behaviour require your Firebase configuration.

## Credits

Original team repository: [JoltedGeo/StockDockPrototype](https://github.com/JoltedGeo/StockDockPrototype). Original authorship is retained in the Git history.

Portfolio contributor: **[Manya Sethi](https://github.com/SethiManya)**.
