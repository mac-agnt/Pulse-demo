# Pulse demo template

Template for a customer-facing Pulse operations mockup. This repo is a GitHub
template (`is_template`). It ships the real `Pulse v4 Glass.dc.html` fixture —
Kilbride Group, a plumbing and heating merchant — which you replace for each
customer. Do not swap that file for a lookalike.

## Create a customer demo

1. **Create a new repository from this template** (GitHub → *Use this template*).
   Name it `{Customer}-Pulse-demo` in `mac-agnt`. Examples:
   `Landmark-Architectural-Pulse-demo`, `Acme-Builders-Pulse-demo`.
2. **Rebrand** the fixture in the new repo. Change company, people, places,
   numbers, vocabulary and the accent so the mock reads as that business.
3. **Remove Kilbride.** Search the mockup for Kilbride, Kilbride Group,
   Martin Kilbride, Ballincollig, Mallow, `kilbridegroup.ie` and related Cork
   merchant copy. None of it should survive a customer demo.
4. **Deploy** the customer repo to the Vercel team **agnt-ie-crms-25**
   (`team_ykvh6KOTqmxAB0Eei4xF38Gb`). Link the GitHub repo, keep `/` rewriting
   to `Pulse v4 Glass.dc.html` via `vercel.json`, and turn off Vercel
   Authentication / SSO if the demo needs a public URL.

This template keeps Kilbride on purpose. Customer repos created from it must
not.

## What this is

A frontend mock. No backend, no live integrations. Helios answers a small set
of questions from fixture data and never executes write or external tools — it
proposes and waits for a confirmation bound to hashed arguments.

## Local

```bash
python3 serve.py
```

Then open http://pulse.localhost:8080 (or double-click `Start Demo.command` on
macOS). React and fonts are in `vendor/`, so the page runs offline.

## Layout

| File | Role |
|---|---|
| `Pulse v4 Glass.dc.html` | The app. Keep this file; rebrand its data. |
| `AgentFace.dc.html` | Agent avatars. Leave it. |
| `support.js` | Generated runtime. Do not edit. |
| `vercel.json` | Clean `/` rewrite onto the Glass mockup. |
| `DEMO-SCRIPT.md` | Questions Helios can actually answer. Update this when you rebrand. |
| `serve.py` | Local server. |

## Product rules the mock must still show

- Helios never executes write/external tools; it proposes and waits.
- The action inbox answers three things per item: what happened, why it
  matters, what I can do.
- Metrics, nav, pages and Helios tools come from the registry — module
  contributions stay labelled as the module's.
