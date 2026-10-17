# Amazon Sales Analysis — Excel

Analysis of **Amazon India (Amazon.in) fashion orders** in Excel: cleaning the raw order export, adding helper columns, and summarizing sales by category, status, fulfilment and region.

<!-- TODO (Ahmed): add 1–2 dashboard screenshots here, e.g. ![Dashboard](dashboard.png) -->

---

## Dataset

Order-level sales export: one row per order line.

| Field group | Columns |
|---|---|
| Order | Order ID, Date, Status, Courier Status, Qty, Amount, Currency |
| Product | Style, SKU, Category (Kurta, Set, Top, Western Dress…), Size, ASIN |
| Fulfilment | Fulfilment (Amazon / Merchant), Ship Service Level, Fulfilled By, Sales Channel |
| Customer location | Ship City, Ship State, Postal Code, Country |
| Other | Promotion IDs, B2B flag |

## What I did

1. **Data cleaning**: standardized dates and amounts, handled blank amounts and cancelled orders (Qty = 0)
2. **Helper columns** for analysis:
   - `Status Group`: groups the detailed order statuses (Shipped, Delivered, Cancelled, Returned…)
   - `Has Promo`: whether the order used a promotion
   - `Data Flag`: marks rows for review
   - `Month`: for time-based analysis
3. **Pivot tables** to summarize revenue and orders by category, status group, fulfilment type and state
4. **Dashboard** with KPIs and charts

## Questions answered

- Which product categories generate the most revenue?
- What share of orders are cancelled or returned, and does fulfilment type (Amazon vs. Merchant) affect it?
- Which states and cities drive the most sales?
- Do promotions increase order value?

## Tools

`Excel` · `Pivot Tables` · `XLOOKUP / INDEX-MATCH` · `Conditional Formatting` · `Charts`

## Files

The workbook is about 35 MB, which is too large to upload through GitHub's website, so it's hosted on Google Drive:
**[Download Amazon Sales.xlsx](PASTE-GOOGLE-DRIVE-LINK-HERE)**

---

**Ahmed Khaled** · Data Analyst · [LinkedIn](https://linkedin.com/in/ahmed-khaled-347711287) · [GitHub](https://github.com/ahmed-dataanalystt)
