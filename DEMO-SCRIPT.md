# Healthcare Abroad — Pulse demo script

## Start and stop

1. Run `python3 serve.py` from this directory. The demo opens at **http://pulse.localhost:8080**.
2. Press Ctrl+C in the terminal when done.

No internet needed; React and the fonts are bundled in `vendor/`.
This is a **proposed operating model with fictional data only**. A "Demo data" indicator stays visible at the bottom of every screen.

## Questions Helios answers

Type these on Home, or click the matching suggestion. The wording can change; Helios listens for the key words.

| Ask | Helios shows | Key words |
|---|---|---|
| Who is travelling next week? | Two patients: Catherine Walsh (Madrid) and Seán Kelly (Pamplona) | travel, travelling, next week, depart |
| Which cases are blocked? | Mary Byrne — missing GP referral, 4 days overdue | block, stuck, missing |
| What needs my approval? | Thomas O'Brien booking at Quirón Barcelona | approv, waiting, need |

## Mary Byrne connected story

Click the play button (▶) at the bottom of the sidebar to open scenario controls.

12 steps walk through Mary Byrne's hip-treatment journey:

1. Referral arrives in Referrals & Paperwork
2. Document Assistant extracts details, finds missing item
3. Referral Coordinator prepares targeted follow-up
4. Completed file ready for hospital review
5. Staff select confirmed option from Care Network
6. Proposed travel plan in Travel & Transport
7. Hospital changes procedure date
8. Pulse identifies affected arrangements
9. Coordinator approves; pending confirmations visible
10. Claims & Funding assembles evidence pack
11. Mismatched payment amount flagged for review
12. Activity records full sequence with approvals

Use **Reset demo** to return to the start.

## Pages to show

- **Home** — Helios chat, action inbox, upcoming travel, numbers
- **Patients** — list and journey board views, click a patient for profile
- **Referrals & Paperwork** — outstanding requests, statuses
- **Care Network** — hospital cards with categories and case counts
- **Travel & Transport** — trip planner, stats
- **Claims & Funding** — HSE claims tracker, funding applications
- **Dashboard** — pipeline, revenue (illustrative), treatment payments, workload
- **Agents** — 6 agents with conversation threads
- **Work** — patient-related tasks
- **Records** — contacts directory
- **Activity** — event log
- **Settings** — deployment, staff, permissions, integrations (simulated)

## Watch out for

- Prices, availability and financial figures are **illustrative**.
- Simulated emails, bookings, lender applications and HSE submissions are **labelled simulated**.
- Administrative readiness is separate from clinical clearance — a complete document checklist does not imply medical clearance.
- Never diagnose, interpret scans, or invent clinical information.
- Hospital fees owed to Healthcare Abroad are separate from money owed to patients by the HSE.
