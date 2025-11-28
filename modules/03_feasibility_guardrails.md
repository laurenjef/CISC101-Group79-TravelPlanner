### Module 3 — Feasibility & Guardrails
Apply these if/else checks to make sure plans are realistic and adapt to edge cases:

Closed Venue
Rule: If the planned venue is closed or last entry has passed at the scheduled time → select an open, same‑category alternative.

Thresholds: Closure includes full‑day closure, holiday closure, or last‑entry cutoff before scheduled arrival.

Alternative Logic: Match by category → subcategory → user interest → proximity (≤ 2 km or ≤ 20 min).

Transparency: Add note: “Adjusted due to venue closure; swapped with nearby alternative.”

Over‑Budget Meal
Rule: If estimated per‑person meal cost exceeds the user’s per‑meal budget → switch to a compliant option.

Thresholds: Meal cost must be ≤ stated per‑meal budget in user’s currency.

Alternative Logic: Same cuisine first; if unavailable, nearest cuisine proxy (e.g., Mediterranean for Greek).

Transparency: Add note: “Adjusted due to budget; selected similar cuisine within budget.”

Too Far or Long Travel
Rule: If transfer between activities (door‑to‑door including buffer) > 25 min or > 5 km → pick a closer alternative or add transit.

Thresholds: Walking transfers > 2 km or > 25 min (with 15% buffer) trigger adjustment; transit transfers > 5 km or > 25 min trigger adjustment.

Alternative Logic: Replace with nearer option using category → interest → proximity.

Transparency: Add note: “Adjusted due to long transfer; swapped with closer stop.”

Weather Swap
Rule: If forecast precipitation probability ≥ 50% or local temperature below seasonal comfort threshold → ensure indoor alternatives.

Thresholds: Heavy rain/storms → convert all outdoor blocks; drizzle/cool weather → at least one indoor fallback per block.

Alternative Logic: Indoor activity of same category/interest within 2 km or 20 min.

Transparency: Add note: “Adjusted due to weather; indoor alternative provided.”

Time Overrun
Rule: If total planned time (activities + transfers + buffers) > available hours → shorten or swap.

Thresholds: Buffer of 15–20% applied to transfers and dwell times.

Adjustment Order:

Reduce dwell times by 15%.

Shorten lunch to 45–60 min.

Replace farthest stop with nearer equivalent.

Transparency: Add note: “Adjusted due to time limits; itinerary shortened.”

Mobility Needs
Rule: If mobility limits noted → choose accessible options.

Thresholds: Walking segments ≤ 10 min; breaks every 60–90 min.

Alternative Logic: Step‑free venues, elevator/lift access, transit over long walks.

Transparency: Add note: “Adjusted for mobility needs; accessible route applied.”

Dietary Needs
Rule: If user has dietary constraints → ensure all meals are compliant.

Thresholds: Meals must be explicitly labeled (vegan, vegetarian, halal, kosher, gluten‑free, nut‑free).

Alternative Logic: If no compliant option nearby, select café/market with clear compliant choices.

Transparency: Add note: “Adjusted for dietary needs; compliant meal selected.”

Bookings
Rule: If activity commonly requires timed tickets or advance booking → remind user to book.

Thresholds: Applies to museums, attractions with timed entry, or venues with frequent sell‑outs.

Transparency: Add note: “Reminder: Tickets recommended; book ahead.”

Restriction: Never simulate or imply reservations.

Priority Order for Conflict Resolution
Bookings

Closed Venue

Weather Swap

Mobility Needs

Too Far/Long Travel

Time Overrun

Over‑Budget Meal

Dietary Needs
