# CMRA / Mailbox / Virtual Office ZIP Checker

A simple, factual web tool that lets attorneys and serve managers check any ZIP code and see which addresses in that area are registered commercial mail receiving agencies (CMRAs), UPS Stores, mailbox shops, or virtual offices.

## Why it exists

Process servers sometimes list a mailbox or virtual-office address as their "office," especially near CT Corporation's registered-agent counter. This tool flags the address type so the question becomes: is there a staffed counter at this exact suite during business hours?

## How it works

- Open `index.html` in a browser, or host it anywhere (GitHub Pages, Netlify, etc.).
- Enter a 5-digit ZIP code.
- It returns every flagged address in that ZIP, labeled as Mailbox/CMRA, Virtual Office, or Real Staffed Office.
- No process server names are listed — only addresses and what they are.

## Data source

Seed data is compiled from public records:

- USPS CMRA registry (commercial mail receiving agencies)
- Known UPS Store and mailbox shop locations
- Virtual office providers (e.g., Regus)

The list is intentionally small and factual. Expand `LOCATIONS` in `index.html` as you verify more addresses.

## Embed on Durable

1. Turn on GitHub Pages: repo → Settings → Pages → Source: Deploy from branch `main`, folder `/ (root)`.
2. In Durable, add an **Embed** section and paste:

```html
<iframe src="https://royjamesbates.github.io/cmra-zip-checker" width="100%" height="640" style="border:0;border-radius:12px;" loading="lazy" title="CMRA ZIP Checker"></iframe>
```

## License

Use freely. Factual public-record data.
