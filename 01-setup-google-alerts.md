# 01. Setting up Google Alerts

Google Alerts is the free baseline. Imperfect coverage but free, easy, and works.

## What to set up

You need 5 categories of alerts at minimum.

### Category 1: Brand name (exact match)

```
"YourBrandName"
```

Wrap in double quotes to force exact phrase match. Without quotes Google treats it as separate words and you get noise.

### Category 2: Brand variations and misspellings

Set one alert per common variation. Examples:

```
"Your Brand Name"
"YourBrand"
"your-brand"
"yourbrand.com"
```

If your brand has common misspellings, add those too. Example: "WordPress" needs "Wordpress" and "Word Press" as separate alerts.

### Category 3: Founder name (if a personal brand)

```
"Founder Full Name"
```

Add common variations:

```
"FName LName"
"F. LName"
```

### Category 4: Product-specific terms

If your product name is unique enough to be search-worthy:

```
"YourProductName"
"YourProductName review"
"YourProductName alternative"
```

### Category 5: Competitor mentions (optional but useful)

```
"YourBrand vs CompetitorA"
"YourBrand vs CompetitorB"
"CompetitorA alternative"
```

The last one is high signal: people searching for alternatives to your competitor are exactly your prospects.

## How to create the alerts

1. Go to `https://www.google.com/alerts`
2. Sign in with the Google account you want to receive alerts at.
3. Enter the search query in the box.
4. Click "Show options" and set:
   - **How often:** As-it-happens (for real-time) or At most once a day (less noisy)
   - **Sources:** Automatic (or restrict to News + Blogs + Web for less noise)
   - **Language:** Your target language
   - **Region:** Any region (unless your brand is region-specific)
   - **How many:** Only the best results (recommended) or All results (for very low-volume brands)
   - **Deliver to:** your email
5. Click "Create Alert"

Repeat for each query.

## Recommended alert configuration

| Query type | Frequency | Sources | Quantity |
|---|---|---|---|
| Brand name exact | As-it-happens | Automatic | All results |
| Brand variations | Daily | Automatic | Best results |
| Founder name | Daily | News + Blogs + Web | Best results |
| Product name | As-it-happens | Automatic | All results |
| Competitor "vs" | Daily | News + Blogs + Web | Best results |
| Competitor "alternative" | Daily | News + Blogs + Web | Best results |

## What Google Alerts misses

- Reddit comments (Google indexes posts, comments unreliably)
- Slack/Discord/private community mentions (not indexed at all)
- Many forum platforms
- LinkedIn posts (Google indexes some, not all)
- YouTube video transcripts (sometimes indexed late)
- TikTok/Instagram captions (mostly missed)
- Podcasts (transcripts mostly not indexed)

For these you need additional tools (see `02-setup-talkwalker.md` for partial coverage) or platform-native searches.

## What you'll get

The first week you may get 0 to 50 emails depending on brand volume. Expect:

- 30 to 60 percent noise (duplicates, irrelevant matches)
- 20 to 30 percent neutral mentions (someone shared a link, you got listed in a directory)
- 10 to 20 percent positive (review, recommendation, citation)
- 5 to 10 percent negative or critical
- 1 to 5 percent worth taking action on

Log everything per `03-tracker-template.csv`. The signal compounds over months.

## Tuning the noise

After 2 weeks, you will know what false positives are eating your time. Common patterns:

- A common phrase that overlaps with your brand name: refine query with additional context.
  - Bad: `"Cole"` -> matches every Cole in the world
  - Better: `"Cole Research" -recipe -football`
- Aggregators that auto-include you in lists: block by adding `-aggregatorname` to query.
- News syndication of the same story: accept the dupes; same-story dupes mean you got picked up.

## When to upgrade

If you receive over 100 mentions per month and the spreadsheet workflow is breaking down, time to consider a paid tool. Until then, Google Alerts + Talkwalker free tier covers it.
