# Landmark Architectural Pulse demo

Frontend-only Pulse operations mockup for **Landmark Architectural** (Mark O'Rourke).

This branch is a client overlay of the Pulse-demo template. Do not merge it into the template default branch.

## Files

| File | What it is |
|---|---|
| `index.html` | Primary page (same content as the Glass mockup). Use this path for CDN loaders. |
| `Pulse v4 Glass.dc.html` | Same Landmark demo; this is the template's historical primary filename. |
| `support.js` | Demo runtime. |
| `AgentFace.dc.html` | Agent avatar component. |
| `vercel.json` | Serves `/` as the Glass page. |

## Local preview

```bash
python3 serve.py
```

Then open http://pulse.localhost:8080
