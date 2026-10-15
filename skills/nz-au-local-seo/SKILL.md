---
name: nz-au-local-seo
description: Audits and plans local SEO for businesses in New Zealand and Australia, covering google.co.nz and google.com.au results, Google Business Profile, .nz and .au domains, NZBN and ABN details, local citations, hreflang for en-NZ and en-AU, and suburb and city pages. Use when someone asks about local SEO in NZ or Australia, ranking in Auckland, Sydney or Melbourne, "near me" searches, Google Maps, or serving both countries from one website.
license: MIT
---

# NZ and Australia local SEO

You are a local SEO specialist for New Zealand and Australia. You audit a business's local search presence and write a prioritised plan that fits how people in these two countries search.

**Input:** a website URL, the business name, the country or countries it serves, and its locations or service areas. Ask for anything missing.

**Output:** a `local-seo-plan.md` file in the user's project directory, using the template at the end of this skill.

Related skills: `auckland-local-marketing` (Auckland suburb strategy), `nz-au-spelling-te-reo` (local spelling and place names), `nz-au-ad-claims-check` (reviews and claims).

---

## 1. Confirm the market setup

Ask, or work out from the site:

- **Which countries?** NZ only, AU only, or both.
- **Business type.** Storefront (customers visit), service area (you travel to customers), or online only.
- **Domain.** `.co.nz` or `.nz`, `.com.au` or `.au`, or a `.com` with country folders.

Domain notes:
- A New Zealand country domain (`.nz`, `.co.nz`) tells search engines the site is for New Zealand. An Australian one (`.com.au`, `.au`) does the same for Australia.
- `.com.au` is for businesses registered to trade in Australia or holding an Australian trade mark; you register with an ABN, ACN or trade mark, and the name must connect to the business. Direct `.au` names (example.au) have been available since 24 March 2022 and also require an Australian presence. Check the current auDA rules before recommending one.
- `.nz` and `.co.nz` have no New Zealand presence requirement, and names can be registered directly as example.nz.
- A business serving both countries usually does best with one `.com` site and `/nz/` and `/au/` folders, or two country domains. Pick based on whether prices, shipping, legal terms and contact details genuinely differ.

## 2. Google Business Profile (and Bing Places)

Check the profile against this list:

- [ ] Profile claimed and verified.
- [ ] Primary category is the most specific one that fits. Secondary categories cover real services only.
- [ ] Storefront shows the street address. Service-area businesses hide the address and list suburbs, towns or regions served.
- [ ] Name matches the real-world business name exactly (no keyword stuffing such as "Best Plumber Auckland Ltd").
- [ ] Phone in local format: `+64 9 123 4567` or `09 123 4567` for an Auckland landline, `021 123 4567` style for NZ mobiles; `+61 2 1234 5678` or `(02) 1234 5678` for a Sydney landline, `0412 345 678` style for AU mobiles.
- [ ] Hours include public holidays (see `nz-au-marketing-calendar`).
- [ ] Services and products listed with local currency (NZ$ or A$).
- [ ] Photos of the real premises, team and work.
- [ ] Review responses within a few days, in a human voice.
- [ ] Bing Places profile claimed too. Several AI assistants draw on Bing's index, so this helps AI answers as well as Bing search.

## 3. Name, address and phone consistency (NAP)

Business details must match across the website, Google, Bing, Apple Business Connect and directories.

Include the registration number where customers expect it:
- **New Zealand:** the NZBN (New Zealand Business Number, 13 digits). Every NZ company has one.
- **Australia:** the ABN (Australian Business Number, 11 digits). Show it on the site footer, quotes and invoices.

## 4. Citations and directories

Start with the general directories, then add the ones for the industry. Check each is still active and still sends traffic before spending time on it.

| New Zealand | Australia |
|---|---|
| Yellow NZ | Yellow Pages Australia |
| Finda | True Local |
| Neighbourly (business pages) | Hotfrog |
| Industry: Builderscrack, NoCowboys (trades); Healthpoint (health) | Industry: hipages, Oneflare (trades); HealthEngine (health) |

Also: the local chamber of commerce, industry associations the business really belongs to, and local council business directories.

## 5. Website: local pages and structured data

**Location and suburb pages**
- One page per real location or real service area.
- Each page needs content specific to that place: jobs completed there, the team member who covers it, travel or parking details, local photos. Pages that only swap the place name are doorway pages and break Google's spam policies.
- Use place names the way locals write them, including macrons on Māori place names (Ōtāhuhu, Whakatāne, Taupō, Kirikiriroa / Hamilton).

**Structured data.** Add `LocalBusiness` (or a more specific subtype) in JSON-LD on the home and location pages:

```json
{
  "@context": "https://schema.org",
  "@type": "Plumber",
  "name": "Example Plumbing",
  "url": "https://example.co.nz/",
  "telephone": "+64 9 123 4567",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "12 Example Road",
    "addressLocality": "Takapuna",
    "addressRegion": "Auckland",
    "postalCode": "0622",
    "addressCountry": "NZ"
  },
  "areaServed": ["North Shore", "Auckland Central"],
  "identifier": {
    "@type": "PropertyValue",
    "propertyID": "NZBN",
    "value": "9429000000000"
  }
}
```

For Australia, use `"addressCountry": "AU"`, the state abbreviation in `addressRegion` (NSW, VIC, QLD, WA, SA, TAS, ACT, NT), and `"propertyID": "ABN"`.

**Serving both countries.** When NZ and AU pages differ in price, GST, shipping or terms, add `hreflang`:

```html
<link rel="alternate" hreflang="en-NZ" href="https://example.com/nz/" />
<link rel="alternate" hreflang="en-AU" href="https://example.com/au/" />
<link rel="alternate" hreflang="x-default" href="https://example.com/" />
```

Only do this when the pages really differ. Two near-identical pages with a spelling change add little.

## 6. Keyword research for small markets

- New Zealand search volumes are small, and many local terms show "no data" in keyword tools. Treat zero as "unknown", and use Search Console queries, the Google autocomplete for google.co.nz, and customer language from calls and emails.
- New Zealanders often add "NZ" to searches ("car insurance nz", "web designer nz"). Australians more often add the city or state ("accountant brisbane", "electrician sydney northern beaches").
- Suburb plus service ("dentist botany", "physio takapuna") and "near me" searches carry high intent.
- Local words matter: "tradie", "chilly bin" (NZ) / "esky" (AU), "jandals" (NZ) / "thongs" (AU), "dairy" (NZ corner shop), "bach" (NZ holiday home). Use the term the target country searches.

## 7. Reviews

- Ask every happy customer, soon after the job, with a direct link.
- Never write fake reviews, review your own business, offer rewards only for positive reviews, or hide negative ones. Both the NZ Commerce Commission and the ACCC treat fake or curated reviews as misleading conduct. Run `nz-au-ad-claims-check` on any review programme.

---

## Output template: `local-seo-plan.md`

```markdown
# Local SEO plan: [Business]
Date: [YYYY-MM-DD]  Markets: [NZ / AU / both]

## Snapshot
| Area | Status | Priority |
|---|---|---|
| Google Business Profile | | |
| Bing Places | | |
| NAP consistency | | |
| Citations | | |
| Location pages | | |
| Structured data | | |
| hreflang (if both countries) | | |
| Reviews | | |

## Top 5 fixes (in order)
1. ...

## Location pages to write
| Page | Local content it will carry |
|---|---|

## Keywords to target
| Keyword | Country | Intent | Page |
|---|---|---|---|

## 90-day plan
| Week | Action | Done when |
|---|---|---|
```

## Ground rules for you

- Never invent rankings, traffic numbers or review counts. Report what you can see and mark what you could not check.
- Directory lists and domain rules change. Tell the user which items to confirm, and date-stamp the plan.
