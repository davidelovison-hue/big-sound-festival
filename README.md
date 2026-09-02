# Big Sound Festival

Festival ticketing prototype skeleton, forked from [fever-festival-plan](https://davidelovison-hue.github.io/fever-festival-plan/). Same pages, cart, and checkout flow — swap the sample festival data when Big Sound is ready.

## Sample festival (placeholder)

The UI currently uses **Bahidorá 2027** as working sample content so the skeleton is complete. Replace it with Big Sound in:

| File | What to change |
| --- | --- |
| `src/lib/festivalEvent.ts` | Event id, title, venue, dates, logo |
| `src/data/festivalConfig.ts` | Hero media, facts, overview copy, currency |
| `src/data/festivalArtists.ts` | Lineup carousel |
| `src/data/planCatalog.ts` | Tickets, bundles, camping, extras |
| `public/` | Logo, poster, hero video, gallery, product photos |
| `index.html` | Document title |

## App structure

- `/` — plan page (overview, tickets, add-ons)
- `/event/:eventId/connect` — login / social connect
- `/event/:eventId/guest-checkout` — guest details
- `/event/:eventId/checkout` — payment
- `/event/:eventId/pmr-questions` — accessibility questions
- `/event/:eventId/post-booking` — post-purchase
- `/event/:eventId/confirmation` — order confirmation
- `/account` — account

## Commands

```bash
npm install
npm run dev      # http://localhost:5174
npm run build
npm run deploy   # GitHub Pages → big-sound-festival
```

## Live URL

https://davidelovison-hue.github.io/big-sound-festival/
