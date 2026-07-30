# brand-mention-tracker

Templates and procedures for tracking brand mentions across the web. The "3x signal" from the GEO baseline: brand mentions correlate roughly 3x stronger with AI engine citation than backlinks.

You cannot improve what you do not measure. This repo gives you the measurement.

## What this contains

- `README.md` (this file)
- [01-setup-google-alerts.md](01-setup-google-alerts.md): setting up Google Alerts for brand and competitor tracking
- [02-setup-talkwalker.md](02-setup-talkwalker.md): setting up the free Talkwalker Alerts tier as backup
- `03-tracker-template.csv`: spreadsheet template for the mention log
- [04-monthly-review.md](04-monthly-review.md): monthly review procedure
- [05-categorization-rubric.md](05-categorization-rubric.md): how to classify mentions
- [06-ai-engine-test-template.md](06-ai-engine-test-template.md): monthly direct AI engine test
- [07-outreach-templates.md](07-outreach-templates.md): templates for responding to mentions (thanks, corrections, link requests)
- [08-bad-mention-response.md](08-bad-mention-response.md): how to handle critical mentions, complaints, and disputes
- [09-quarterly-report-template.md](09-quarterly-report-template.md): quarterly mention report for stakeholders
- [10-what-NOT-to-track.md](10-what-NOT-to-track.md): signals that look like data but are noise

## The "3x signal" hypothesis

Per published industry research (cited in the GEO baseline), AI engines correlate citations more strongly with brand mentions across third-party sources than with traditional backlinks. The mechanism is plausible: mentions signal that an entity is being talked about in the language people use to discuss it, which is exactly the language AI engines learn from.

A brand mentioned in 50 sources is treated as a real entity. A brand with 50 backlinks from the same source network may not be.

This means tracking mentions is the highest-impact GEO measurement after the citation test itself.

## Why DIY beats paid tools (in year one)

Paid brand monitoring tools (Brand24, Mention.com, Brandwatch, Sprout) start at $99/month and scale to thousands. For an indie or small-business audit, they are overkill. Google Alerts + Talkwalker Alerts (both free) plus a spreadsheet covers 80% of the value at 0% of the cost.

When you outgrow the free stack, you will know. Until then, this repo is enough.

## How to use

1. Read [01-setup-google-alerts.md](01-setup-google-alerts.md) and create the alerts (15 minutes).
2. Read [02-setup-talkwalker.md](02-setup-talkwalker.md) and create the backup alerts (10 minutes).
3. Copy `03-tracker-template.csv` to a new Google Sheet or Excel file (5 minutes).
4. Each time an alert hits, log it per [05-categorization-rubric.md](05-categorization-rubric.md) (1 minute per mention).
5. Run [04-monthly-review.md](04-monthly-review.md) on the first weekday of each month (30 minutes).
6. Run [06-ai-engine-test-template.md](06-ai-engine-test-template.md) monthly (45 minutes).
7. Quarterly, build the report from [09-quarterly-report-template.md](09-quarterly-report-template.md).

Total ongoing time: about 90 minutes per month.

## Pairs with

- [geo-audit-checklist](https://github.com/0xelitesystem/geo-audit-checklist): full GEO audit; this repo covers the monitoring section
- [llms-txt-generator](https://github.com/0xelitesystem/llms-txt-generator): increase the chance you get cited (this tracks whether you do)
- [ai-citability-scorer](https://github.com/0xelitesystem/ai-citability-scorer): improve passage quality so mentions convert to citations
- [e-e-a-t-auditor](https://github.com/0xelitesystem/e-e-a-t-auditor): improve trust signals across the site

## More

Part of a catalog of single-file browser tools and plain-language references, all MIT licensed and dependency-free: [0xelitesystem.github.io](https://0xelitesystem.github.io/). Built by [elitesystem.ai](https://elitesystem.ai).

## License

MIT. Free to use, fork, adapt.
