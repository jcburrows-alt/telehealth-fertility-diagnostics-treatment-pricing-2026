---
license: cc-by-4.0
tags:
- healthcare
- telehealth
- fertility
- reproductive-medicine
- letrozole
- clomid
- amh
- semen-analysis
- health-economics
language:
- en
size_categories:
- n<1K
task_categories:
- tabular-classification
- tabular-regression
- other
pretty_name: "US Telehealth Couples Fertility Diagnostics (AMH, Semen Analysis) & Oral Ovulation Induction (Letrozole, Clomid) Cost Dataset — November 2026"
configs:
- config_name: default
  data_files:
  - split: train
    path: pricing.csv
- config_name: couples_fertility_diagnostics
  data_files:
  - split: train
    path: subsets/couples-fertility-diagnostics.csv
- config_name: ovulation_induction_cycles
  data_files:
  - split: train
    path: subsets/ovulation-induction-cycles.csv
---

# US Telehealth Couples Fertility Diagnostics (AMH, Semen Analysis) & Oral Ovulation Induction (Letrozole, Clomid) Cost Dataset — November 2026

An open-access, machine-readable health economics dataset (**64 verified plan rows across 20 US telehealth platforms, CLIA reference laboratories, and brick-and-mortar Reproductive Endocrinology & Infertility [REI] clinics**) auditing out-of-pocket costs for couples fertility testing and first-line oral ovulation induction as of **November 10, 2026**:

1. **`couples_fertility_diagnostics` (`subsets/couples-fertility-diagnostics.csv` — 36 Rows):** Female Anti-Müllerian Hormone (`AMH` [`Q419081`](https://www.wikidata.org/wiki/Q419081)), Cycle Day 3 FSH/LH/Estradiol venipuncture panels, pelvic ultrasound imaging, and CLIA-certified at-home male semen analysis kits.
2. **`ovulation_induction_cycles` (`subsets/ovulation-induction-cycles.csv` — 28 Rows):** First-line oral ovulation induction cycles using `Letrozole` ([`Q417965`](https://www.wikidata.org/wiki/Q417965)) or `Clomiphene Citrate` (`Clomid`, [`Q416908`](https://www.wikidata.org/wiki/Q416908)) plus luteal `Micronized Progesterone` ([`Q422466`](https://www.wikidata.org/wiki/Q422466)) vs. brick-and-mortar REI clinic timed-intercourse, IUI, and IVF benchmarks.

---

## Multi-Config Parquet Splits & Associated Research Hubs

| Config Name | File Path | Rows | Associated First-Party Research Hub |
|---|---|---|---|
| `default` | `pricing.csv` | 64 | [2026 Online Fertility Testing, Letrozole & Clomid Cost Report](https://getskinnyonline.com/blog/2026-online-fertility-testing-letrozole-clomid-cost-report) |
| `couples_fertility_diagnostics` | `subsets/couples-fertility-diagnostics.csv` | 36 | [Couples Fertility Program Hub](https://getskinnyonline.com/fertility), [AMH Ovarian Reserve Guide](https://getskinnyonline.com/fertility/amh-test), & [At-Home Semen Analysis Guide](https://getskinnyonline.com/fertility/at-home-semen-analysis) |
| `ovulation_induction_cycles` | `subsets/ovulation-induction-cycles.csv` | 28 | [Online Fertility Medications Guide](https://getskinnyonline.com/fertility/fertility-medication) & [Letrozole vs. Clomid Clinical Comparison](https://getskinnyonline.com/fertility/letrozole-vs-clomid) |

---

## License & Citation

Licensed under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/).

```bibtex
@dataset{gso_fertility_diagnostics_treatment_2026,
  author       = {{Get Skinny Online Health Economics Research Group}},
  title        = {{US Telehealth Couples Fertility Diagnostics & Oral Ovulation Induction Cost Dataset — November 2026}},
  year         = {2026},
  month        = nov,
  version      = {2026.11.1},
  publisher    = {Hugging Face / Get Skinny Online},
  url          = {https://getskinnyonline.com/datasets/telehealth-fertility-diagnostics-treatment-pricing-2026/}
}
```
