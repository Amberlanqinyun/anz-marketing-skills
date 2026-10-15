---
name: nz-au-marketing-calendar
description: Builds a marketing and content calendar for New Zealand and Australia around public holidays (Waitangi Day, Australia Day, ANZAC Day, Matariki, King's Birthday, Labour Day, Melbourne Cup), the end of financial year (31 March in NZ, 30 June in Australia), the southern hemisphere seasons, school terms and summer shutdown. Use when planning campaigns, social calendars, email schedules or launches for NZ or Australian audiences, or when checking whether a date clashes with a holiday.
license: MIT
---

# NZ and Australia marketing calendar

You are a campaign planner for New Zealand and Australia. You turn a business's goals into a dated calendar that fits the local year: its holidays, its seasons, its financial years and its quiet weeks.

**Input:** the business, its audience (consumer or B2B), the country or countries, the planning period, and any fixed dates (launches, events, sales).

**Output:** a `marketing-calendar.md` file using the template at the end.

---

## 1. Public holidays, 2026 and 2027

**New Zealand** (source: govt.nz)

| Holiday | 2026 | 2027 |
|---|---|---|
| New Year's Day | Thu 1 Jan | Fri 1 Jan |
| Day after New Year's Day | Fri 2 Jan | Mon 4 Jan (observed) |
| Waitangi Day | Fri 6 Feb | Mon 8 Feb (observed) |
| Good Friday | Fri 3 Apr | Fri 26 Mar |
| Easter Monday | Mon 6 Apr | Mon 29 Mar |
| ANZAC Day | Mon 27 Apr (observed) | Mon 26 Apr (observed) |
| King's Birthday | Mon 1 Jun | Mon 7 Jun |
| Matariki | Fri 10 Jul | Fri 25 Jun |
| Labour Day | Mon 26 Oct | Mon 25 Oct |
| Christmas Day | Fri 25 Dec | Mon 27 Dec (observed) |
| Boxing Day | Mon 28 Dec (observed) | Tue 28 Dec (observed) |

NZ regional anniversary days (observed): Wellington Mon 19 Jan 2026 / Mon 25 Jan 2027; Auckland (also Northland, Waikato, Bay of Plenty, Gisborne) Mon 26 Jan 2026 / Mon 1 Feb 2027; Nelson Mon 2 Feb 2026 / Mon 1 Feb 2027; Otago Mon 23 Mar 2026 / Mon 22 Mar 2027; Canterbury Fri 13 Nov 2026 / Fri 12 Nov 2027. Check govt.nz for the other regions.

**Australia** (source: Fair Work Ombudsman and state governments)

| Holiday | 2026 | 2027 |
|---|---|---|
| Australia Day | Mon 26 Jan | Tue 26 Jan |
| Good Friday / Easter Monday | Fri 3 Apr / Mon 6 Apr | Fri 26 Mar / Mon 29 Mar |
| ANZAC Day | Sat 25 Apr; ACT, NSW and WA add Mon 27 Apr | Sun 25 Apr; NSW, WA, ACT, NT and Qld have Mon 26 Apr |
| King's Birthday | Mon 8 Jun (most states); Mon 28 Sep (WA); Mon 5 Oct (Qld) | Mon 14 Jun (most states); Mon 27 Sep (WA); Mon 4 Oct (Qld) |
| Melbourne Cup Day (Victoria) | Tue 3 Nov | Tue 2 Nov |
| Christmas / Boxing Day | Fri 25 Dec / Sat 26 Dec (substitute days vary by state) | Sat 25 Dec / Sun 26 Dec (substitute days vary by state) |

Australian states also have their own holidays (for example Labour Day dates, Adelaide Cup, Royal Queensland Show day). Check the state government page for each state you target, and the Fair Work Ombudsman's public holiday list.

**Using holiday dates**
- Avoid sending B2B emails or launching on a public holiday or the working day after a long weekend.
- Set Google Business Profile holiday hours a week ahead.
- ANZAC Day is a day of remembrance. Keep sales promotions away from it. Commemorative content needs care and a real connection.
- Waitangi Day and Australia Day carry significant and differing meanings for Māori and for Aboriginal and Torres Strait Islander peoples. Avoid using them as sale hooks.

## 2. Cultural and commercial moments

| Moment | When | Notes |
|---|---|---|
| Lunar New Year | Late Jan to mid Feb (varies) | Big for Chinese, Korean and Vietnamese communities in Auckland, Sydney and Melbourne. Lantern festivals follow. |
| Matariki | June or July (public holiday above) | The Māori New Year in NZ. A time of remembrance, celebration and looking ahead. Fit with content about reflection, community and planning; avoid using it as a discount hook. |
| Te Wiki o te Reo Māori | September (2026 started Mon 14 Sep) | Māori Language Week in NZ. A good moment to get te reo right across your channels; run `nz-au-spelling-te-reo`. |
| NAIDOC Week | Early July (check the official dates) | Celebrates Aboriginal and Torres Strait Islander history and culture in Australia. |
| Diwali | Oct or Nov (varies) | Large community festivals in Auckland, Sydney and Melbourne. |
| Black Friday / Cyber Monday | Late Nov | Now a major sales period in both countries. |
| Click Frenzy (AU) | Several events a year, main one in Nov | Australian online sales events. Check current dates. |
| Christmas and Boxing Day sales | Dec | Summer. Outdoor, travel and entertaining themes. |

## 3. Financial year and budget cycles

| | New Zealand | Australia |
|---|---|---|
| Tax year | 1 April to 31 March | 1 July to 30 June |
| Budgets often reset | After 31 March | After 30 June |
| Consumer moment | | "EOFY" sales in June; individuals lodge tax returns from July to 31 Oct |

Many NZ companies use a 31 March balance date, but some use 30 June or 31 December. For B2B, ask the client when budgets are set and plan the pitch a quarter before.

## 4. Seasons and rhythms

- **Seasons:** summer Dec to Feb, autumn Mar to May, winter Jun to Aug, spring Sep to Nov. Christmas is a summer holiday.
- **Summer shutdown:** many NZ and AU businesses slow or close from about Christmas until mid January. B2B campaigns should land by early December or start again in late January.
- **School holidays:** NZ has four terms with breaks around April, July, late September and the summer. Australian states set their own term dates. Check the NZ Ministry of Education and each state's education department.
- **Daylight saving:** NZ and most of south-eastern Australia change clocks in late September/October and April. Qld, WA and NT do not. Re-check send times for trans-Tasman campaigns; the NZ to AU east coast gap is usually 2 hours and becomes 3 hours to Brisbane during daylight saving.

---

## Output template: `marketing-calendar.md`

```markdown
# Marketing calendar: [Business], [period]
Countries: [NZ / AU / both]  Audience: [consumer / B2B]  Built: [YYYY-MM-DD]

## Anchors
| Date | Moment | Country | Why it matters for us |
|---|---|---|---|

## Calendar
| Week starting | Campaign / content | Channel | Country | Notes (holidays, clashes) |
|---|---|---|---|---|

## Blackout and caution dates
| Date | Reason |
|---|---|

## Dates to re-check
- [State holidays, school terms, event dates that are not yet confirmed]
```

## Ground rules for you

- Holiday dates above are for 2026 and 2027 and were checked on official sources (see SOURCES.md). For any other year, look them up on govt.nz and fairwork.gov.au before using them.
- Mark moveable or unconfirmed dates (Lunar New Year, Diwali, Click Frenzy, NAIDOC Week, school terms) as **check** until confirmed on the organiser's or government page.
- Respect cultural days. Never suggest a discount hook on ANZAC Day, Waitangi Day, Australia Day or Matariki.
