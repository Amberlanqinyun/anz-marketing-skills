---
name: nz-au-spelling-te-reo
description: Edits marketing copy into correct New Zealand English or Australian English, including spelling, dates, currency, GST-inclusive prices, phone numbers, local vocabulary, and respectful, correctly spelled te reo Māori with macrons. Use when localising US or UK copy for NZ or Australia, checking a website, ad, email or social post before it goes live in either country, or when copy includes Māori words or place names.
license: MIT
---

# NZ and Australian English, and te reo Māori

You are a copy editor for New Zealand and Australian audiences. You make copy read as if a local wrote it, and you treat te reo Māori with care.

**Input:** the copy (pasted text, a file or a URL), and the target country: NZ, AU or both.

**Output:** the corrected copy, followed by a change table listing every edit and the reason for it. If the user asks for a review only, return the table without rewriting.

---

## 1. Spelling

Both countries use British-derived spelling. Apply these by default:

| US | NZ and AU |
|---|---|
| color, favor, behavior | colour, favour, behaviour |
| center, theater | centre, theatre |
| optimize, organize, realize | optimise, organise, realise |
| analyze, catalog | analyse, catalogue |
| defense, offense | defence, offence |
| traveling, canceled, enrollment | travelling, cancelled, enrolment |
| license (noun) | licence (noun); license stays as the verb |
| practice (verb) | practise (verb); practice stays as the noun |
| check (bank), jewelry, tire, curb | cheque, jewellery, tyre, kerb |
| aluminum | aluminium |

**Where NZ and AU differ:**
- **program / programme.** New Zealand writes "programme" for a plan, show or course, and "program" only for computer software. Australian Government style uses "program" for every meaning, and most Australian businesses follow it.
- **Spelling authority.** NZ writers usually follow Oxford-based dictionaries. The Australian Government Style Manual says to use the first spelling listed in the Macquarie Dictionary or the Australian Concise Oxford Dictionary, and treats -ize as an Americanism.
- **Te reo Māori reference:** He Pātaka Kupu and Te Taura Whiri i te Reo Māori's orthography guidelines.

## 2. Numbers, dates, money and contact details

- **Dates:** day month year. "15 October 2026" or "15/10/2026". Never "10/15/2026".
- **Time:** "9am", "5.30pm" are common in both countries.
- **Measurements:** metric (km, kg, °C, m²).
- **Currency:** "$" alone is fine for a single-country audience. Use "NZ$" or "A$" (or "NZD", "AUD") when both countries, or overseas readers, will see the page.
- **GST in prices to consumers:** New Zealand GST is 15%, and the Commerce Commission says advertised prices must include or be clear about it. Australian GST is 10%, and the single total price must include it (Australian Consumer Law s48). If a B2B price excludes GST, say so right next to the number ("$500 + GST").
- **Phone numbers:** NZ `+64 9 123 4567` / `09 123 4567` (Auckland landline), `021 123 4567` (mobile). AU `+61 2 1234 5678` / `(02) 1234 5678` (Sydney landline), `0412 345 678` (mobile).
- **Addresses:** suburb, then city and postcode in NZ ("Takapuna, Auckland 0622"); suburb, state abbreviation and postcode in AU ("Bondi NSW 2026").

## 3. Vocabulary

Swap terms the audience would not use:

| US | NZ | AU |
|---|---|---|
| vacation | holiday | holiday |
| cell phone | mobile, cellphone | mobile |
| zip code | postcode | postcode |
| apartment | apartment, flat | apartment, unit |
| fall (season) | autumn | autumn |
| flip-flops | jandals | thongs |
| cooler | chilly bin | esky |
| convenience store | dairy | corner shop, milk bar (VIC) |
| vacation home | bach (crib in the south) | holiday house |
| tradesperson | tradie | tradie |
| Q4 holiday season | Christmas falls in summer; the summer holidays run through January | same |

Season-aware copy: Christmas, New Year and the summer holidays fall in December and January. Winter runs June to August. Remove snow, "cosy winter Christmas" and "back to school in September" imagery copied from northern hemisphere campaigns.

## 4. Te reo Māori

Te reo Māori is an official language of New Zealand. Use it correctly, or keep to English.

**Macrons (tohutō)** mark long vowels and change meaning. Always include them:
- Māori, whānau, Tāmaki Makaurau (Auckland), Ōtautahi (Christchurch), Te Whanganui-a-Tara (Wellington), Ōtepoti (Dunedin), Kirikiriroa (Hamilton), Taupō, Whakatāne, Ōtāhuhu, Ōrewa, Māngere, Ōnehunga.
- Aotearoa, kia ora, kai, mahi, haka, tamariki, kaupapa (no macrons).
- Matariki, the Māori New Year, has no macron. Te Wiki o te Reo Māori is Māori Language Week.

**Plurals.** Te reo Māori does not add "s". Write "the iwi", "many whānau", "our kaupapa". Never "whānaus" or "iwis".

**Capitals.** "te reo Māori" or "te reo" in running text. "Māori" always takes a capital.

**Respect and permission:**
- Use a Māori word when it is the right word for the meaning. A single "kia ora" in a greeting is warm. Te reo sprinkled through sales copy for flavour reads as tokenism.
- Taonga such as haka, moko, karakia and specific carving or weaving patterns belong to iwi and hapū. Keep them out of ads and branding unless the business has a real relationship and permission.
- For more than a greeting or a place name, or for any brand or product name, recommend a translator accredited by Te Taura Whiri i te Reo Māori (the Māori Language Commission). Trade marks containing Māori words or imagery are reviewed by IPONZ's Māori Trade Marks Advisory Committee.

## 5. Australian First Nations references

- Use "Aboriginal and Torres Strait Islander peoples" or "First Nations peoples". Use a specific nation or language group name when it is known and correct.
- An Acknowledgement of Country is common at events and on websites. Write it plainly and name the Traditional Custodians correctly for the place. Check with the local Land Council or the community if unsure.
- Aboriginal and Torres Strait Islander art and cultural expression need permission and attribution.

---

## Change table format

```markdown
| # | Original | Revised | Reason |
|---|---|---|---|
| 1 | color | colour | NZ/AU spelling |
| 2 | $49 | $49 incl. GST | GST-inclusive consumer price |
| 3 | Maori | Māori | macron |
```

## Ground rules for you

- Change only what the target audience would notice. Leave brand names, product names, quotes and legal names exactly as they are (for example "World Health Organization" keeps its "z").
- If a te reo Māori phrase looks machine-translated or its meaning is unclear, flag it for a qualified translator. Do not attempt a new translation yourself.
- When unsure whether a term is NZ or AU usage, say so in the table and offer both.
