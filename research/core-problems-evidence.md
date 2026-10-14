# Core problems in tax compliance and internal tax audit: evidence from surveys and data

*Date: 14 Oct 2026. Context: an AI startup offering **internal tax audit (pre-audit before the external audit)** to **tech companies** (GCCs, IT/ITES, SaaS) in India.*

**Honest caveat:** no survey was found that covers *exactly* "internal tax audit at Indian tech companies". The evidence below comes from the closest sources:
- Indian government data
- Industry-body surveys (NASSCOM–KPMG)
- Big 4 and vendor surveys (EY, ClearTax, Grant Thornton Bharat, Thomson Reuters, TeamLease RegTech)

Vendor surveys are marked as such. Treat their numbers as indicative.

---

## The core problem in one line

**Tax teams cannot see and fix their own tax risk before the tax department or the external auditor finds it.** Data is scattered across systems, compliance volume is huge, the rules keep changing, and checks are manual. Avoidable mismatches therefore turn into notices, blocked refunds, disallowances and years of litigation.

---

## Problem 1: avoidable notices caused by your own data mismatches

| Evidence | Source |
|----------|--------|
| **80% of GST notices in FY25 were avoidable.** The leading cause is that GSTR-1 and GSTR-3B are filed from **different internal data sets**, which triggers automatic mismatch notices. | ClearTax *State of Tax Assurance 2026* (500 companies, 100+ CFO interviews; **vendor**) ([ClearTax](https://www.cleartax.com/in/india-cfo-survey-report)) |
| **About ₹3 cr of ITC left unclaimed per enterprise per year** on average | Same (vendor) |
| **91%** of tax and finance leaders say their data sits in **too many silos**, and **80%** say a lack of AI-ready data is their biggest barrier | EY 2025 Tax & Finance Operations Survey (1,600 executives, 30 jurisdictions, global) ([EY](https://www.ey.com/en_gl/insights/tax/tfo-survey)) |

**Implication:** reconciling the company's *own* data before filing, and before the auditor arrives, is the highest-value fix.

## Problem 2: disputes are huge, slow and rising, with little visibility

| Evidence | Source |
|----------|--------|
| **₹48.18 lakh cr** in outstanding income-tax arrears (22.9M demand entries) as of 1 Apr 2025 | Govt data via [TaxHeal](https://www.taxheal.com/?p=112177) |
| **5.39 lakh appeals** pending at the first appellate level (CIT(A)) in FY25. High Court disputes **doubled in value** from ₹2.75 to ₹5.65 lakh cr in four years. | Rajya Sabha reply via [LiveLaw](https://www.livelawbiz.com/tax-cases/income-tax-disputes-high-court-pendency-doubled-rajya-sabha-data-313114), [Outlook Money](https://www.outlookmoney.com/tax/taxpayers-in-limbo-over-5-lakh-appeals-pending-before-cit-a-tax-practitioners-call-for-early-disposal) |
| **₹5.76 lakh cr** locked in indirect-tax (GST) litigation | ClearTax (vendor) |
| **90%** of tax leaders expect more disputes in the next 3 years. **Fewer than half** feel highly prepared. **Only 9%** have full visibility over their disputes. Only 31% are very satisfied with how they manage disputes. | EY 2025 Tax Risk & Controversy Survey (1,934 executives, 48 jurisdictions, global) ([EY Tax News](https://taxnews.ey.com/news/2025-2477-global-tax-policy-and-controversy-watch-december-2025-edition), [Bloomberg Tax](https://news.bloombergtax.com/international-trade/tax-controversy-is-becoming-an-always-on-challenge-for-business)) |

**Implication:** prevention is cheap and litigation is expensive. Companies also need a single view of open notices and disputes.

## Problem 3: tech-specific tax issues (GCCs, IT/ITES)

| Evidence | Source |
|----------|--------|
| **Transfer pricing is the #1 regulatory priority for 81% of GCC executives.** SEZ/STPI rules come next (67%), followed by labour laws (60%), DPDPA (49%) and FEMA (37%). | NASSCOM–KPMG GCC report (75+ GCCs, May 2024) ([Outlook Business](https://www.outlookbusiness.com/news/regulatory-compliance-key-concern-for-gccs-in-india-report), [BusinessWorld](https://businessworld.in/article/regulatory-compliance-vital-for-india%E2%80%99s-gccs-transfer-pricing-tops-concerns-521466)) |
| A GCC handles about **2,051 compliance filings a year** under **537 legal obligations** across 18 regulators (labour, tax, environment) | TeamLease RegTech study (**vendor**) ([Outlook Business](https://www.outlookbusiness.com/news/over-2000-filings-a-year-the-compliance-cost-of-indias-gcc-boom), [CAalley](https://caalley.com/news-updates/indian-news/gccs-in-india-drive-10-4-mn-jobs-30-higher-pay-2-000-legal-obligations)) |
| GST on **head-office ↔ overseas-branch** transactions is a **"persistent area of litigation"** for IT/ITES exporters, causing ITC reversals and blocked refunds. NASSCOM raised this, plus R&D/testing exports, before the **57th GST Council (Oct 2026)**, which **recommended relaxing both**. | NASSCOM via [KNN India](https://knnindia.co.in/news/newsdetails/economy/nasscom-seeks-gst-clarity-on-overseas-branch-services-rd-work-ahead-of-council-meet), [Daily Pioneer](https://dailypioneer.com/news/nasscom-welcomes-gst-council-move-on-services-exports), [NASSCOM community](https://community.nasscom.in/communities/public-policy/gstat-and-tech-economy) |
| The **"intermediary"** classification has led to refund rejections and show-cause notices for IT/ITES | [Conventus Law](https://conventuslaw.com/report/india-refund-of-unutilised-itc-cannot-be-denied-to-supplier-of-subcontracted-services/), [NASSCOM](https://community.nasscom.in/communities/policy-advocacy/gst-advocacy-on-early-resolution-of-issues-around-intermediary-services-for-it-ites-sector.html) |
| GCC audit hot-spots: **foreign payments and withholding tax**, intermediary or testing services under GST, and **permanent-establishment risk** from India-based leadership | KPMG *GCCs in India: key tax insights* (Sep 2025) ([KPMG](https://kpmg.com/in/en/insights/2025/09/gccs-in-india-key-tax-insights.html)), [CFO India](https://www.cfo-india.in/?p=26182) |
| GST cross-charge between a company's own state offices (HR, IT, CEO costs) is being questioned through notices | [Entrackr](https://entrackr.com/?p=70502), [HNA](https://hnallp.com/assets/articles/701ab-cross-charge-in-gst-july-23.pdf) |

**Implication:** the riskiest tax areas for tech companies are transfer pricing, GST export refunds and cross-charge, foreign-payment TDS and PE risk. They are complex and rule-heavy, which makes them a good fit for an AI pre-audit.

## Problem 4: constant rule changes

- **Income Tax Act 2025** took effect on 1 Apr 2026: sections and forms are renumbered ([TaxGuru](https://taxguru.in/?p=1039324)).
- **Transfer-pricing safe harbour** was reset in Budget 2026 ([Mondaq](https://www.mondaq.com/india/tax-authorities/1748156/budget-2026-a-structural-reset-of-indias-transfer-pricing-framework)).
- **GST Council (Oct 2026)** changed export rules for overseas branches and R&D/testing services (above).
- The **GST Appellate Tribunal** started in Sep 2025 (NASSCOM).

**Implication:** every change has to be re-mapped in checklists, ERP tax logic and audit programmes. Manual teams lag behind. A rules engine that is kept up to date is valuable.

## Problem 5: finance and tax teams are stretched and under-tooled

| Evidence | Source |
|----------|--------|
| **55.7%** of Indian CFOs say they are only "somewhat prepared" for upcoming challenges. **48%** still spend significant time on operational oversight. **75%** expect to spend more time on AI and automation, and 71% will raise tech spend. | Grant Thornton Bharat *India Finance Leaders Barometer* (149 CFOs, Aug 2026) ([Board Stewardship](https://boardstewardship.com/?p=52956), [Analytics Insight](https://www.analyticsinsight.net/news/india-cfos-turn-to-ai-85-report-stronger-business-outlook)) |
| **44%** of CFOs and tax leaders (including 70 from large Indian companies) cite a **lack of skilled talent** as a major barrier to GenAI in tax | EY GenAI in Tax survey (Nov 2024) ([EY India](https://www.ey.com/en_in/newsroom/2024/11/94-percent-of-cfo-s-and-tax-leaders-expect-gen-ai-as-a-game-changer-for-tax-functions)) |
| **Chronic talent shortage**. **57%** of tax professionals call AI their top tech investment for 2026, up from 35%. **Low-value work** is the top barrier to profitability. | Thomson Reuters *2026 State of Tax Professionals* (~600 respondents, global) ([TR Institute](https://www.thomsonreuters.com/en/institute/reports/state-of-tax-professionals-report-2026)) |
| More than half of Indian chief audit executives lack subject-matter experts for technical risks. Only about 16% are highly prepared. | IIA India–Protiviti 2025 ([Industrial Automation India](https://www.industrialautomationindia.in/news/chief-audit-executives-ai-cybersecurity-risks-iia-protiviti-survey-2025)) |

**Implication:** buyers want automation and accept AI. The constraint is people and data, not willingness to buy.

---

## Ranked problem list for the startup (judgement, based on the evidence above)

| Rank | Problem | Evidence strength | Product answer |
|------|---------|-------------------|----------------|
| 1 | **Internal data mismatches cause avoidable notices and lost ITC** | Strong (vendor survey plus EY silo data) | Continuous reconciliation: books vs GSTR-1/3B/2B, TDS returns vs ledgers |
| 2 | **Transfer pricing and intercompany risk at GCCs** | Strong (NASSCOM–KPMG, 81%) | Intercompany reconciliation, cost-base and markup checks, safe-harbour test |
| 3 | **GST export refunds, HO–BO and cross-charge** | Strong (NASSCOM advocacy, court cases, Council action) | Refund computation and evidence pack, cross-charge and ISD engine, tracking of rule changes |
| 4 | **Rising disputes with no visibility** | Strong (government data, EY 9% visibility) | Notice and dispute tracker linked to root cause |
| 5 | **Compliance volume and changing rules** | Medium (vendor filing count, rule-change record) | Rules engine updated for IT Act 2025, GST Council changes and safe harbour |
| 6 | **Talent and manual work** | Strong (EY, TR, GT Bharat, IIA) | AI-drafted working papers and an audit-ready pack for the external CA |

## Validate in discovery calls

1. How many tax notices did you get last year, and what share came from internal mismatches?
2. How much ITC or export refund is blocked right now?
3. How many person-days does the year-end tax audit preparation (3CD schedules) take?
4. Which tax area worries you most: TP, GST export, cross-charge, foreign TDS or PE?
5. What tools do you use today, and who owns the budget?
