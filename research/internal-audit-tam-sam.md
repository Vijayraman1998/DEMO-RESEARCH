# TAM and SAM for an AI internal audit platform in India (full internal audit scope)

*Date: 14 Oct 2026. Replaces the TAM/SAM section of `internal-audit-large-companies-india.md`, which focused on finance and tax controls. This version covers the **whole internal audit function** (every audit area and every regulated sector).*

**Read this first:** no published report sizes India's internal audit market. Every number below is a **bottom-up estimate**. The inputs that come from sources are cited. The rest are assumptions, labelled as such, so you can change them. Items marked † are from general knowledge, not from a source found in this research.

---

## Summary

| Layer | What it measures | Estimate |
|-------|------------------|----------|
| **TAM: total spend** | Everything Indian organisations spend on internal audit each year (in-house staff, outsourced and co-sourced firms, concurrent audit, tools) | **≈ ₹28,000 cr (~$3.2B)** |
| **TAM: software** | What that market would spend on internal audit software at fair prices | **≈ ₹4,900 cr (~$560M)** |
| **SAM** | What an India-built AI internal audit startup can realistically serve in 3–5 years (mid-to-large corporates, NBFCs/HFCs, and smaller mandated companies through audit firms) | **≈ ₹2,600 cr (~$300M)** |
| **SOM** | A realistic 3–5 year revenue target | **≈ ₹35–50 cr ARR (~$4–6M)** |

The ₹ to $ conversion uses about ₹88 per $1.

---

## 1. Who must do internal audit (the demand)

| Segment | Rule | Count used | Basis |
|---------|------|-----------|-------|
| Listed companies | Sec 138: always mandatory | ~5,500–6,000 unique | NSE about 2,700, BSE about 5,700 ([Motilal Oswal](https://www.motilaloswal.com/blog-details/how-many-companies-are-listed-in-the-indian-stock-market/20955)) |
| Unlisted public and private companies | Sec 138: turnover ≥ ₹200 cr, or borrowings > ₹100 cr (public companies also on capital or deposits) | **~40,000 corporates in total** (range 30k–60k), including listed | **Assumption.** No official count was found. More than 50,000 PAN-level entities have turnover above ₹500 cr ([ClearTax News](https://news.cleartax.in/?p=5471)), and that figure includes non-companies. About 12,000 companies were newly mandated since 2023 (vendor estimate, [Dataintelo](https://dataintelo.com/report/global-internal-audit-outsourcing-market)). |
| Banks | RBI: risk-based internal audit, concurrent audit and IS audit | 12 public, 21 private, 44 foreign and 11 small finance banks, plus about 43 RRBs † | [RBI](https://rbi.org.in/SCRIPTS/PublicationsView.aspx?id=23653). About 1.6 lakh branches †. |
| NBFCs / HFCs | RBIA for all deposit-taking NBFCs and HFCs, and non-deposit-taking ones with assets ≥ ₹5,000 cr. Middle- and upper-layer NBFCs run full internal audit. | ~650 (middle and upper layer = about 7% of about 9,300 NBFCs) | [RBI NBFC list](https://website.rbi.org.in/documents/87730/39016390/ListofNBFCsandARCsregisteredwiththeRBI.pdf), [RBI report](https://rbi.org.in/SCRIPTs/PublicationsView.aspx?id=23641), [Business Standard](https://www.business-standard.com/amp/article/economy-policy/rbi-makes-risk-based-internal-audit-mandatory-for-select-nbfcs-ucbs-121020302071_1.html) |
| Cooperative banks | RBIA for urban cooperative banks with assets ≥ ₹500 cr. Concurrent audit at state and district cooperative banks. | ~300 large urban cooperative banks plus state and district cooperative banks † | Fee examples in [HP State Cooperative Bank](https://hpscb.bank.in/upload/tender/7gVdFkM084A3QSDcjaizG20bcDszKYuC0AGhF8RR.pdf) and [Prakasam DCCB](https://prakasamdccb.bank.in/wp-content/uploads/2025/04/RBIA.pdf) tenders |
| Insurers | IRDAI corporate-governance rules require internal audit † | ~70 insurers † | — |
| Voluntary (not mandated) | Companies with ₹50–200 cr turnover that run internal audit by choice | ~10,000 (assume 20% of about 50,000) | **Assumption** |

### Corporate tiers (assumption)

| Tier | Turnover | Companies |
|------|----------|-----------|
| T1a, Very large | > ₹5,000 cr | ~1,000 |
| T1b, Large | ₹1,000–5,000 cr | ~4,000 |
| T2, Upper mid | ₹500–1,000 cr | ~10,000 |
| T3, Mandated mid | ₹200–500 cr, or borrowings > ₹100 cr, or small listed | ~25,000 |

---

## 2. TAM, total-spend view: ≈ ₹28,000 cr per year

Covers in-house internal audit salaries, fees to outsourced, co-sourced and concurrent auditors, and tools.

| Segment | Calculation (assumptions) | Annual spend |
|---------|---------------------------|--------------|
| Corporates T1 (a+b) | 5,000 × ₹3 cr (in-house team of 10–30 plus Big 4 / CA co-source) | ₹15,000 cr |
| Corporates T2 | 10,000 × ₹50 lakh | ₹5,000 cr |
| Corporates T3 | 25,000 × ₹15 lakh | ₹3,750 cr |
| Banks: concurrent audit fees | About 30,000 branches under concurrent audit × ₹15,000/month × 12. Tenders show ₹7,500–26,000 per branch per month ([Nainital Bank](https://www.nainitalbank.bank.in/pdf/Tender_Proposal_NO_NTB_CIAD_CONCURRENT_2025_02_001.pdf), [HP State Cooperative Bank](https://hpscb.bank.in/upload/tender/7gVdFkM084A3QSDcjaizG20bcDszKYuC0AGhF8RR.pdf), [TaxGuru / Andhra Bank](https://taxguru.in/chartered-accountant/online-empanelment-ca-firms-concurrent-audit-andhra-bank.html)) | ₹540 cr |
| Banks: in-house inspection and audit departments | About 16,000 staff (roughly 1 per 10 branches) × ₹15 lakh loaded cost | ₹2,400 cr |
| NBFCs / HFCs | 650 × ₹1 cr | ₹650 cr |
| Cooperative banks | Lump estimate | ₹200 cr |
| Insurers | 70 × ₹5 cr | ₹350 cr |
| Voluntary internal audit | 10,000 × ₹4 lakh | ₹400 cr |
| **TAM** | | **≈ ₹28,300 cr (~$3.2B)** |

**Cross-checks:**
- Global internal audit services are about $75B ([Research and Markets](https://www.researchandmarkets.com/report/internal-audit)). India at 3–4% would be about $2.2–3B, the same range.
- Big 4 India revenue is about ₹38,800 cr across *all* service lines in FY24 ([The Finance Story](https://thefinancestory.com/big-4-india-ey-deloitte-pwc-kpmg-eyes-revenue-₹45000-cr)). Internal audit and risk is one slice of that, and the rest of this TAM is in-house staff and CA firms.
- Salary benchmarks for the in-house cost assumptions: internal auditors about ₹4–14 lakh, senior or manager about ₹9–23 lakh ([AmbitionBox](https://www.ambitionbox.com/salaries/cognizant-salaries/internal-auditor), [Eduyush](https://eduyush.com/en-us/blogs/cima/cia-salary-in-india)).

**Sensitivity:** if the corporate count is 30k–60k instead of 40k, TAM moves to about **₹22,000–40,000 cr**.

---

## 3. TAM, software view: ≈ ₹4,900 cr per year

This is the spend if every organisation above bought an internal audit platform at a fair contract value. The **annual contract values (ACV) are assumptions**.

| Segment | Entities | ACV | Value |
|---------|----------|-----|-------|
| Corporates T1 | 5,000 | ₹40 lakh | ₹2,000 cr |
| Corporates T2 | 10,000 | ₹12 lakh | ₹1,200 cr |
| Corporates T3 | 25,000 | ₹4 lakh | ₹1,000 cr |
| Banks | ~130 | ₹3 cr | ₹390 cr |
| NBFCs / HFCs | 650 | ₹20 lakh | ₹130 cr |
| Insurers | 70 | ₹50 lakh | ₹35 cr |
| Cooperative banks | ~300 | ₹5 lakh | ₹15 cr |
| Voluntary internal audit | 10,000 | ₹1.5 lakh | ₹150 cr |
| **Software TAM** | | | **≈ ₹4,900 cr (~$560M)** |

**Cross-checks:**
- This is about 17% of the total-spend TAM, which fits a reasonable 15–20% share of internal audit spend shifting to technology.
- MarketsandMarkets puts India eGRC (all governance, risk and compliance software, not only internal audit) at **$458.5M in 2024, growing to $930M by 2029** ([MarketsandMarkets](https://www.marketsandmarkets.com/Market-Reports/geography/enterprise-governance-risk-compliance-market/India)). That is the same order of magnitude.

---

## 4. SAM: ≈ ₹2,600 cr per year

The SAM is the part the startup can realistically win in 3–5 years with an India-built AI internal audit platform. It covers every audit area: P2P, O2C, R2R, payroll, inventory, fixed assets, tax, ITGC/SoD, branch audits, working papers, reporting and follow-up.

| Included segment | Why it's included | Entities | ACV | SAM |
|------------------|-------------------|----------|-----|-----|
| Corporates T2 (₹500–1,000 cr) | Internal audit is mandatory, teams are small and Excel-based, the CFO decides, and they are under-served by global tools | 10,000 | ₹12 lakh | ₹1,200 cr |
| Corporates T1b (₹1,000–5,000 cr) | Real budgets, but not locked into SAP GRC or Big 4 platforms | 4,000 | ₹25 lakh | ₹1,000 cr |
| NBFCs / HFCs under RBIA | Clear regulatory mandate. Easier than banks. | 650 | ₹20 lakh | ₹130 cr |
| Corporates T3, reached **through internal audit / CA firms** | Too small to sell to directly, but reachable via the firms that audit them. Assume 30% are reachable. | 7,500 | ₹4 lakh | ₹300 cr |
| **SAM** | | | | **≈ ₹2,630 cr (~$300M)** |

**Left out of SAM, and why:**

| Segment | Reason |
|---------|--------|
| T1a (largest ~1,000) | Locked into SAP GRC, MetricStream or Big 4 platforms, with 9–18 month sales cycles |
| Banks | eTHIC is entrenched, and security and procurement take a long time. A phase-2 target. |
| Insurers | Small count and IRDAI-specific needs |
| Voluntary small companies | Low budget, and internal audit is not mandatory |

---

## 5. SOM: ≈ ₹35–50 cr ARR in 3–5 years

| Source | Assumption | ARR |
|--------|-----------|-----|
| Direct corporate customers | 150–250 customers × ₹15 lakh average ACV | ₹22–38 cr |
| NBFCs / HFCs | 20 × ₹20 lakh | ₹4 cr |
| Internal audit / CA firm partners | 10 firms × 40 client entities × ₹2 lakh | ₹8 cr |
| **SOM** | | **≈ ₹35–50 cr (~$4–6M)**, about 1.5–2% of SAM |

---

## 6. Caveats and how to firm these up

1. **Number of companies by turnover band is the biggest uncertainty.** Pull counts from MCA21 (AOC-4 turnover and borrowings), CMIE Prowess, or a Lok Sabha / CBDT answer.
2. **Internal audit spend per company is assumed.** Validate it with 10–15 CFO or audit-head interviews, and with internal audit fee disclosures in annual reports of listed companies.
3. **Bank figures** (branch count, branches under concurrent audit, audit headcount) come from general knowledge and a few tenders. Check them against RBI's *Trend and Progress of Banking* tables.
4. **Contract values (ACV)** should be tested in paid pilots. Indian buyers are price-sensitive.
5. Growth drivers not included here: ICAI's revised Standards on Internal Audit (possibly mandatory, with SIA 240 on technology), audit-trail rules, the Income Tax Act 2025 transition, and ESG/BRSR assurance. Each adds scope and could push TAM up.
