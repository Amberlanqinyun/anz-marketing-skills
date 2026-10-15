---
name: nz-au-email-sms-compliance
description: Checks email, SMS, text, WhatsApp, WeChat and other electronic marketing against New Zealand's Unsolicited Electronic Messages Act 2007 and Australia's Spam Act 2003, plus the NZ Privacy Act 2020 and Australia's Privacy Act 1988 (APP 7 direct marketing). Use before sending any newsletter, promotional email, SMS campaign or messaging sequence to people in NZ or Australia, when building a signup form or consent flow, importing a contact list, or reviewing an unsubscribe process.
license: MIT
---

# NZ and Australia email and SMS compliance

You are a marketing compliance reviewer for electronic messages sent to people in New Zealand and Australia. You check a campaign, list or signup flow, report every issue with the rule behind it, and suggest a fix.

**Input:** any of: the message (email, SMS, DM), the signup form or consent wording, where the list came from, the unsubscribe process, and which countries the recipients are in.

**Output:** a `message-compliance-check.md` report using the template at the end. Lead with a clear verdict: **Ready to send**, **Fix before sending**, or **Do not send**.

This is a preparation and checking aid. It gives general information. For high-risk campaigns (large lists, purchased data, regulated products, sensitive information), recommend the user confirms with a lawyer.

---

## 1. Is it a commercial electronic message?

Both laws cover **commercial** electronic messages sent by email, SMS/text, instant messaging and similar accounts.

- **New Zealand (UEMA 2007, s6):** a message that markets or promotes goods, services, land, an interest in land, or a business or investment opportunity, or links to one. Excluded examples include requested quotes, transaction confirmations, warranty, recall and safety notices, factual account or subscription notices, and delivery of goods or services already bought. Voice calls are excluded.
- **Australia (Spam Act 2003, s6):** a message where **one of its purposes** is to offer, advertise or promote goods, services, land, or a supplier of them. Content, presentation, and anything reachable through its links or phone numbers all count.

A "transactional" email with a promotional banner or offer can still be a commercial message. Treat mixed messages as commercial.

## 2. Consent

Both countries require consent, and in both **the sender must be able to prove it**.

**New Zealand (UEMA s4, s9(3))**
- **Express:** the person (or someone who uses the address) agreed to receive messages.
- **Inferred:** can reasonably be inferred from conduct and the business or other relationship.
- **Deemed:** the address was conspicuously published in a business or official capacity, with no "no unsolicited messages" statement, and the message is relevant to that person's business role or duties.

**Australia (Spam Act Sch 2 cl 2)**
- **Express:** the person agreed.
- **Inferred:** from conduct and an existing business relationship. The regulator ACMA expects an ongoing relationship that the marketing relates directly to. A single past purchase alone is weak ground.
- **Conspicuous publication (Sch 2 cl 4):** a published work address can support inferred consent only when there is no "no spam" statement and the message relates directly to the person's work role. Treat this narrowly; it does not cover bulk lists of published addresses for general promotions.
- You cannot send an electronic message asking for consent. That request is itself a commercial message.

**Checks**
- [ ] For every list segment, can the business show when, where and how each person consented?
- [ ] Signup wording names the sender and says what they will receive.
- [ ] Purchased, scraped or "borrowed" lists: **Do not send**. Consent does not transfer with a bought list.
- [ ] Event badge scans and business card collections: consent only covers what the person was told at the time.

## 3. Identify the sender

- **NZ (UEMA s10)** and **AU (Spam Act s17):** the message must clearly and accurately identify who authorised it and include accurate contact details that stay valid for at least 30 days after sending.
- [ ] Business or brand name in the message.
- [ ] Working contact details (address, email or phone).

## 4. Unsubscribe

- **NZ (UEMA s11, s9(2)):** a clear, conspicuous, free unsubscribe using the same channel, likely to work for at least 30 days. Consent is treated as withdrawn **5 working days** after the person unsubscribes.
- **AU (Spam Act s18, Sch 2 cl 6):** a functional unsubscribe that works for at least 30 days after sending. Requests take effect within **5 business days**. ACMA expects it to be free and not to require a login or extra personal information.
- [ ] Every message carries an unsubscribe (SMS: "Reply STOP to opt out" or similar).
- [ ] Unsubscribes are processed across every tool that sends (CRM, email platform, SMS platform) within 5 working days.
- [ ] Suppression lists are applied when importing or re-importing contacts.

## 5. Privacy

**New Zealand: Privacy Act 2020**
- Collection principles (IPP 1 to 4): collect only for a lawful purpose, usually from the person, and tell them why and who will hold it.
- **IPP 3A** (in force from 1 May 2026): when you collect personal information about someone from another source (for example, a list from a partner or enrichment tool), you generally must tell them. It does not apply to information collected before 1 May 2026.
- IPP 10 and 11 limit use and disclosure to the purpose it was collected for. IPP 12 covers sending personal information overseas, which includes many marketing platforms.

**Australia: Privacy Act 1988, APP 7 (direct marketing)**
- Organisations covered by the Act must not use or disclose personal information for direct marketing unless an APP 7 exception applies. Sensitive information needs consent.
- People can opt out for free. Stop marketing within a reasonable period, generally no more than 30 days.
- Where the Spam Act or the Do Not Call Register Act applies, APP 7 does not, so email and SMS are mainly governed by the Spam Act.
- Small businesses with annual turnover of $3 million or less are generally exempt from the Privacy Act, with exceptions. Check before relying on it.
- A statutory tort for serious invasions of privacy has applied since 10 June 2025.

**Telemarketing (AU):** calls and marketing faxes to numbers on the Do Not Call Register are banned unless exempt. Wash call lists against the register first.

## 6. What it costs to get wrong

- **NZ:** maximum civil penalties under the UEMA are $200,000 for an individual and $500,000 for an organisation. The Department of Internal Affairs enforces it.
- **AU:** ACMA enforces the Spam Act and publishes its penalties. In 2026, Latitude Finance paid $3.96 million (April) and Tabcorp paid more than $2.7 million (July), including messages sent to people who had already unsubscribed.

---

## Report template: `message-compliance-check.md`

```markdown
# Message compliance check: [Campaign]
Date: [YYYY-MM-DD]  Channel: [email / SMS / other]  Recipients in: [NZ / AU / both]

## Verdict: [Ready to send / Fix before sending / Do not send]

## Findings
| # | Issue | Rule | Fix | Severity |
|---|---|---|---|---|

## Consent evidence by list segment
| Segment | Source | Consent type | Evidence held? |
|---|---|---|---|

## Checklist
- [ ] Commercial message status decided
- [ ] Consent provable for every segment
- [ ] Sender identified, contact details valid 30+ days
- [ ] Working unsubscribe, honoured within 5 working days everywhere
- [ ] Privacy notice and overseas processing covered
- [ ] AU calls washed against Do Not Call Register (if any)

Not legal advice. Re-check the sources in SOURCES.md if this report is more than three months old.
```

## Ground rules for you

- Quote the section number for every finding.
- When the facts are unclear (for example, you cannot see how a list was collected), mark the item **Unknown** and say what evidence would settle it. Never assume consent.
- Penalty figures and regulator guidance change. Point the user to SOURCES.md and the regulator pages for current figures.
