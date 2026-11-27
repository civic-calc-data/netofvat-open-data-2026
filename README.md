# Net of VAT Open Data (2026)

Open CSV datasets indexing HMRC's complete UK VAT Flat Rate Scheme percentages (all 54 sector rates, the 16.5% limited cost business override, effective net-sales percentages, and 2020–2022 temporary hospitality cuts) alongside 147 HMRC VAT rate categories across standard (20%), reduced (5%), zero-rated (0%), exempt, outside-scope, and mixed supplies.

All figures are transcribed and computed directly from official HMRC VAT notices and GOV.UK rate guidance. Interactive VAT and CIS calculators live at [netofvat.co.uk](https://netofvat.co.uk/).

## Datasets in this repository

| File | Coverage | Live report & calculator |
|---|---|---|
| [`data/uk-vat-flat-rate-scheme-percentages-2026.csv`](data/uk-vat-flat-rate-scheme-percentages-2026.csv) | 64 rows (55 current rules: 54 sectors + 16.5% limited cost business override, plus 9 historical 2020–2022 temporary cut periods): flat rate %, first-year -1% rate, and effective % of net sales | [VAT Flat Rate Scheme Report](https://netofvat.co.uk/reports/flat-rate-scheme-percentages/) / [Flat Rate Calculator](https://netofvat.co.uk/flat-rate-scheme/) |
| [`data/uk-vat-rates-by-category-2026.csv`](data/uk-vat-rates-by-category-2026.csv) | 147 HMRC VAT rate categories with section, group, item description, rate code, notes, VAT Notice reference, and GOV.UK source URL | [UK VAT Rates by Category Report](https://netofvat.co.uk/reports/uk-vat-rates-by-category/) / [VAT Rates Reference](https://netofvat.co.uk/vat-rates/) |

---

## 1. UK VAT Flat Rate Scheme Percentages (VAT Notice 733)

Key figures from [`data/uk-vat-flat-rate-scheme-percentages-2026.csv`](data/uk-vat-flat-rate-scheme-percentages-2026.csv):
- **55 current rows** (`current = true`): 54 business sectors plus the **16.5%** Limited Cost Business override (`15.5%` in year one, equal to **19.8%** of net VAT-exclusive sales).
- **Lowest current sector rate:** **4.0%** (3.0% first year, **4.8%** of net sales) for retailing food, confectionery, tobacco, newspapers or children's clothing.
- **Professional services examples:** accountancy or book-keeping at **14.5%** (17.4% of net sales); advertising at **11.0%** (13.2% of net sales).
- **9 historical rows** record HMRC's temporary 2020–2022 hospitality, catering and attractions VAT rate cuts.

---

## 2. UK VAT Rates Across 147 HMRC Categories

Breakdown of the **147 categories** in [`data/uk-vat-rates-by-category-2026.csv`](data/uk-vat-rates-by-category-2026.csv):

| Rate classification | Code | Categories |
|---|---|---:|
| Zero-rated (0%) | `0` | **69** |
| Exempt from VAT | `exempt` | **39** |
| Reduced rate (5%) | `5` | **21** |
| Standard rate (20%) | `20` | **12** |
| Outside the scope of UK VAT | `outside` | **4** |
| Mixed / split-rate items | `mixed` | **2** |

One row covers electricity from a public or workplace EV charging point: standard-rated at 20% from 1 November 2026, because it no longer counts as domestic use. Home charging on a household supply stays at the domestic rate.

---

## Primary Official Sources

- HMRC: [VAT Flat Rate Scheme (VAT Notice 733)](https://www.gov.uk/guidance/flat-rate-scheme-for-small-businesses-vat-notice-733--2) and [Flat rate percentages](https://www.gov.uk/vat-flat-rate-scheme/how-much-you-pay)
- HMRC: [VAT rates](https://www.gov.uk/vat-rates) and [Rates of VAT on different goods and services](https://www.gov.uk/guidance/rates-of-vat-on-different-goods-and-services)
- HMRC: [VAT Notice 700/1 supplement (thresholds)](https://www.gov.uk/government/publications/vat-notice-7001-should-i-be-registered-for-vat/vat-notice-7001-supplement--2)
- HMRC: [Construction Industry Scheme (CIS 340)](https://www.gov.uk/government/publications/construction-industry-scheme-cis-340/construction-industry-scheme-a-guide-for-contractors-and-subcontractors-cis-340)

## Interactive Calculators and Embeds

- UK VAT Calculator (add / remove 20% & 5%): https://netofvat.co.uk/
- Remove VAT Calculator: https://netofvat.co.uk/remove-vat/
- VAT Flat Rate Scheme Calculator: https://netofvat.co.uk/flat-rate-scheme/
- VAT Registration Threshold Checker (£90,000): https://netofvat.co.uk/vat-threshold/
- VAT Margin Calculator: https://netofvat.co.uk/vat-margin-calculator/
- UK CIS Deduction Calculator (20% / 30%): https://netofvat.co.uk/cis-calculator/
- Lightweight iframe embeds: `https://netofvat.co.uk/embed/vat/`, `https://netofvat.co.uk/embed/cis/`

## License and Citation

Licensed under [CC-BY-4.0](LICENSE). Contains public sector information licensed under the Open Government Licence v3.0. Citation metadata is in [`CITATION.cff`](CITATION.cff).

```text
Net of VAT (2026). Net of VAT Open Data 2026: UK VAT Flat Rate Scheme Percentages and 147 HMRC VAT Rate Categories [Dataset]. https://netofvat.co.uk/reports/ (CC-BY-4.0).
```
