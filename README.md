# Healthcare IV Pulse demo

Frontend-only Pulse operations mockup for **Healthcare** (community IV / OPAT), greeting **Audrey Weston**.

This is not Healthcare Abroad. This branch is a client overlay of the Pulse-demo template. Do not merge it into the template default branch.

## Files

| File | What it is |
|---|---|
| `index.html` | Primary page (rebranded Glass, support inlined). |
| `Pulse v4 Glass.dc.html` | Same Healthcare IV demo; kept for loaders that expect this filename. |
| `AgentFace.dc.html` | Agent avatar component. |
| `vercel.json` | Serves every unmatched path as `index.html`. |

Branding in `index.html`: **Audrey Weston** present, **Healthcare** present, **Kilbride** absent, **Healthcare Abroad** absent.

## Local preview

```bash
python3 serve.py
```

Then open http://pulse.localhost:8080

## Vercel

Preferred production URL: **https://healthcare-iv-pulse.vercel.app**

That hostname is already assigned to project `healthcare-iv-pulse` on team **agnt-ie-crms-25** (`team_ykvh6KOTqmxAB0Eei4xF38Gb`). This overlay could not create a production deployment there (403: no production-deploy permission on that existing project). Do not merge this branch into `main`.

Publish from a Vercel login that owns AGNTie CRMS25:

```bash
git checkout healthcare-iv-pulse
npx vercel link --scope agnt-ie-crms-25 --yes --project healthcare-iv-pulse
npx vercel deploy --prod --scope agnt-ie-crms-25
```

Set the project's production branch to `healthcare-iv-pulse` if the project is git-connected.

### Interim public URL

Until the AGNTie project is published, a bootstrap that loads this branch's HTML is live at:

**https://aw-healthcare-iv.vercel.app**
