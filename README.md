# Poulton Consultancy – Financial Dashboard (Static)

This repository hosts a single-page dashboard you can deploy via GitHub Pages.

## Files
- `index.html` – the full dashboard (drop-in).
- `costs_template.csv` – header-only template for bulk expense imports.
- `invoices_template.csv` – header-only template for bulk invoice imports.

## Deploy (Org: Poulton-Consultancy)
1. Create a repo under the org, e.g. `finance-dashboard`.
2. Upload the three files above into the repo **root**.
3. In **Settings → Pages**, set:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` (or `master`) / `/root`
4. The site will publish at `https://poulton-consultancy.github.io/finance-dashboard/` (adjust for your repo name).
5. To update, replace `index.html` or upload new CSVs and refresh your browser cache.

## CSV Formats
### Costs (`costs_template.csv`)
```
Date,Description,Category,Amount,Currency,Tax Deductible,Notes
2025-08-31,Office Rent,Office,4500,AED,Yes,Business Bay
```
- `Category`: Licensing | Office | Marketing | Travel | Technology | Professional | Training | Insurance | Utilities | Salary | Other
- `Currency`: AED or USD
- `Tax Deductible`: Yes / No

### Invoices (`invoices_template.csv`)
```
Invoice #,Date,Client,Amount,Currency,Status,Paid Amount
0000042,2025-08-30,Nature Adventure LLC,8000,AED,Paid,8000
```
- `Status`: Unpaid | Paid | Partially Paid

---

> Tip: If you enable Pages on `main`, make sure the repo has *public* visibility or an appropriate Pages plan.