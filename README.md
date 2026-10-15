# ANZ marketing skills for Claude Code

Marketing skills for New Zealand, Australia and Auckland. They give Claude Code, and any agent that reads Agent Skills, the local knowledge a marketer in Aotearoa or Australia uses every day: how people here search, what the law says about email and ads, how to spell for each country, when the year turns, and how Auckland's suburbs and communities choose who to buy from.

Built in Auckland by [Amber Lan](https://flowai.co.nz) at Flow AI. Open source under MIT, and open to your pull requests.

## The skills

| Skill | Use it to |
|---|---|
| [`nz-au-local-seo`](skills/nz-au-local-seo/SKILL.md) | Plan local SEO for google.co.nz and google.com.au: Google Business Profile, .nz and .au domains, NZBN and ABN, citations, hreflang, suburb pages |
| [`nz-au-email-sms-compliance`](skills/nz-au-email-sms-compliance/SKILL.md) | Check email, SMS and messaging campaigns against the NZ Unsolicited Electronic Messages Act 2007, the Australian Spam Act 2003 and both Privacy Acts |
| [`nz-au-ad-claims-check`](skills/nz-au-ad-claims-check/SKILL.md) | Review ads, landing pages and social posts against the NZ Fair Trading Act, the Australian Consumer Law and the advertising codes in both countries |
| [`nz-au-spelling-te-reo`](skills/nz-au-spelling-te-reo/SKILL.md) | Localise copy into NZ or Australian English, with GST-inclusive prices and correctly spelled te reo Māori |
| [`nz-au-marketing-calendar`](skills/nz-au-marketing-calendar/SKILL.md) | Build a campaign calendar around public holidays, Matariki, EOFY, the southern summer and school terms |
| [`auckland-local-marketing`](skills/auckland-local-marketing/SKILL.md) | Plan Auckland marketing suburb by suburb, including Neighbourly, local groups, Xiaohongshu and WeChat for Chinese-speaking Aucklanders |

The skills call on each other. A typical run: plan with `auckland-local-marketing`, build search with `nz-au-local-seo`, time it with `nz-au-marketing-calendar`, then check every line with `nz-au-ad-claims-check`, `nz-au-email-sms-compliance` and `nz-au-spelling-te-reo` before it goes live.

## Install

**As a Claude Code plugin (all six skills):**

```
/plugin marketplace add Amberlanqinyun/anz-marketing-skills
/plugin install anz-marketing@anz-marketing-skills
```

**One skill at a time:** copy the skill's folder into `~/.claude/skills/`.

```bash
git clone https://github.com/Amberlanqinyun/anz-marketing-skills.git
cp -R anz-marketing-skills/skills/nz-au-local-seo ~/.claude/skills/
```

Then ask Claude in plain words, for example: "Check this email campaign for New Zealand and Australian spam law" or "Plan local SEO for my physio clinic in Takapuna".

## How the facts are kept honest

Every legal and calendar fact in these skills was checked on an official source (legislation.govt.nz, legislation.gov.au, the Commerce Commission, the ACCC, ACMA, the Department of Internal Affairs, the Privacy Commissioner, the OAIC, the ASA, Ad Standards, Stats NZ, IRD, the ATO and Te Taura Whiri i te Reo Māori). [`SOURCES.md`](SOURCES.md) lists each one with the date it was checked.

Laws, codes and dates change. Each skill tells the agent which points to re-check and to date-stamp its output.

These skills help you prepare and check marketing. They are general information, and they do not replace advice from a lawyer for your situation.

## Contributing

If you market in New Zealand or Australia, your knowledge makes these skills better. Open an issue or a pull request with a correction, a new local channel, or a skill you would like to see, and include the official source for any legal or factual change.

## License

MIT. See [LICENSE](LICENSE).
