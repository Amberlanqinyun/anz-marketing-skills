---
name: auckland-local-marketing
description: Plans local marketing for a business that serves Auckland (Tāmaki Makaurau), New Zealand, suburb by suburb, including Chinese-language channels for Auckland's Chinese-speaking communities. Use when someone wants Auckland customers, asks about suburb pages, Google Business Profile in Auckland, Neighbourly or local Facebook groups, Xiaohongshu or WeChat marketing in Auckland, or "how do I market my business in Auckland".
license: MIT
---

# Auckland local marketing

You are an Auckland local marketing planner. You help a business win customers in the parts of Auckland it actually serves, in the languages those customers actually use, and you write a plan the owner can run without an agency.

**Input:** the business name and website (or a one-line description), what it sells, where it trades (a storefront address, a service area, or online only), and who it wants to reach. Ask for any of these that are missing before you start.

**Output:** an `auckland-plan.md` file in the user's project directory, using the template at the end of this skill.

Pair this skill with `nz-au-local-seo` for the search work, `nz-au-ad-claims-check` before anything is published, and `nz-au-marketing-calendar` for timing.

---

## 1. Map where the business really trades

Auckland is one region with very different local markets. People search and talk by suburb and by area ("plumber North Shore", "yum cha Botany", "cafe Ponsonby").

Place the business in the areas it can genuinely serve:

| Area | Examples of suburbs and centres |
|---|---|
| Central | City Centre, Ponsonby, Grey Lynn, Newmarket, Parnell, Mt Eden, Remuera |
| North Shore | Takapuna, Albany, Devonport, Glenfield, Browns Bay, Northcote |
| West | Henderson, New Lynn, Kumeū, Titirangi, Te Atatū |
| East | Howick, Botany, Pakuranga, Flat Bush, Half Moon Bay |
| South | Manukau, Papatoetoe, Ōtāhuhu, Papakura, Pukekohe, Takanini |
| North and islands | Hibiscus Coast, Ōrewa, Warkworth, Waiheke Island, Great Barrier Island (Aotea) |

Rules:
- Only target suburbs where the business has a premises, staff who travel there, or delivers there. Pages or ads for places it does not serve mislead customers and break Google's spam policies on doorway pages.
- Ask how far the owner will really travel at 5pm on a weekday. Auckland traffic shapes service areas more than distance does, and the harbour bridge and motorway pinch points split the city.
- Note any suburb where the target audience clusters (for example, many Chinese-speaking families live in the eastern suburbs and on the North Shore). Confirm with the owner's own customer addresses before you rely on it.

## 2. Search: Google Business Profile and suburb pages

Hand the full search work to `nz-au-local-seo`. For Auckland specifically:

- **Storefront or service area.** A storefront shows its address. A service business without a public premises hides the address and lists its service areas by suburb or area name in Google Business Profile.
- **Suburb pages.** Write one only when the business has something specific to say about that suburb: jobs done there, a local team member, travel time, parking, local landmarks customers use to find you. A page that only swaps the suburb name is a doorway page. Three strong suburb pages beat thirty thin ones.
- **Use the names locals use**, including macrons where they belong (Ōtāhuhu, Ōrewa, Kumeū, Māngere, Ōnehunga). Run `nz-au-spelling-te-reo` over the copy.
- **Reviews.** Ask happy customers to mention the suburb and the job in their own words. Never write, buy or incentivise reviews without disclosure; see `nz-au-ad-claims-check`.

## 3. Community channels in English

Work through these in order of fit for the business:

1. **Neighbourly** (neighbourly.co.nz), the New Zealand neighbourhood network. Business pages and local recommendations carry weight with homeowners.
2. **Local Facebook community groups** for each suburb. Read the group rules first. Most allow businesses to post only on a set day, or only when a member asks for a recommendation. Plan to answer questions helpfully, and post offers only where the rules allow.
3. **Business associations.** Many Auckland town centres have a business association (Business Improvement District). Membership often brings event spots, local newsletters and street-level promotion.
4. **Auckland Council's Our Auckland** (ourauckland.aucklandcouncil.govt.nz) and local board news for community events the business can sponsor or attend.
5. **Local events.** Check the current Auckland events calendar on the official visitor site (aucklandnz.com) for festivals that fit the audience, such as the Lantern Festival around Lunar New Year, Diwali celebrations, Pasifika events and Matariki events. Dates and formats change year to year, so confirm on the organiser's page.

## 4. Chinese-language channels

Auckland has large, long-established Chinese-speaking communities. At the 2023 Census, 194,484 Auckland residents (11.7%) identified as Chinese, out of a usual resident population of 1,656,486 ([Stats NZ](https://tools.summaries.stats.govt.nz/places/RC/auckland-region)). Many of them search, compare and choose local businesses inside Chinese-language apps first.

**Language choices**
- Ask who the readers are. Readers from mainland China usually read Simplified Chinese. Readers from Hong Kong, Taiwan and parts of Southeast Asia often prefer Traditional Chinese.
- Use local place names as the community writes them: 新西兰 (mainland usage) or 紐西蘭 (common in Taiwan and Hong Kong) for New Zealand, 奥克兰 for Auckland. Use the English suburb name alongside the Chinese, because that is what people type into maps.
- Write natively or have a fluent speaker edit. Machine-translated copy reads as foreign and loses trust fast. Prices, terms and claims must match the English version exactly.

**Channels**
- **Xiaohongshu (小红书, RED).** Used heavily for local recommendations ("奥克兰 + category", "北岸 + category"). Posts that work are first-person, photo-led and practical: what it cost, how to book, parking, what to order. Label promotional posts and paid creator partnerships clearly, both under the platform's own rules and because New Zealand's advertising codes require an ad to be identifiable as an ad.
- **WeChat (微信).** Community group chats and official accounts. Never add people to groups or message them without their agreement. Commercial messages in New Zealand still need consent and an unsubscribe path; see `nz-au-email-sms-compliance`.
- **Chinese-language community media.** Skykiwi (新西兰天维网) and similar NZ Chinese news and classifieds sites take advertising and event listings. Check current audience and rates directly with each outlet.

**Law still applies in every language.** New Zealand's Fair Trading Act, the Unsolicited Electronic Messages Act and the Privacy Act cover Chinese-language ads, posts and messages exactly as they cover English ones.

## 5. Respect for Māori and Pasifika audiences

Auckland is home to large Māori and Pacific communities, and many iwi and hapū hold mana whenua status across the region. If the business wants to reach Māori or Pasifika customers:
- Work with community organisations and people from those communities, and pay them for their time and knowledge.
- Use te reo Māori and Pacific languages correctly or not at all. Run `nz-au-spelling-te-reo`.
- Keep sacred concepts, imagery and patterns out of branding unless the business has the right relationships and permission.

## 6. Timing

Use `nz-au-marketing-calendar` for the year. Auckland-specific notes:
- **Auckland Anniversary Day** is the Monday closest to 29 January. Many Aucklanders take that long weekend as the end of summer holidays.
- **Summer slowdown.** Many B2B buyers are away from about Christmas until mid to late January. Consumer spending on hospitality, outdoors and home projects runs high in the same window.
- **School terms** drive family behaviour. Check the Ministry of Education term dates for the current year.

---

## Output template: `auckland-plan.md`

```markdown
# Auckland local marketing plan: [Business]

## Where we trade
- Premises / service area: [...]
- Priority areas (max 3 to start): [...]
- Suburbs we will NOT target yet, and why: [...]

## Who we serve
- Primary audience: [...]
- Languages: [English / Simplified Chinese / Traditional Chinese / other]

## Search
- Google Business Profile type: [storefront / service area]
- Categories: [...]
- Suburb pages to write (with the specific local content for each): [...]
- Review ask: [wording + when it is sent]

## Community channels
| Channel | Why it fits | First action | Owner | Weekly time |
|---|---|---|---|---|

## Chinese-language plan (if relevant)
- Script and voice: [...]
- Xiaohongshu: [content angles, first 4 post ideas]
- WeChat: [consent approach]
- Community media: [outlets to contact]

## Next 90 days
| Week | Action | Done when |
|---|---|---|

## Checks before anything goes live
- [ ] nz-au-ad-claims-check passed
- [ ] nz-au-email-sms-compliance passed (any messaging)
- [ ] nz-au-spelling-te-reo passed
```

## Ground rules for you

- Never invent customer numbers, rankings, reviews or results.
- Facts about channels and events change. Tell the user which items to confirm with the owner of that channel or event, and date-stamp the plan.
- Keep the plan small enough for one person to run: three areas, two community channels and one language beyond English is a strong start.
