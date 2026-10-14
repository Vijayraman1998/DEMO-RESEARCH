# Internal audit for large companies in India: core problems in tax compliance, TAM and SAM

*Research date: 14 Oct 2026. Scope: large Indian companies that must have an internal audit under Companies Act Sec 138. This replaces the consumer-ITR framing in `tax-filing-problems-and-market-size.md`.*

---

## 0. Who must have an internal audit (Sec 138 + Rule 13)

- **Every listed company.** No threshold applies.
- **Unlisted public companies** that meet any one of these in the preceding year: paid-up capital ≥ ₹50 cr, turnover ≥ ₹200 cr, borrowings > ₹100 cr, or deposits ≥ ₹25 cr.
- **Private companies** with turnover ≥ ₹200 cr or bank/FI borrowings > ₹100 cr.
- The internal auditor can be a CA, a cost accountant or another professional chosen by the board, but **not the statutory auditor**.

Source: [TaxGuru](https://taxguru.in/company-law/internal-audit-applicability-private-companies-india.html), [LegalWiz](https://www.legalwiz.in/blog/internal-audit-rules-for-private-companies)

---

## 1. Core problems in tax filing and compliance at large companies

**In one line:** The tax department now checks **100% of a company's data automatically and continuously** (GSTR-1 vs 3B vs 2B, e-invoices, AIS/TDS). Internal audit at most large companies is still **sample-based, periodic (usually quarterly) and done in Excel**. Mismatches are found by the department first and arrive as notices and demands, not as internal audit findings.

| # | Problem | Detail | Evidence |
|---|---------|--------|----------|
| 1 | **GST reconciliation at scale** | A large company has many state GSTINs and thousands of vendors. GSTR-1, 3B and 2B must reconcile every month. ITC is allowed only if it appears in GSTR-2B (Rule 36(4)), so a supplier's non-filing becomes *your* tax cost. Scrutiny notices for GSTR-1 vs 3B gaps are generated automatically. | [Masters India](https://www.mastersindia.co/blog/gst-red-flags-2025-compliance-guide/), [Free Press Journal](https://www.freepressjournal.in/amp/mumbai/top-indian-corporations-mncs-across-banking-insurance-fmcg-and-telecom-sectors-file-appeals-against-gst-demand-notices) |
| 2 | **Notice and demand overload** | DGGI issued **20,000+ notices worth over ₹80,000 cr** for FY 2017-18 to FY 2021-22. Single companies get very large demands: UltraTech about ₹782 cr, LIC about ₹806 cr, Dabur about ₹320 cr. | [Taxo](https://taxo.online/latest-news/23-08-2024-over-rs-80000-crore-worth-gst-notices-issued-for-assessment-year-2018-22/), [CemNet](https://www.cemnet.com/News/story/180505/ultratech-cement-hit-with-inr7-82bn-tax-demand-notice.html), [Taxscan](https://www.taxscan.in/?p=460422) |
| 3 | **Root cause is internal data mismatch** | Per ClearTax's CFO survey, **80% of enterprises got at least one GST notice in FY25**, traced to sales and accounts modules showing different numbers for the same invoices. The same report says **80% of notices were avoidable** and about **₹5.76 lakh cr** is locked in indirect-tax litigation. This is a vendor survey, so treat it as indicative. | [Clear CFO survey](https://www.cleartax.com/in/india-cfo-survey-report) |
| 4 | **Mandatory audit trail (edit log)** | Since FY 2023-24, accounting software must log every change and the log cannot be switched off (Rule 3(1)). Statutory auditors must report on it (Rule 11(g)). Problems include ERP migration, huge log volumes, admin-privilege control, and the risk of a modified audit opinion. | [ICAI CA Journal](https://cajournal.icai.org/article-details/audit-trail-requirements-responsibilities), [Taxmann](https://www.taxmann.com/post/?p=47236), [Deloitte](https://www2.deloitte.com/content/dam/Deloitte/in/Documents/risk/in-ra-mandatory-accounting-audit-trail-feature.pdf) |
| 5 | **Transition to the Income Tax Act 2025** (in force from 1 Apr 2026) | Sections and forms are renumbered (for example, Form 16 becomes Form 130), and reassessment windows change (4 years 3 months, or 6 years 3 months for high-value cases). TDS logic in ERPs, tax-audit checklists and IA programmes all need re-mapping. | [TaxGuru](https://taxguru.in/?p=1039324), [Outlook Business](https://www.outlookbusiness.com/news/new-income-tax-act-effective-april-2026-early-itr-rollout-in-january-to-aid-smooth-transition) |
| 6 | **Internal audit is under-equipped** | In the IIA India–Protiviti 2025 survey of 225 CAEs, only about **16%** felt highly prepared for emerging risks (AI, cyber, automation), and more than half lacked subject-matter experts. Data is scattered across ERPs and departments. | [IIA–Protiviti via Industrial Automation India](https://www.industrialautomationindia.in/news/chief-audit-executives-ai-cybersecurity-risks-iia-protiviti-survey-2025), [Protiviti](https://www.protiviti.com/in-en/survey/top-risks-chief-audit-executives-2025) |
| 7 | **Low AI and analytics adoption** | Globally, only **4%** of internal audit teams report significant progress with GenAI (AuditBoard). Continuous monitoring is still rare. | [CFOtech / AuditBoard](https://cfotech.in/story/auditboard-study-reveals-internal-audit-struggles-in-2025) |
| 8 | **Fragmented tax footprint** | GST, TDS/TCS, corporate tax, transfer pricing and customs are each handled by different teams and tools, with no single view of tax risk for the audit committee. | Synthesised from the sources above |

**Product angle:** "Continuous tax-compliance audit". Pull ERP, GSTN, e-invoice and TDS data. Reconcile the **full population** of transactions, not a sample. Flag ITC at risk from non-filing vendors and audit-trail exceptions **before** the department does. Produce internal audit working papers and an audit-committee dashboard.

---

## 2. TAM and SAM

No public report sizes India's internal audit market on its own, so these are **bottom-up estimates**. Every assumption is listed so you can change it.

### Data points

| Data point | Value | Source |
|------------|-------|--------|
| Listed companies | NSE about 2,600–2,700, BSE about 5,600–5,700. Roughly **5,500–6,000 unique** after removing overlap. | [Motilal Oswal](https://www.motilaloswal.com/blog-details/how-many-companies-are-listed-in-the-indian-stock-market/20955), [Aditya Birla Capital](https://www.adityabirlacapital.com/abc-of-money/how-many-companies-are-listed-in-nse-and-bse) |
| Taxpayers with turnover > ₹500 cr | "More than 50,000" eligible for e-invoicing phase 1 (Oct 2020). This counts PAN-level GST entities, not only companies. | [ClearTax News](https://news.cleartax.in/?p=5471) |
| Companies filing corporate tax returns | About 10.7 lakh (FY24). Fewer than 1,000 have income above ₹500 cr. | [Business Standard](https://www.business-standard.com/amp/companies/news/in-tax-records-the-marked-rise-of-companies-reporting-zero-income-124071900401_1.html) |
| Newly mandated internal audit companies | About 12,000 more since 2023. Vendor estimate. | [Dataintelo](https://dataintelo.com/report/global-internal-audit-outsourcing-market) |
| Big 4 India revenue (FY24) | About ₹38,800 cr combined: EY ₹13,400 cr, Deloitte ₹10,000 cr, PwC ₹9,200 cr, KPMG about ₹6,000 cr. FY25 expected above ₹45,000 cr. Covers all service lines. | [The Finance Story](https://thefinancestory.com/big-4-india-ey-deloitte-pwc-kpmg-eyes-revenue-₹45000-cr) |
| India eGRC software | $458.5M (2024), forecast $930M by 2029 (15.2% CAGR) | [MarketsandMarkets](https://www.marketsandmarkets.com/Market-Reports/geography/enterprise-governance-risk-compliance-market/India) |
| Global internal audit services | About $74.8B (2025), 5.9% CAGR | [Research and Markets](https://www.researchandmarkets.com/report/internal-audit) |
| Internal audit sourcing mix | Roughly half of large companies outsource or co-source, and half run in-house. CA firms are the preferred outside provider. | [ICMAI study](https://www.icmai.in/upload/AdvStudies/Executive-Summary-IA.pdf) |

### Universe of companies under Sec 138 (assumption)

| Tier | Definition | No. of companies (estimate) |
|------|-----------|--------------------------|
| T1, Enterprise | Turnover ≥ ₹1,000 cr (large listed, MNC subsidiaries, PSUs, banks/NBFCs) | ~5,000 |
| T2, Upper mid | ₹500–1,000 cr | ~10,000 |
| T3, Mandated mid | ₹200–500 cr, or borrowings > ₹100 cr, or small listed companies | ~25,000 |
| **Total** | | **~40,000** (plausible range 30k–60k) |

### TAM: total internal audit spend (in-house teams, outsourced firms and tools)

| Tier | Companies | Annual internal audit spend each | TAM |
|------|-----------|----------------------------------|-----|
| T1 | 5,000 | ₹3 cr (in-house team of 10–30 plus Big 4 / CA co-source) | ₹15,000 cr |
| T2 | 10,000 | ₹50 lakh | ₹5,000 cr |
| T3 | 25,000 | ₹15 lakh | ₹3,750 cr |
| **TAM** | **~40,000** | | **≈ ₹24,000 cr (~$2.7B per year)** |

**Sanity checks:**
- India is about 3% of the $75B global internal audit services market, or about $2.2B.
- Big 4 India earns about ₹39k–45k cr across *all* service lines, and risk advisory is a slice of that.

**Tech-addressable TAM:** assume 15–20% of internal audit spend can move to software and automation. That gives **≈ ₹3,600–4,800 cr (~$400–550M)**, which matches the India eGRC estimate of about $460M (₹4,000 cr).

### SAM: an AI / continuous-audit product for T1 + T2 companies, focused on finance and tax controls

| Tier | Companies | Annual contract value (ACV) | SAM |
|------|-----------|-----------------------------|-----|
| T1 | 5,000 | ₹40 lakh | ₹2,000 cr |
| T2 | 10,000 | ₹12 lakh | ₹1,200 cr |
| **SAM** | **15,000** | | **≈ ₹3,200 cr (~$360M)** |

**Narrower SAM (tax-compliance internal audit module only):** GST/TDS reconciliation, ITC-at-risk tracking and audit-trail checks, at an ACV of ₹15 lakh (T1) and ₹5 lakh (T2). That gives **≈ ₹1,250 cr (~$140M)**.

### SOM (reference)

Winning **100–200 enterprise logos at about ₹25 lakh ACV** within 3–5 years gives **₹25–50 cr ARR**. That is about 1–1.5% of SAM.

### Caveats

- No official count of companies by turnover band was found. The tier counts are the biggest assumption. Verify with MCA master data, CMIE Prowess, or a Lok Sabha / CBDT reply.
- Spend per company is an assumption. Validate it with 5–10 CAE or CFO interviews, or with internal audit fee disclosures in annual reports.
- Several problem-side figures (80% notices, ₹5.76 lakh cr litigation) come from vendor reports.
- The ₹ to $ conversion uses about ₹88 per $1.
