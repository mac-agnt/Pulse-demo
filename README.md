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

## Local preview

```bash
python3 serve.py
```

Then open http://pulse.localhost:8080
