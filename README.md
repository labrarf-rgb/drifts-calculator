# DRIFTS Calculator — The Cost of Inaction

An interactive calculator that puts a dollar figure on the hidden cost of tolerating known problems in product & delivery teams. Inaction feels free — it isn't. Configure your team, move the levers across the six DRIFTS categories, and watch the cost (and the shape of your team's profile) update live.

**[▶ Live demo](https://labrarf-rgb.github.io/drifts-calculator/)**

## The six categories

- **D — Decision Drag** — decisions that stall or never get made
- **R — Rework from Unclear Requirements** — the breakdown between product and engineering
- **I — Invalid Assumptions Shipped** — building what nobody validated
- **F — Fragmented Priorities** — mid-sprint pivots and a roadmap nobody trusts
- **T — Technical Debt & Incidents** — unplanned work that steals sprint capacity
- **S — Slow Feedback Loops** — the cost of learning slowly, or not at all

## How it works

- **One self-contained file.** `index.html` — no build step, no dependencies, no backend. Vanilla HTML/CSS/JS with an inline SVG radar.
- **A real cost model, not a questionnaire.** Five categories (D, R, I, F, T) draw from a single team-capacity pool that's proportionally normalized so the internal-capacity total can never exceed the team's fully-loaded payroll. S (market time lost to slow feedback) is reported separately, outside that ceiling.
- **Raw-dominant ledger.** Each category shows its raw cost prominently; making one problem worse never visibly shrinks another.
- **Transparent assumptions.** Every number driving the model is exposed and editable in the Settings panel — tune it to your team or trust the stage-based defaults.
- **Light/dark mode**, responsive, and embeddable via iframe.

All figures are estimates, presented as ranges, and fully tunable.

## Run locally

Open `index.html` in any browser, or serve the folder:

```bash
python3 -m http.server 4173
# → http://localhost:4173
```

## Embed

```html
<iframe src="https://labrarf-rgb.github.io/drifts-calculator/" title="DRIFTS Calculator" allowfullscreen></iframe>
```

---

Built by [Ray Labra](https://www.labrarf.com).
