# Brand voice & design rules for dakshvanshaj.com

Distilled from building the actual template sites this portfolio links to (CloseLoop, FirstReply, SnapTally,
RecapRelay) — each rule below is something that was tried, got corrected by the site's owner, and confirmed
right afterward. Not theory.

## Copy

- **Zero jargon on any page a visitor lands on first** (homepage, project cards): no "webhook," "polling," cron
  times, internal field/status names, or a build/test-status table. That detail is legitimate, but it belongs on
  a separate deep "how it works" page only — and that page needs one italic framing line at the top so a
  non-technical reader doesn't think they're expected to run any of it themselves, e.g. *"This page goes deep on
  purpose — it's the proof the homepage summary is real. You don't need to follow all of it."*
- **Name/tagline test:** a non-technical reader has to get it instantly, zero context, "wow, that's my problem."
  State the outcome/benefit, never the mechanism. ("Never let a closed deal go cold," not "CRM-to-ops follow-up
  handoff via webhook.")
- **Lead each project's "problem" framing with the universal, emotionally relatable pain**, not the narrowest
  technical scenario. The narrow scenario is a good supporting bullet, never the headline.
- **Never invent a specific-sounding claim** — a stat, an exact count, a named behavior pattern — without it
  being genuinely sourced. If nothing well-sourced exists, use a general statement instead of a plausible-sounding
  invented one. A real, hedged, cited stat (labeled as a vendor/survey figure if that's what it is) beats a bare
  assertion of benefit, but a fake one is worse than no number at all.

## Visual

- **Real official brand logos only** for every integration/tool shown (e.g. via a permissively-licensed set like
  simple-icons) — never a hand-drawn fake logo, never a guessed brand color.
- **Show breadth across three logo tiers**, not one, where a project genuinely spans them: sources/triggers,
  alert channels (Slack/WhatsApp/email), and destinations (Sheets/Notion/Asana/Trello/CRM) — this lets different
  kinds of visitors recognize their own stack.
- **Trace ONE real flow end-to-end** instead of generic abstract numbered circles or disconnected logo rows:
  source logo → action/checkmark icon → alert-channel logo → destination logo, with arrows and a one-line caption
  under each stage. This reads clearer than either abstract steps alone or logos with no connecting story.
- A real, readable, sanitized screenshot of the actual automation can add supporting trust on a deep technical
  page — never as a homepage replacement for the diagram above (a dense node-canvas screenshot at page size is a
  readability failure).

## Honesty — do not soften any of these

- **Narada OS:** no paying customers. Say what was built; never imply distributor adoption.
- **Authorship:** never claim deep line-by-line hand-authorship of any codebase. Honest framing: "I directed the
  architecture and product decisions, Claude Code implemented it, I reviewed every output." Agents are how it
  was built, not something to hide, but also not the headline.
- **Straight Answer Agent:** the production source is intentionally not published (real proprietary software for
  a venture with no paying customers). This is a documentation/case-study piece, not a downloadable template —
  say "the architecture is proven, each build is custom," never "download and use this."
- **StoreCast:** built on a public retail dataset, not a live client's data. Any dollar figure is a *simulated
  projection* from a documented error-rate improvement in the repo's own feasibility report — say "a projected
  result on public data," never "saved a client $X."
- **No client names, no revenue figures, no claim of paying users anywhere on the site.** None exist yet.

## One pattern worth knowing before building any "status" or interactive state into the site

If the site ever shows or lets a visitor toggle a status (e.g. a project's "approved/reviewed" state in a demo),
ask: is this status a claim about an AI's output, or about something a human did in the real world? Those two
need opposite carry-over behavior when the underlying data changes — don't copy whichever rule was used last
without re-asking this per field. (Context: SnapTally's approval resets when re-extracted numbers change because
it's a claim about those specific numbers; RecapRelay's "done" mark never resets because it tracks real human
progress independent of the AI re-running.)
