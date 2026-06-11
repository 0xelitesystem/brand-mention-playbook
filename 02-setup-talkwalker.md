# 02. Setting up Talkwalker Alerts (backup)

Talkwalker Alerts is Google Alerts' main alternative. Free tier, similar workflow, different coverage. Catches mentions Google Alerts misses and vice versa. Run both.

## Why also use Talkwalker

- Different crawler, different sources, different latency
- Often catches forum and blog mentions Google Alerts misses
- Covers some non-Western language sources better
- Different ranking of results

The two tools together catch about 1.4x the mentions of either alone.

## How to set up

1. Go to `https://www.talkwalker.com/alerts`
2. Enter your email and the search query in the box on the homepage.
3. Click "Create Alert".
4. Verify your email when the confirmation arrives.
5. Configure each alert:
   - **Result type:** News & Blogs (broadest), Web (less noise), or Discussions (forums and Q&A)
   - **Language:** Your target language
   - **Region:** Worldwide (or restrict if you only serve one region)
   - **Frequency:** Daily (recommended) or Weekly (for low-volume brands)
   - **Number of results:** Only the best results (default) or All

## Recommended alerts

Mirror your Google Alerts setup. Same queries, same priority:

| Query type | Frequency | Result type |
|---|---|---|
| Brand name exact | Daily | News & Blogs |
| Brand name exact | Daily | Discussions |
| Founder name | Daily | News & Blogs |
| Product name | Daily | News & Blogs |
| "Brand alternative" | Weekly | News & Blogs |

The Discussions filter is the value-add over Google Alerts. It catches forum threads, Reddit (sometimes), Q&A sites.

## What Talkwalker catches that Google misses

- Some Reddit comments (variable; Reddit blocks/allows differently by source)
- More foreign-language coverage
- Older archived sources Google has de-indexed
- Some Stack Overflow and Stack Exchange threads
- Quora answers (variable)
- Some Medium articles

## What Talkwalker also misses

- Most private/gated communities (Slack, Discord, Circle, Mighty Networks)
- LinkedIn (most of it)
- Most podcasts
- Most video platforms
- Real-time Twitter/X (use Twitter's native search separately)

## When alerts arrive

Talkwalker bundles a day's hits into one email per query. Google Alerts sends real-time or daily depending on your settings. The combined inbox volume is manageable: 10 to 30 emails per day total for most indie brands.

## Combining the two

Log mentions from both into the same spreadsheet (see `03-tracker-template.csv`). Mark the source in the "Discovered via" column. After 3 months you will see which tool earns its setup time for your brand. Often one is clearly stronger for your niche.

## Other free options to consider

- **X (Twitter) advanced search**: `(@yourhandle) OR (yourbrand)` with a date filter. Bookmark the search URL.
- **Reddit search**: `site:reddit.com "your brand"` in Google works better than Reddit's own search.
- **LinkedIn search**: log in and search your brand name; LinkedIn shows mentions inside its walled garden.
- **Hacker News**: `https://hn.algolia.com/?q=yourbrand` indexes HN posts and comments fast.

For a brand active in tech, the HN search is high signal. Check weekly.

## Don't subscribe to the paid plans yet

Talkwalker has a paid tier ($199+/month). For indie brands the free tier is sufficient. Same for Brand24, Mention.com, etc. Upgrade only when:

- You have over 200 mentions per month and the spreadsheet workflow is breaking down
- You need historical search (paid tools index further back)
- You need API access to feed mentions into a dashboard automatically

If you cannot articulate which of those three needs you have, the free tier is enough.
