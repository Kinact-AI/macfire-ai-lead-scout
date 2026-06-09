# MacFire AI Lead Scout Dashboard

Static Supabase-backed dashboard for the MacFire lead scout.

## Purpose

This repo is the standalone public dashboard for MacFire's lead-generation system. It reads lead data from Supabase and presents the highest-value opportunities, enrichment status, confidence scoring, and lead detail views.

The production data pipeline itself now lives in:

- `jonathanmccrimmond/macfire-production`

This dashboard repo should stay separate from `macfire-production`.

## Current State

Recent dashboard features already present:

- Lead detail drawer
- Shareable URLs for filters and individual leads
- Street View image panel
- Director appointment history
- Website auto-detection signals
- Google Maps / Places / Street View enrichment display
- Four-dimension confidence scoring

## Files

- `index.html` - main static dashboard UI and client-side logic
- `config.js.example` - example Supabase config
- `config.js` - local/live config if present
- `src/scrapers/social/` - social scraping experiments/support code

## Run

Open `index.html` directly or serve the repo root:

```bash
python3 -m http.server 4173
```

Then open `http://localhost:4173`.

## Current Instruction From User

Lead Scout dashboard/interface work is parked for now.

The active work has moved to Content Radar:

- guarded publish pipeline
- editorial dashboard/interface
- calendar of events/content
- human approval before auto-posting

Do not start Lead Scout dashboard changes unless the user explicitly asks to return to it.

## Related Repos

- Production scout pipeline: `jonathanmccrimmond/macfire-production`
- Content Radar: `jonathanmccrimmond/macfire-content-radar`
- Projects dashboard: `jonathanmccrimmond/macfire-projects-dashboard`

## Claude Notes

- Do not move this repo back into `macfire-production`.
- Do not commit Supabase service-role keys or private credentials.
- Keep this dashboard client-side unless the user asks for a backend.
- If resuming dashboard work later, start with observability, contact discovery state, planning-application signal state, and re-enrichment queue visibility.
