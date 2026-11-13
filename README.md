
# Waves Salon - Business Performance Analysis

**Educational case study · Google Sheets · Data Analytics**

## Overview

Waves is a curly-hair salon featured in an educational analytics project. The task was to examine manually maintained transaction records and identify opportunities to improve business performance.

The analysis covered three areas: revenue and operating expenses, promotional campaigns, and demand for services and retail products.

## Tools and methods

- Google Sheets: data preparation, formulas, pivot tables, and charts (also exported to Excel).
- Data cleaning: checked missing values, duplicates, inconsistent categories, and formatting; prepared calculated fields.
- Functions: `IF`, `OR`, `MONTH`, `VLOOKUP`, `IFNA`, `COUNTIFS`, and `SUMIFS`.
- Metrics: monthly revenue and expenses, sales volume, discount amounts, average transaction value, and product contribution after direct purchase costs.

### Technical approach

1. Standardized manually entered records and added fields for transaction classification and monthly reporting.
2. Matched promotional codes with campaign information using lookup formulas.
3. Aggregated transactions by month and category using conditional formulas and pivot tables.
4. Built three reporting views: financial performance, promotional campaigns, and product/service demand.

**Illustrative formulas** (generic examples, not copied from the underlying dataset):

```excel
=IFNA(VLOOKUP(C2, $H$2:$J$10, 3, FALSE), "")
=SUMIFS($D$2:$D$100, $B$2:$B$100, "Service A", $E$2:$E$100, 3)
```

These demonstrate matching promotion information and summing revenue by category and month. Source data and internal dataset paths are not included.

## Key findings

**Financial performance.** Revenue remained relatively stable across the six complete months, with no clear sustained growth trend. Services accounted for the majority of revenue. Payroll and marketing expenses dropped markedly in May without a similarly large decline in revenue; the reason requires investigation. Some consumable purchases also increased later in the period.

**Promotions.** Campaigns differed in redemption frequency, discount amounts, and average transaction value. Telegram posts and VK advertising were associated with comparatively high total discounts and lower average transaction values. However, discounts alone do not establish campaign profitability: individual customer histories and campaign-level marketing costs were unavailable.

**Services and retail.** Services were the main revenue driver. Hair gel sales increased in the later complete months, suggesting an assortment idea worth testing rather than a proven long-term trend. A shampoo-and-conditioner bundle generated greater retail revenue and contribution than shampoo alone, although fewer bundles were sold.

## Business recommendations

1. Investigate May's cost changes before treating the reduction in payroll and marketing spend as a sustainable efficiency gain.
2. Track customers over time, including new versus returning visitors, to assess acquisition and retention.
3. Review campaign economics using marketing budgets and customer outcomes, not just coupon redemptions and discounts.
4. Check consumable purchasing trends for changes in suppliers, quantities, or unit prices.
5. Test complementary retail products, including different hair gels and care bundles, using customer feedback and small experiments.

## Limitations and data availability

- The extract includes a partial final month; monthly trend conclusions are based on complete months.
- Transaction records do not establish unique-customer acquisition or marketing return on investment.
- Retail contribution after direct product costs is not the salon's net profit after all operating expenses.
- The original dataset and working spreadsheet arenot publicly shared due to confidentiality and redistribution restrictions. Conclusions are presented at a permitted, high level; no source URLs or internal file paths are disclosed.

## Project context

This is an independent educational case study completed during data analytics training, not a paid client engagement.
