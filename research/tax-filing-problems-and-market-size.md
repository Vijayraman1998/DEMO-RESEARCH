# Tax filing in India: core problems, TAM and SAM

*Research date: 14 Oct 2026. Scope: India. Covers individual income tax returns (ITR) first, and GST compliance for small businesses second.*

---

## 1. Core problems in tax filing today

**In one line:** Submitting the return is no longer the hard part, because the portal and pre-filled forms handle that. The hard part is **reconciliation**. The taxpayer's numbers have to match what the department already holds (AIS, Form 26AS, Form 16, GSTR-2B). Any mismatch leads to a notice, a defective return or a refund hold. On top of that, the rules are complex enough that people pay a CA for help.

### Individual taxpayers (ITR)

| # | Problem | What happens | Evidence |
|---|---------|--------------|----------|
| 1 | **Data mismatch (AIS / 26AS / Form 16 vs return)** | The department cross-matches every return against AIS, 26AS, TDS, bank and mutual-fund data. If you file before AIS is fully updated, or forget an interest or dividend line, you get a defective notice under Sec 139(9), a revised return, or a held refund. | [efiletax](https://www.efiletax.in/blog/income-tax-portal-issues-ay-2025-26-5-common-itr-filing-problems/), [TaxBuddy](https://www.taxbuddy.com/blog/why-your-income-tax-refund-is-delayed-in-2025-and-how-to-fix-it) |
| 2 | **Refund delays and processing backlog** | About 63 lakh AY 2025-26 returns were still pending. Under the CBDT "nudge" campaign, processing paused until mismatches were corrected. Refunds also stall when the bank account isn't pre-validated. | [Angel One](https://www.angelone.in/news/taxation/over-63-lakh-itrs-pending-in-ay-2025-26-why-refunds-are-delayed) |
| 3 | **Late forms and utilities, shifting deadlines** | AY 2025-26 utilities arrived about 3 months late. The deadline moved from 31 Jul to 15 Sep because of ITR form revisions. | [Business Standard](https://www.business-standard.com/finance/personal-finance/itr-2-itr-3-delay-decoded-changes-challenges-and-what-s-next-125062500777_1.html), [IANS](https://ianslive.in/over-6-crore-itrs-filed-so-far-for-ay-2025-26-income-tax-department--20250914173421) |
| 4 | **Portal glitches near deadlines** | Server crashes, session timeouts and AIS/26AS mismatches led professional bodies to ask CBDT to extend deadlines. In a LocalCircles survey, the portal was the #1 pain point (up to 38% of respondents). | [CAalley](https://www.caalley.com/news-updates/indian-news/extend-itr-and-tax-audit-deadlines-due-to-tax-portal-glitch-data-mismatch-in-ais-and-form-26as-new-icai-format-says-cctax), [StudyCafe](https://studycafe.in/itr-filing-2023-24-49-taxpayers-still-left-to-file-itrs-technical-issues-with-it-portal-become-top-reason-for-delay-332267.html) |
| 5 | **Transition to the new Income Tax Act 2025** (in force from 1 Apr 2026) | Forms are renumbered (for example, Form 16 becomes Form 130, and 15G/15H merge into Form 121). Old-Act ITR forms are still used for AY 2026-27, with new forms expected later. Expect confusion and a spike in queries. | [Outlook Business](https://www.outlookbusiness.com/news/new-income-tax-act-effective-april-2026-early-itr-rollout-in-january-to-aid-smooth-transition), [TaxGuru](https://taxguru.in/?p=1039324), [Outlook Money](https://www.outlookmoney.com/amp/story/tax/itr-forms-under-new-income-tax-act-to-be-notified-prior-to-fy28-govt) |
| 6 | **Complexity drives people to pay for help** | Capital gains (rate changes, grandfathering), F&O, crypto, multiple Form 16s, foreign assets and the old-vs-new regime choice all push filers to a CA. CA-assisted plans cost about ₹1,300 for salary income and ₹3,000–4,000+ for capital gains or business income. | [ClearTax pricing](https://cleartax.in/meta/Pricing) |
| 7 | **Post-filing notices** | Most tools focus on "file and forget". Understanding and answering notices (139(9), 143(1) adjustments, mismatch nudges) is still manual and stressful. | Synthesised from the sources above |
| 8 | **Low coverage** | Only **6.68%** of India's population filed an ITR in FY24, so a large first-time-filer pool still lacks tax literacy. | [Business Standard](https://www.business-standard.com/amp/finance/news/only-6-68-of-population-filed-income-tax-return-in-fy24-govt-tells-house-124121700768_1.html) |

### Businesses (GST)

- **GSTR-1, GSTR-3B and GSTR-2B don't reconcile.** The portal auto-flags the gaps, and Rule 88C / DRC-01B notices are generated automatically. ([Masters India](https://www.mastersindia.co/blog/gst-red-flags-2025-compliance-guide/))
- **Input tax credit (ITC) depends on your supplier filing.** Under Rule 36(4), only ITC that appears in GSTR-2B can be claimed. ([TaxGuru](https://taxguru.in/?p=1045082))
- **Mismatches are common.** In ClearTax's CFO survey, **80% of enterprises received at least one GST notice in FY25**, caused by sales and accounts systems showing different figures. This is a vendor survey, so treat it as indicative. ([Clear CFO survey](https://www.cleartax.com/in/india-cfo-survey-report))
- **The annual return is often filed wrong.** GSTR-9 is often filed incorrectly or skipped. ([Kanakkupillai](https://www.kanakkupillai.com/learn/top-gst-mistakes-small-businesses-make-in-india/))

**Takeaway for a product:** the opportunity is not "another filing form". It is **continuous reconciliation plus notice handling**: pull AIS, 26AS and broker data, flag mismatches before filing, then track and answer notices after filing.

---

## 2. TAM and SAM

No public report sizes India's *tax filing services* market on its own, so the numbers below are **bottom-up estimates**. Every assumption is listed so you can change it.

### Input data

| Input | Value | Source |
|-------|-------|--------|
| ITRs filed per year | ~7.3 crore by 16 Sep 2025 (AY 25-26). Using **~7.5 crore** to include audit cases. | [Bhaskar](https://english.bhaskardigital.com/itr-filing-sets-new-record-over-7-8-crore-income-tax-returns-filed-by-august-31/), [PIB (AY 24-25: 7.28 cr)](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2040669&reg=48&lang=2) |
| ITR form mix | ITR-1 45.8%, ITR-2 14.9%, ITR-3 12.5%, ITR-4 25.8%, ITR-5 to 7 1.0% | [PIB](https://www.pib.gov.in/PressReleasePage.aspx?PRID=2040669&reg=48&lang=2) |
| First-time filers | ~58.6 lakh per year | PIB |
| Active GST registrations | 1.52 crore (1.33 crore normal, ~15 lakh composition) | [IANS / SBI Research](https://ianslive.in/every-1-in-5-gst-taxpayers-in-india-now-a-women-sbi-research--20250722100004) |
| Assisted filing price | ₹1,299 (salary) to ₹3,999+ (capital gains / business) | [ClearTax](https://cleartax.in/meta/Pricing) |
| Market leader revenue | Clear (Defmacro): ₹272 cr in FY25, +30% YoY, ₹96 cr loss. Covers ITR, GST and enterprise products. | [Entrackr](https://entrackr.com/fintrackr/clear-reports-rs-272-crore-revenue-and-rs-96-crore-loss-in-fy25-10808038) |
| India tax management software (third-party report) | USD 466M (2023), forecast USD 959M by 2030, 10.9% CAGR | [Grand View Research](https://www.grandviewresearch.com/horizon/outlook/tax-management-software-market/india) |

### TAM: all tax-filing spend in India, if every filer paid a fair price

**Individual ITR**

| Segment | Filers | Price assumed | Value |
|---------|--------|---------------|-------|
| ITR-1 (salaried, simple) | 3.45 cr | ₹1,000 | ₹3,450 cr |
| ITR-2 (capital gains, NRI) | 1.12 cr | ₹3,000 | ₹3,375 cr |
| ITR-3 (business / F&O) | 0.94 cr | ₹5,000 | ₹4,690 cr |
| ITR-4 (presumptive) | 1.95 cr | ₹1,500 | ₹2,925 cr |
| ITR-5 to 7 (firms, trusts) | 0.08 cr | ₹10,000 | ₹770 cr |
| **Subtotal** | **7.5 cr** | | **≈ ₹15,000 cr (~$1.7B)** |

**GST compliance (SMBs)**

| Segment | Count | Annual spend assumed | Value |
|---------|-------|----------------------|-------|
| Normal taxpayers | 1.33 cr | ₹12,000 (≈ ₹1,000/month to an accountant or software) | ₹16,000 cr |
| Composition taxpayers | 0.15 cr | ₹3,000 | ₹450 cr |
| **Subtotal** | | | **≈ ₹16,500 cr (~$1.9B)** |

**Combined TAM ≈ ₹31,000 cr (~$3.5B per year).** Most of this money currently goes to offline CAs and local accountants, not software.

### SAM: the part a digital, consumer-focused ITR product can realistically serve

Focus on individuals who have real complexity, file online and are willing to pay:

| Segment | Share taken | Filers | Price | Value |
|---------|-------------|--------|-------|-------|
| ITR-2 (investors, capital gains, NRIs) | 100% | 1.12 cr | ₹2,500 | ₹2,810 cr |
| ITR-3 (traders, freelancers, professionals) | 50% (urban, digital) | 0.47 cr | ₹4,000 | ₹1,880 cr |
| ITR-1 (salaried who want help or optimisation) | 25% | 0.86 cr | ₹800 | ₹690 cr |
| **SAM** | | **~2.45 cr filers** | | **≈ ₹5,400 cr (~$600M)** |

If you also target **GST for digital-first SMBs**, assume about 20% of normal GST taxpayers (~27 lakh) at ₹6,000 per year. That adds about ₹1,600 cr, for a **combined SAM of about ₹7,000 cr (~$800M)**.

**Sanity check:** Grand View sizes India tax software at about $0.5–1B, which is the same range as this SAM. The leader, Clear, earns ₹272 cr across all its products, roughly 4–5% of SAM. That points to a fragmented market that is still mostly offline.

### SOM (reference)

A new entrant that wins **2–3% of the individual-ITR SAM in 3–5 years** would earn about **₹110–160 cr per year**.

### Caveats

- Prices and paid-share percentages are assumptions. Change them and the TAM or SAM moves proportionally.
- ITR counts are filings, not unique people, though they are close.
- The ₹ to $ conversion uses about ₹88 per $1.
- Several problem-side sources are vendor blogs. Treat their specific percentages as indicative.
