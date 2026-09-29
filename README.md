# Simple Browser BMI Calculator

## Confirmed decisions

- **Units:** Metric (kg / cm) and imperial (lb / in) with a toggle
- **Look:** Coastal teal + coral, sky-to-mint gradient
- **Name:** BMI Check
- **Delivery:** Single [`index.html`](index.html) file (open in browser; no build step)

## Approach

Create a self-contained web app in the empty workspace: one [`index.html`](index.html) with embedded CSS and JavaScript. Double-click or open the file in a browser—no server or npm required.

**Formula:** `BMI = weight_kg / (height_m)²` (convert imperial to metric before calculating).

## UI & design

One focused composition (not a dashboard):

- **BMI Check** as the hero brand signal
- Short line of support text
- Height + weight inputs, unit toggle, Calculate button
- Result: BMI number + category with a distinct color

**Visual direction:** bright coastal health look—teal primary, coral accent, soft sky-to-mint gradient background. Expressive Google Fonts (Outfit + Fraunces). Avoid purple themes, cream/terracotta, flat single-color backgrounds, and emoji clutter.

**Category colors (result feedback):**

| BMI | Category | Accent |
|-----|----------|--------|
| &lt; 18.5 | Underweight | cool blue |
| 18.5–24.9 | Normal | green |
| 25–29.9 | Overweight | amber |
| ≥ 30 | Obese | coral/red |

Light motion: soft fade-in on result, brief scale on the BMI number when it updates.

## Behavior

1. User picks units, enters height and weight
2. Validate positive numbers; show a short inline message if invalid
3. On Calculate (and optionally on Enter), compute BMI to 1 decimal place
4. Show category label and tint the result area to match

## Files

- [`index.html`](index.html) — markup, styles, and script in one file for easy sharing and opening

## Out of scope

No backend, accounts, charts history, or mobile app wrappers—browser page only.
