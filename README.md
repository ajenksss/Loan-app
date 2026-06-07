# Owner Financing Loan Calculator

A single-file tool for sizing up a property deal before you negotiate owner
financing. Enter the price and your numbers, and it shows you a grid of monthly
payments across different loan terms and interest rates — so you walk into the
conversation knowing your true limit and which terms actually work for you.

## How to use

1. Open **`index.html`** in any web browser (double-click it, or drag it into a
   browser tab). No installation, no internet connection required.
2. Fill in the deal inputs:
   - **Property / Deal name** — appears on the printed PDF.
   - **Purchase prices to compare** — comma-separated (e.g. `180000, 200000,
     220000`). Use this to see how different negotiated prices play out.
   - **Your max monthly payment** — your true ceiling. Any payment at or under
     this is highlighted **green**; anything over is **red**.
   - **Down payments to compare** — comma-separated, in dollars or as a
     percentage of price (toggle the `$` / `%` button).
   - **Loan terms to compare** — years, comma-separated (e.g. `10, 15, 20, 30`).
   - **Interest rates to compare** — percent, comma-separated (e.g. `4, 5, 6`).
     Include `0` if you're floating a no-interest offer.
   - **Balloon payment** (optional) — check the box if you want payments
     amortized over the term but the remaining balance due as a lump sum after
     a set number of years. Common in owner-financed deals.
3. Click **Calculate**.
4. Click **Save as PDF / Print**, then choose "Save as PDF" as the
   destination. Take it into the negotiation.

## What it shows

- **Loan Summary** — the prices, down payments, max payment, and structure.
- **Monthly Payment by Term & Rate** — the core comparison grids, one for each
  purchase price and down payment combination, color-coded against your budget.
- **Your True Limit** — working backwards from your max monthly payment, the
  highest purchase price you can afford at each down payment, term, and rate.
- **Total Cost Detail** — total interest and total paid over each scenario for
  a chosen price and down payment (or, for balloon deals, how much you'd pay in
  before the balloon and the lump sum still owed).
- **Seller's Perspective** — total interest the owner earns and the total
  they'd receive (down payment plus every payment) for each scenario. Hand
  this to the seller to show why financing beats a cash sale.
- **Side-by-Side Comparison** — pick any two term/rate scenarios and compare
  them line by line (monthly payment, total interest, total paid, plus balloon
  figures), including the dollar difference between them.
- **Amortization Schedule** — a full payoff breakdown for one chosen scenario,
  either a yearly summary or month by month, showing principal, interest,
  cumulative interest, and remaining balance. If a balloon applies, the
  schedule ends with the lump-sum payoff row.

## Notes

- All payment figures are **principal & interest only**. Property taxes,
  homeowner's insurance, and HOA dues are not included — budget for those
  separately.
- Math is standard amortization. Always confirm final figures with the seller
  and, for a real deal, an attorney or title company.
