# Starting wedge: tax audit for the tech industry (India)

*Date: 14 Oct 2026. The founders want to start with **tax audit**, focused on the **tech industry** (IT services, ITES/BPM, GCCs, SaaS/product companies), and later expand into full internal audit. Items marked † are from general knowledge and were not confirmed by a source found in this research. All sizing is a bottom-up estimate.*

---

## 1. Positioning: internal tax audit *before* the external audit

**Decision (14 Oct 2026):** the startup starts with an **internal tax audit**, a pre-audit or readiness review run *by or for the company* **before** the external audits. It finds and fixes tax errors, prepares clean schedules and evidence, and reduces adverse remarks and disallowances when the external CA does the statutory audit and the Sec 44AB tax audit (Form 3CD).

| | **Our product: internal tax audit (pre-audit)** | External tax audit (Sec 44AB / Form 3CD) and statutory audit |
|---|---|---|
| Who runs it | The company's tax, finance or internal audit team, using our software | Independent external CA (must sign) |
| When | Continuous or quarterly, plus an intensive year-end pre-audit (about Jan–Jul) | After year end. The 3CD report is due about 30 Sep, with transfer-pricing cases later † |
| Goal | Find and fix issues *before* the auditor or department finds them | Independent opinion and reporting |
| Buyer | **CFO / Head of Tax / Head of Internal Audit** | — (the external CA receives our "audit-ready pack") |

**Value to the customer:**
- **Fewer disallowances.** Examples: 43B(h) MSME payments, and 40(a)(i)/(ia) when TDS is not deducted on payments, including foreign ones † (both are reported in 3CD).
- **Fewer adverse remarks** in Form 3CD and the auditor's report, and fewer later notices.
- **GST refunds and ITC protected**: export refunds, cross-charge, reverse charge.
- **Faster, cheaper external audit.** The CA gets reconciled schedules and evidence instead of raw ledgers.

**The external CA's role:** a *recipient* of the audit-ready pack and a possible referral partner. The CA is not the buyer.

### Annual cycle for an Indian tech company (FY Apr–Mar) †

| Period | Internal tax audit activity (our product) | External event |
|--------|-------------------------------------------|----------------|
| Monthly / quarterly | GST (GSTR-1/3B/2B, export LUT and refunds, cross-charge, reverse charge), TDS returns, Sec 195 / 15CA-CB foreign payments, intercompany invoicing | GST and TDS filings |
| Jan–Mar | Pre-close review: provisions, TDS on year-end accruals, MSME dues (43B(h)), related-party and TP data | — |
| Apr–Jul | **Year-end pre-audit**: draft 3CD schedules, exception list, fix and document, then hand the audit-ready pack to the CA | Statutory audit |
| Aug–Oct | Support CA queries, TP documentation, track open items | Sec 44AB tax audit report, TP report (Form 3CEB), ITR |
| Ongoing | Notice tracker, root-cause fixes | Assessments and notices |

Existing tools (KDK, Computax, BDO's tax-audit tool, AssureAI) mostly help the **external CA fill in 3CD**. Few, if any, offer a **company-side, continuous internal tax audit** built for tech-industry tax issues. That gap is the opening. ([BDO](https://www.bdo.in/en-gb/services/bdo-digital/technology-products-and-solutions/compliance/tax-audit), [KDK](https://www.kdksoftware.com/blog/simplifying-gst-compliance-reporting-in-form-3cd-tax-audit-report-with-express-gst/), [Computax](https://computaxonline.com/product/audit-report-software), [ICAI AI use cases](https://ai.icai.org/usecases_details.php?id=286))

---

## 2. Why tech is a good first sector for tax audit

- **No physical audit needed.** Tech companies have no plants or inventory, so all evidence is digital. This fits the founders' constraint of no physical audits.
- **Heavy, cross-border tax complexity.** Export of services, related-party transactions with foreign parents, multi-state GST registrations, and large payroll with ESOPs (details below).
- **Large, growing segment.**
  - About 1,700 GCCs (FY24, NASSCOM via government) and 2,117 GCC parents with 3,728 centres (FY26, Zinnov–NASSCOM). Revenue grew from $64.6B (FY24) to $98.4B. ([IANS](https://ianslive.in/over-1700-gccs-are-in-operation-in-india-minister--20250806142159), [Storyboard18](https://www.storyboard18.com/amp/how-it-works/indias-gcc-sector-hits-64-6-billion-in-fy24-grows-9-8-annually-meity-85690.htm), [businessofgcc](https://www.businessofgcc.com/insights/analysis/gcc-market-size-2026))
  - The tech industry overall had revenue of about $283–297B in FY25 and about 5.8M employees. ([NASSCOM](https://nasscom.in/sites/default/files/media_pdf/Nasscom%20SR%20Press%20release.pdf), [ETV Bharat](https://www.etvbharat.com/en/business/india-fy26-tech-revenues-hit-usd-315-billion-enn26022404879))
- **Buyers are SaaS-friendly** and use cloud ERPs (NetSuite, SAP, Oracle, Zoho †), so data integration is easier than with Tally-heavy manufacturers.

**Trade-off:** tech companies have a smaller full internal audit universe (see the sector scoring in `go-to-market-recommendation.md`). That is fine for a *tax-audit wedge*. The expansion path is wider internal audit in tech, then pharma and auto.

---

## 3. Tax pain points specific to tech companies

| # | Pain point | What goes wrong | Source |
|---|-----------|-----------------|--------|
| 1 | **GST refunds on export of services** | Exporters build up unused ITC and must claim refunds (Rule 89(4) formula). Officers have denied refunds by treating IT and ITES services as "intermediary" services, which leads to long litigation (for example Genpact, P&H HC). Interest applies if a refund is delayed beyond 60 days. | [Conventus Law](https://conventuslaw.com/report/india-refund-of-unutilised-itc-cannot-be-denied-to-supplier-of-subcontracted-services/), [CAM blog](https://tax.cyrilamarchandblogs.com/2022/11/refund-of-unutilised-itc-cannot-be-denied-to-supplier-of-subcontracted-services/), [Regitom](https://www.regitom.com/gst-refund-export-of-services-india), [HNA](https://hnallp.com/assets/articles/Refund-Mechanism-for-Export-of-Services-under-GST.pdf) |
| 2 | **GST cross-charge between offices in different states** | Each GSTIN is a "distinct person". Head-office costs (HR, IT, leadership salaries) must be cross-charged or distributed through ISD. Circular 199/2023 helped, but employee-cost recharges remain grey, and notices are being issued. | [ClearTax](https://cleartax.in/s/all-about-gst-on-cross-charge-transactions), [HNA](https://hnallp.com/assets/articles/701ab-cross-charge-in-gst-july-23.pdf), [Entrackr](https://entrackr.com/?p=70502) |
| 3 | **Transfer pricing for captives and GCCs** | Disputes over the markup, cost base (pass-through costs), ESOP recharges, and overdue receivables from the parent being treated as loans. The safe-harbour threshold was widened substantially in Budget 2026 (sources differ on the exact figure). | [BCAJ](https://bcajonline.org/journal/transfer-pricing-for-captive-service-providers-in-india-disputes-resolution-and-policy-considerations/), [Mondaq](https://www.mondaq.com/india/tax-authorities/1748156/budget-2026-a-structural-reset-of-indias-transfer-pricing-framework), [Roedl](https://www.roedl.com/insights/newsletter-indien/2025-04/transfer-pricing-news) |
| 4 | **TDS on foreign payments (Sec 195, Form 15CA/CB)** † | Payments for cloud, SaaS subscriptions, licences and group recharges abroad. Questions of whether something is royalty or fees for technical services, DTAA rates, and grossing-up. | — |
| 5 | **Reverse charge on imported services** † | GST due on imported software and services, and on cross-border services from related parties | — |
| 6 | **Payroll TDS and ESOP perquisites** † | Large workforces, ESOP perquisite valuation and deferral for eligible startups, and multi-state professional tax | — |
| 7 | **SEZ / STPI unit compliance** † | Sec 10AA deductions, SEZ GST zero-rating, and Softex forms | — |
| 8 | **Form 3CD clause load** | 40+ clauses, location-wise reporting, and 43B(h) disallowance of MSME vendor payments (match vendor master to payments) | [Moneylife](https://moneylife.in/article/how-this-new-cbdt-rule-will-create-problems-for-your-tax-audit/38430.html), [ICAI AI](https://ai.icai.org/usecases_details.php?id=286) |
| 9 | **Income Tax Act 2025 transition** (from 1 Apr 2026) | Section and form renumbering, so tax-audit and TDS mappings need updating | [TaxGuru](https://taxguru.in/?p=1039324) |

---

## 4. Sizing the wedge: tax audit in tech

### Segments (assumptions)

| Segment | Entities | Basis |
|---------|----------|-------|
| GCCs (Indian entities of global firms) | ~2,000 | 1,700–2,117 GCC parents (sourced) |
| Indian IT / ITES / ER&D services companies, ₹200–5,000 cr | ~1,000 | **Assumption** † |
| SaaS / product / funded tech companies with revenue ≥ ₹100 cr | ~500 | **Assumption** † |
| *Excluded:* the top ~20 IT firms (TCS, Infosys and others) | — | Big 4 / in-house locked |
| **Core universe** | **~3,500** | |

Smaller tech companies (thousands, above the 44AB threshold) are reachable only through CA firms.

### TAM / SAM / SOM

| Layer | Calculation | Value |
|-------|-------------|-------|
| **TAM (services spend)** | 3,500 × about ₹40 lakh per year on tax audit, TP study, GST reviews and refund work, and internal tax reviews (assumption) | **≈ ₹1,400 cr (~$160M)** |
| **TAM (software)** | 3,500 × ₹12 lakh ACV (assumption) | **≈ ₹420 cr (~$48M)** |
| **SAM** | Company-side internal tax audit for GCCs + mid IT/ITES services (~3,000 × ₹10 lakh). The CA-firm channel is no longer counted, because the buyer is the company. | **≈ ₹300 cr (~$34M)** |
| **SOM (about 3 years)** | 60–100 direct customers × ₹10 lakh | **≈ ₹6–10 cr ARR** |

**What this means:** the tech tax-audit wedge is **small but focused**, about 11–12% of the full internal audit SAM (≈ ₹2,600 cr in `internal-audit-tam-sam.md`). Use it to win the first 50–100 customers and build the data engine, then expand:

1. Full internal audit for the same tech customers (payroll, procurement, revenue/contracts, ITGC)
2. Tax audit for pharma and auto
3. Full internal audit in pharma and auto

---

## 5. Who to target first in tech

### a) GCCs (best fit: complex tax, budget, compliance-driven, fully digital)

- **Where:** Bengaluru, Hyderabad, Pune, Chennai and NCR host most GCCs.
- **Who to contact:** India finance controller or CFO, India tax head, and the head of internal audit or SOX at the parent.
- **Examples by category** †: global banks and financial services (the GS, JPMorgan, Wells Fargo-type centres), retail and consumer (Walmart Global Tech, Target, Lowe's), and engineering and pharma GCCs. Build the actual list from the NASSCOM/Zinnov GCC directory or LinkedIn.

### b) Mid-size listed Indian IT / ITES companies

From general knowledge †; verify revenue and the current tax/internal audit set-up on Screener.in and in annual reports:

| Company | City | Approx. revenue band |
|---------|------|----------------------|
| Mastek | Ahmedabad / Mumbai | ₹3,000–4,000 cr |
| Happiest Minds | Bengaluru | ₹2,000–2,500 cr |
| Intellect Design Arena | Chennai | ₹2,500–3,000 cr |
| Newgen Software | Delhi NCR | ₹1,500 cr |
| Tanla Platforms | Hyderabad | ₹4,000 cr |
| eClerx | Mumbai | ₹3,000–3,500 cr |
| Datamatics | Mumbai | ₹1,500–2,000 cr |
| R Systems | Noida | ₹1,500–2,000 cr |
| Nucleus Software | Noida | ₹800 cr |
| Saksoft | Chennai | ₹800–1,000 cr |
| Sasken Technologies | Bengaluru | ₹800 cr |
| Ramco Systems | Chennai | ₹500–600 cr |
| Kellton Tech | Hyderabad | ₹1,000 cr |
| Latent View Analytics | Chennai | ₹800 cr |
| Affle | Gurugram | ₹2,000–2,500 cr |
| Zaggle | Hyderabad | ₹1,000–1,500 cr |
| Tata Elxsi | Bengaluru | ₹3,500–4,000 cr |
| Zensar Technologies | Pune | ₹5,000–5,500 cr (upper edge) |
| Birlasoft | Pune | ₹5,000–5,500 cr (upper edge) |

### c) SaaS and product companies (Indian entities of US-domiciled startups)

These have heavy TP, GST export refund and 195 TDS exposure. Examples by type †: Freshworks, Chargebee, BrowserStack, Postman, Druva, Darwinbox-type companies. Verify Indian entity revenue on Tracxn or MCA.

### d) External CA / tax firms: referral partners, not buyers

- They receive the audit-ready pack and benefit from shorter audits, so they can refer clients.
- They are not the target buyer.

### First 20 discovery calls

- 8 GCC finance or tax heads
- 6 mid-size IT company CFOs or tax heads
- 3 SaaS company finance controllers
- 3 heads of internal audit at tech companies (to test the internal-audit buyer)

---

## 6. MVP scope for "Internal Tax Audit (pre-audit) for Tech"

1. **Connectors:** NetSuite, SAP, Oracle, Zoho Books, Tally †; GST portal data; TDS (TRACES) returns
2. **Pre-audit of Form 3CD items:** clause-wise schedules (43B(h) MSME, 40(a)(i)/(ia) TDS disallowances, GST reporting, related parties), exception flags with fix workflow, and an audit-ready pack for the external CA
3. **GST export module:** LUT tracking, Rule 89(4) refund computation, flags for intermediary-risk contracts, refund claim pack
4. **Cross-charge module:** allocation of head-office costs to state GSTINs, ISD distribution, documentation
5. **Foreign payments module:** Sec 195 / 15CA-CB checks, DTAA rate validation, RCM on imported services
6. **TP support:** intercompany invoice and receivable reconciliation, cost-base and markup checks, safe-harbour eligibility test
7. **Outputs:** working papers, a tax-risk dashboard for the CFO and Audit Committee, and a notice tracker
