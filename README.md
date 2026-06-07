# Property Deal Structurer

A single-file tool for structuring a real estate deal and selling it to the
other side. It has two tabs:

1. **Deal Structurer** — frame an offer the seller can't ignore. Enter a
   property and the seller's numbers, and it turns your offer into a plain-English
   pitch built around *their* gain and *their* cash flow. Saves your deals in the
   browser so you stop re-entering everything.
2. **Payment Calculator** — the original owner-financing calculator: payment
   grids across terms and rates, your true price limit, total-cost detail, the
   seller's interest earned, side-by-side comparison, and a full amortization
   schedule.

Open **`index.html`** in any browser (double-click it, or drag it into a tab).
No installation and no internet connection required. Switch between the two tabs
at the top.

---

## Tab 1 — Deal Structurer

The idea: instead of arguing over price, show the seller what your offer *means*
to them — how far above their basis it is, and how many months of their own cash
flow that represents, handed over in one check with none of the work.

### Saving deals

Deals are stored in your browser (localStorage), so they persist between visits
on the same device and browser.

- **+ New deal** — clear the form to start fresh.
- **Save deal** — store the current property; it appears in the *Saved Deals*
  list, where you can **Open** or **Delete** it.
- **Export all (backup)** — download every saved deal as a JSON file.
- **Import backup** — load deals from a JSON backup (e.g. to move them to
  another computer). Importing merges with what you already have.

> Because storage is per-browser, deals saved on one device won't automatically
> appear on another. Use Export/Import to move them.

### Property & Seller inputs

- **Property / address** — shows on the pitch; also generates quick lookup
  links to Zillow, Redfin, county records, and sale history so you can grab a
  value when it's worth it.
- **What the seller paid** — their basis (cost).
- **When they bought it** *(optional)* — used to show how long they've held it.
- **Estimated value today** *(optional, manual)* — leave blank to skip; the
  pitch adapts either way.
- **Seller's monthly cash flow** — their net, after expenses. This is the
  number the whole pitch is built around.
- **Gross monthly rent** *(optional)* — for your own reference.
- **Notes** — condition, motivation, anything to remember.

### Your Offer

- **Offer price(s) to compare** — one or several, comma-separated.
- **Pitch style** — toggle between:
  - **Cash / lump-sum** — you buy out their equity. The pitch leads with the
    premium over their basis and converts it to *months of cash flow*.
  - **Owner-finance** — they carry the note. Enter down payment, term, and
    rate (and optionally a balloon). The pitch compares the monthly check they'd
    collect against their current cash flow, plus total interest earned.

### What you get

- **Deal Snapshot** — basis, value today, equity, cash flow (monthly and
  annual), and how long they've owned it.
- **What Each Offer Means to the Seller** — a table: for each offer price, the
  premium over basis, how many months/years of cash flow that equals, how it
  compares to today's value, and (in finance mode) the monthly check vs. their
  current cash flow.
- **The Pitch** — ready-to-say paragraphs built around a chosen offer. Use
  **Copy pitch text** to grab it, or **Save pitch as PDF / Print** for a
  one-pager to hand across the table.

---

## Tab 2 — Payment Calculator

The original owner-financing calculator, unchanged. Fill in the deal inputs and
click **Calculate**:

- **Property / Deal name** — appears on the printed PDF.
- **Purchase prices to compare** — comma-separated (e.g. `180000, 200000,
  220000`).
- **Your max monthly payment** — your true ceiling. Payments at or under this
  are highlighted **green**; anything over is **red**.
- **Down payments to compare** — comma-separated, in dollars or as a percentage
  of price (toggle the `$` / `%` button).
- **Loan terms to compare** — years, comma-separated (e.g. `10, 15, 20, 30`).
- **Interest rates to compare** — percent, comma-separated (e.g. `4, 5, 6`).
  Include `0` for a no-interest offer.
- **Balloon payment** *(optional)* — payments amortized over the term, with the
  remaining balance due as a lump sum after a set number of years.

It then shows the Loan Summary, the Monthly Payment grids, your True Limit (max
affordable price), Total Cost Detail, the Seller's Perspective (interest
earned), a Side-by-Side Comparison, and a full Amortization Schedule. Use **Save
as PDF / Print** to take it into the negotiation.

---

## Notes

- All payment figures are **principal & interest only**. Property taxes,
  homeowner's insurance, and HOA dues are not included — budget for those
  separately.
- Cash-flow figures use whatever you enter as the seller's net; the tool does
  not estimate expenses for you.
- Math is standard amortization. Always confirm final figures with the seller
  and, for a real deal, an attorney or title company.
