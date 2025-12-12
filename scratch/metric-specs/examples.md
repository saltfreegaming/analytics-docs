Metric: Division Performance Index (DPI)

Intent: Primary signal for “skill mismatch” against division peers.
Grain: player x rolling window (e.g., last 20 matches or last 60 days)

Definition (example)

Compute a weighted performance score per match (see “Signal Specs”)

DPI = player_avg_score − division_peer_avg_score (normalized as z-score)

Minimum data needed

match roster + division-at-time-of-match + win/loss
Better data

hero, role, K/D/A, GPM/XPM, warding, building damage (any subset helps)

Edge cases

New division assignment: exclude first N matches in new division or label as “provisional”

Small sample size: require N matches for stability

Acceptance test

A known stable player in Division B should have DPI near 0 (±1)

Known high-skill player placed low should show DPI consistently > +2

Metric: Abrupt Shift Score (ASS)

Intent: Detect step changes consistent with account change/sharing/boosting.
Definition

Compare last 10 matches vs previous 20 matches for key stats and win impact.

ASS = max standardized delta across metrics (winrate, DPI, hero pool entropy)

Guardrails

Ignore if role changed and matches are few; require persistence beyond 1 session.