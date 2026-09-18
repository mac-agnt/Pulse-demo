# Active Life Pharmacy Pulse demo

Frontend-only Pulse operations mockup for **Active Life Pharmacy** (Pat Durkin / MacDaithi · ACMR).

This branch is a client overlay of the Pulse-demo template. Do not merge it into the template default branch.

## Files

| File | What it is |
|---|---|
| `index.html` | Primary page (same content as the Glass mockup). Use this path for CDN loaders. |
| `Pulse v4 Glass.dc.html` | Same Active Life Pharmacy demo; the template's historical primary filename. |
| `support.js` | Demo runtime. |
| `AgentFace.dc.html` | Agent avatar component. |
| `vercel.json` | Serves `/` as `index.html` with `cleanUrls`. |

## Local preview

```bash
python3 serve.py
```

Then open http://pulse.localhost:8080

## CDN

jsDelivr branch snapshot:

- https://cdn.jsdelivr.net/gh/mac-agnt/Pulse-demo@active-life-pharmacy/index.html
- https://cdn.jsdelivr.net/gh/mac-agnt/Pulse-demo@active-life-pharmacy/support.js
