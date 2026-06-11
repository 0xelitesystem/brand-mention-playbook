# 06. AI engine direct test

Monthly. 45 minutes. The most direct measurement of GEO progress. Ask the AI engines about your brand and topics, record what they say.

## What you are measuring

- Whether AI engines mention your brand at all
- Whether information is accurate
- Whether AI engines cite your URL or just say your name
- Whether competitors are cited when you are not (and why)

This is your ground truth. Server logs and alerts are leading indicators; AI engine answers are the actual outcome.

## Engines to test

1. ChatGPT (web search enabled)
2. Claude (web search enabled)
3. Perplexity
4. Google AI Overviews (via search.google.com with the test query, on a logged-out incognito session)
5. Optional: Gemini, Copilot

Use the free tier of each. You do not need pro features for this.

## The five baseline prompts

Customize these to your brand. Use the SAME prompts every month to make month-over-month comparable.

1. **Direct brand query:** "What is [YourBrand]?"
2. **Best-of-category query:** "Best [your category] for [your audience]?"
3. **Comparison query:** "How does [YourBrand] compare to [TopCompetitor]?"
4. **Founder query:** "Who is [Founder Name]?" (skip if anonymous)
5. **Alternative query:** "[YourBrand] alternative" or "[TopCompetitor] alternative"

For each prompt, in each engine, log:

- Were you mentioned at all? (Yes/No)
- Was the information accurate? (Yes/Partial/No)
- Were you cited by URL? (Yes/No, which URL)
- Position in the answer (first paragraph / mid / last / not present)
- Competitors cited (which ones)
- Notable phrasing the engine used to describe you

## The log table

For each (prompt, engine) pair, fill in a row:

| Date | Prompt # | Engine | Mentioned | Accurate | Cited URL | Position | Competitors cited | Notes |
|---|---|---|---|---|---|---|---|---|
| 2026-05-15 | 1 | ChatGPT | Yes | Partial | Yes (homepage) | First para | None | Got name right, described us as "an invoice generator" but missed BYOK angle |
| 2026-05-15 | 1 | Claude | Yes | Yes | No | Mid | None | Accurate but not cited |
| 2026-05-15 | 1 | Perplexity | Yes | Yes | Yes (pricing page) | First para | InvoiceMaker | Cited pricing page directly |
| 2026-05-15 | 1 | Google AI Overview | No | N/A | No | N/A | InvoiceMaker, BillPro | Did not appear |

5 prompts x 4 engines = 20 rows minimum per test.

## What to do with the data

### Month over month

- Mentioned count: rising? Falling?
- Accuracy: improving as you fix descriptions on your site?
- URL citations: which pages are being cited? Are those your strongest pages?
- Competitor displacement: are you appearing where competitors used to be? Or vice versa?

### Specific actions per finding

**You are not mentioned at all in any engine for prompt 1:**
You have a discoverability problem (see `01-discoverability.md` in geo-audit-checklist).

**You are mentioned but description is wrong:**
Your homepage or About page is not stating clearly what you do. Rewrite the first paragraph of those pages to lead with the specific claim.

**You are mentioned but not cited by URL:**
Your content is being used as background but not as a citation source. Improve passage citability (see `02-passage-quality.md` in geo-audit-checklist).

**Competitors are always cited and you are not:**
Either you are not in the engine's index, OR your content does not give the engine quotable passages. Check both.

**One engine cites you reliably, another never does:**
Engines weight different signals. Examine what the citing engine has that the non-citing engine lacks. Often it is structured data, often it is sameAs profiles.

## What you cannot measure this way

- Whether anyone is actually clicking through (use server logs and analytics)
- Whether the AI engine answer is causing brand searches (use Search Console branded queries)
- Whether AI engine mentions convert better than traditional traffic (use UTM parameters where possible, though AI engine referral attribution is unreliable)

This test measures perception, not conversion. Pair with the metrics in `09-quarterly-report-template.md` for the full picture.

## Run discipline

- Same prompts every time, in the same order
- Same engines every time
- Same time of day (engines update; testing at the same time controls for daily variance)
- Same fresh incognito session per engine (logged-in personalization corrupts the data)
- Log the answers verbatim where possible; do not summarize

## The honesty test

If you find your brand is consistently cited everywhere, congratulations. If you find your brand is never cited and your action list never changes, your GEO work is not landing. Adjust based on data, not on hope.
