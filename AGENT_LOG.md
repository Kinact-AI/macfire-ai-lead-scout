# MacFire AI Lead Scout Agent Log

## 2026-06-09 - Claude handoff note

### Current Repo Purpose

This is the standalone static dashboard for MacFire AI Lead Scout. It should stay separate from `macfire-production`.

The production scraper/enrichment pipeline lives in:

- `jonathanmccrimmond/macfire-production`

### Current User Direction

The user explicitly parked Lead Scout dashboard/interface work for now.

Current active work is in Content Radar:

- publish pipeline
- improved editorial dashboard/interface
- calendar of events/content
- human approval before auto-posting

### Existing Dashboard Direction For Later

If the user returns to Lead Scout dashboard work, likely next areas are:

- run observability from `scout_runs`
- contact discovery status
- planning applications signal status
- re-enrichment queue visibility
- clearer lead triage ergonomics

### Safety Notes

- Do not commit Supabase secrets or service-role keys.
- Do not re-nest this repo in `macfire-production`.
- Avoid changing live dashboard behavior unless the user asks to resume Lead Scout work.
