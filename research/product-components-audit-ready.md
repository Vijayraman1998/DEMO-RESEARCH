# Product components for a complete internal (tax) audit workflow that leaves the company ready for external audit

*Date: 15 Oct 2026. Scope: an AI internal audit platform for Indian tech companies (GCCs, IT/ITES, SaaS). It starts with internal tax audit and extends to full internal audit. Items marked † are from general knowledge; check them against the current statute or standard before building rules.*

**An honest limit:** no tool can *guarantee* "no problems in the external audit". The external auditor forms an independent opinion and decides how much to rely on internal audit work. Under SA 610 (ISA 610), the auditor checks internal audit's **objectivity, competence and systematic, disciplined approach (including quality control)**. The auditor cannot rely on it if objectivity or competence is low, and keeps sole responsibility for the opinion ([ClearTax on SA 610](https://cleartax.in/s/sa-610-using-the-work-of-internal-auditors), [ACCA](https://www.accaglobal.com/uk/en/student/acca-qual-student-journey/qual-resource/acca-qualification/f8/technical-articles/internal-auditors.html), [ISA 610](https://ktkt.uel.edu.vn/Resources/Docs/SubDomain/ktkt/VanBan/ISA/ISA%20610.pdf)).

**The design goal** is therefore:
1. Fix issues *before* the auditor finds them.
2. Produce documentation good enough that the auditor can **rely on it** under SA 610.
3. Hand over a complete, tied-out **audit-ready pack**.

---

## 0. What the external auditors will look at, and so what the product must prepare for

| External audit / report | Who | What they need from the company | Covered by component |
|-------------------------|-----|--------------------------------|---------------------|
| **Statutory audit** (financial statements, SAs) | Statutory auditor | Tied-out schedules, evidence, related-party list, management representations, internal audit reports | 1, 3, 6, 7, 9 |
| **IFC over financial reporting** (Sec 143(3)(i)) † | Statutory auditor | Risk-control matrix, design and operating-effectiveness test results, deficiencies | 2, 4, 7 |
| **CARO 2020** | Statutory auditor | 3(vii)(a) undisputed statutory dues (GST, PF, ESI, income tax and others) paid regularly, and arrears over 6 months. 3(vii)(b) disputed dues with amount and forum. 3(xiv) adequacy of internal audit. ([Taxmann](https://taxmann.com/post/blog/reporting-of-statutory-dues-under-caro-observations-by-frrb), [TaxGuru](https://taxguru.in/company-law/caro-2020-key-clauses.html)) | 5, 8 |
| **Audit trail** (Rule 3(1) Accounts Rules / Rule 11(g) Audit Rules) | Statutory auditor | Proof that the edit log was on all year for all transactions | 1, 5 |
| **Tax audit, Sec 44AB / Form 3CD** | Tax auditor (CA) | Clause-wise schedules: 43B / 43B(h), 40(a)(i)/(ia) TDS disallowances, related parties, GST details, loans, deemed income and others † | 5 (Income-tax / 3CD) |
| **Transfer-pricing report** (Form 3CEB, Master File / CbCR) † | Accountant (CA) | Intercompany transaction list, agreements, cost base, markup, benchmarking | 5 (TP) |
| **GST annual return / reconciliation** (GSTR-9 / 9C) † | Company (self-certified) | Books-to-returns reconciliation, ITC tables, tax paid | 5 (GST) |
| **Tax provisions** (Ind AS 12, uncertain tax positions; Ind AS 37 contingent liabilities) † | Statutory auditor | Current and deferred tax workings, uncertain tax positions, tax disputes and contingent-liability schedule | 5, 8 |

---

## 1. Data and integration layer (the foundation)

| Sub-component | What it does |
|---------------|-------------|
| ERP / accounting connectors | NetSuite, SAP, Oracle, Dynamics, Zoho Books, Tally †. Pull trial balance, GL, sub-ledgers, vendor and customer masters, fixed assets. |
| Government data | GST portal (GSTR-1, 3B, 2B, e-invoice and e-way bill) through a GSP; TRACES / 26AS / AIS; income-tax portal (notices, demands, refunds) |
| Other sources | Payroll (including ESOP), bank statements, intercompany ledgers or parent ERP, contract repository (MSAs, SOWs), 15CA/CB acknowledgements |
| **Completeness and tie-out checks** | Every data pull reconciles to the trial balance, and filed returns reconcile to the books before any testing. Auditors reject analysis built on incomplete data. |
| **Audit-trail / edit-log ingestion** | Ingest the ERP change logs to prove the log was on all year and to flag back-dated or edited entries |
| Master-data validation | PAN, GSTIN and TAN validation, MSME status of vendors (for 43B(h)), related-party flags, foreign-vendor treaty data |
| Multi-entity / multi-GSTIN model | GCCs and IT companies have several state GSTINs and sometimes several legal entities |

## 2. Governance and planning

- **Internal audit charter and methodology** aligned to the **IIA Global Internal Audit Standards (2025)** and **ICAI Standards on Internal Audit** (including draft SIA 240 on technology), to meet SA 610's "systematic and disciplined approach" test
- **Audit universe and risk assessment:** tax risks first (GST, TDS, TP, income tax, payroll tax), then finance and operations
- **Risk-control matrix (RCM) library:** ready-made controls and tests for tech companies, which customers can edit
- **Annual audit plan** with Audit Committee approval workflow
- **Independence and competence records:** team qualifications, conflict declarations, and reviewer assignments (SA 610 evidence)

## 3. Evidence and document management

- **Evidence vault:** invoices, contracts, challans, returns and approvals, each **linked to the transaction or test it supports**
- **Document AI:** reads invoices, MSAs/SOWs (for "intermediary" risk, PE indicators and TP terms), Form 16A/15CB, and notices
- **Immutable logs and versioning:** who changed what and when, inside the tool itself (auditors test this)
- **Retention policy:** keep records for the statutory retention and reassessment window (longer under IT Act 2025 reassessment limits)

## 4. Test execution engine

- **Full-population tests by default**, with statistical sampling only where full testing isn't possible, documented with the rationale
- **Control testing in two stages:** design (walkthrough) and operating effectiveness, which feeds IFC
- **Continuous monitoring:** monthly or quarterly runs, plus an intensive year-end pre-audit
- **AI exception triage:** ranks exceptions by ₹ exposure, explains why each was flagged and cites the rule, and a human confirms

## 5. Tax audit modules (the starting wedge)

| Module | Key tests and outputs |
|--------|-----------------------|
| **GST** | GSTR-1 vs 3B vs books. ITC vs GSTR-2B (vendor non-filing, blocked credits). Export of services: LUT, realisation in foreign exchange, Rule 89(4) refund computation. HO–BO / overseas-branch treatment, including **57th GST Council (Oct 2026)** changes. Intermediary-risk contract flags. Cross-charge and ISD distribution. RCM on imported services. E-invoice coverage. **GSTR-9 / 9C reconciliation pack.** |
| **TDS / TCS** | Section-wise rate and threshold checks. Lower-deduction certificates. TDS returns (24Q/26Q/27Q) vs books vs challans. Late deduction and late payment interest. **Sec 195 / 15CA-CB:** royalty vs fees-for-technical-services vs business-income classification, DTAA rates, TRC/Form 10F, grossing-up †. Payroll TDS, including **ESOP perquisites**. |
| **Income tax / Form 3CD readiness** | Clause-wise draft schedules with exceptions: **43B(h) MSME payments**, 43B statutory dues, **40(a)(i)/(ia)** disallowances, related-party payments, loans and deposits, deemed income, **audit-trail status**. Mapped to **IT Act 2025** section numbering †. |
| **Transfer pricing / intercompany** | Intercompany invoices vs agreements. Cost-base completeness, including pass-through costs and ESOP recharges. Markup check vs policy and the **safe-harbour** test (Budget 2026 changes). Overdue intercompany receivables (deemed-loan risk). Data pack for **Form 3CEB** and Master File / CbCR. |
| **Payroll and statutory dues** | PF, ESI, professional tax (multi-state), LWF. Paid on time vs due dates. **CARO 3(vii)(a) arrears over 6 months** list. |
| **Tax provisions and disputes** | Current tax and deferred tax workings support (Ind AS 12). Uncertain tax position register. **Disputed dues by forum (CARO 3(vii)(b))**. Contingent-liability schedule (Ind AS 37) †. |
| **Special regimes** † | SEZ / STPI compliance (Softex, SEZ zero-rating). PE-risk indicators (India-based leadership acting for the parent). FEMA reporting links for foreign payments. |

## 6. Full internal audit modules (expansion)

| Module | Examples of tests |
|--------|-------------------|
| **Record-to-Report** | Manual and unusual journals (weekend, back-dated, round amounts, unusual users). Period-end cut-off. Account reconciliations. Audit-trail edits. |
| **Revenue / Order-to-Cash** (Ind AS 115 for SaaS) † | Contract vs billing vs revenue recognition. Deferred revenue. Credit notes. Unbilled receivables. FX realisation. |
| **Procure-to-Pay** | Duplicate vendors and invoices. PO–GRN–invoice match. Approvals. Related-party vendors. MSME payment timelines. |
| **Payroll / Hire-to-Retire** | Ghost employees. Payroll vs HRMS. Full-and-final settlements. Bonus and ESOP accounting. |
| **Fixed assets and capitalised software** | Capitalisation criteria for internally developed software. Depreciation and amortisation. Disposals. |
| **Treasury** | Bank reconciliations. FX hedging. Investments. Covenants. |
| **ITGC / SoD** | ERP user access, segregation-of-duties conflicts, change management, privileged access. Directly relevant to IFC and audit-trail reporting. |
| **Related parties** | Complete related-party list vs transactions. Approvals (Sec 188 / audit committee) †. |

## 7. Working papers and review (what makes the work *reliable* for the external auditor)

- **Standard working paper per test:** objective; criteria and regulation (with citation); data source and completeness tie-out; population or sample; procedure; results; exceptions; conclusion; and **preparer and reviewer sign-off with timestamps**
- **Maker-checker review workflow,** with review notes that must be cleared before sign-off (quality control under SA 610)
- **AI-drafted, human-approved:** AI drafts the working paper and an auditor reviews and signs. Every AI output keeps citations and the underlying data so it can be **re-performed**.
- **Cross-referencing and tickmarks:** each number traces back to the trial balance, the return or the source document

## 8. Findings, remediation and compliance tracking

- **Finding register:** condition, criteria, cause, effect (₹ quantified), recommendation, risk rating, owner, due date
- **Management response and remediation tracking,** with **re-testing** before closure
- **Root-cause linkage:** connect each finding to a control or process fix so the same notice doesn't recur
- **Compliance calendar:** GST, TDS, PF/ESI, TP, ITR and 3CD due dates, with filed vs pending status
- **Notice and litigation tracker:** fetch notices from the GST, income-tax and TRACES portals; record replies and deadlines; record forum and amount (feeds **CARO 3(vii)(b)** and contingent liabilities)

## 9. Reporting and external-audit handoff

| Output | Audience |
|--------|----------|
| **Audit Committee report** (quarterly): coverage, key findings, ₹ exposure, remediation status, tax-risk heat map | Audit Committee, board |
| **CFO and tax-head dashboard:** ITC at risk, refunds pending, notices, TDS exposure, TP status | Management |
| **IFC test report:** controls tested, deficiencies, significant deficiencies or material weaknesses | Management and statutory auditor |
| **Audit-ready pack (PBC):** auto-generated "prepared-by-client" schedules for the statutory auditor, the 3CD tax auditor, the 3CEB accountant and GSTR-9C, each tied to the trial balance and returns | External auditors |
| **External-auditor portal:** read-only access to working papers and evidence, a **query/response tracker**, and status of each PBC item | External auditors |
| **Management representation support:** list of known issues, disputes and contingencies to inform the representation letter | CFO and statutory auditor |

## 10. Regulatory content and rules engine

- **Rules library** covering GST, TDS, income tax, TP, CARO, audit-trail and payroll laws, with **effective dates** so each year is tested under the right rules
- **Change management:** IT Act 2025 ↔ 1961 section mapping; GST Council decisions (for example, the 57th meeting on HO–BO and R&D exports); safe-harbour updates; CBDT/CBIC circulars
- **Expert review:** a CA/tax expert approves every rule before release, with version notes

## 11. Platform, security and trust

- **Security:** ISO 27001, then SOC 2 Type II; **data residency in India**; DPDPA compliance; encryption; SSO; role-based access
- **AI governance:** no customer data used to train shared models without consent; explainable outputs; human approval for conclusions; model-change logs
- **Tool-level audit log:** the platform itself has an immutable activity log, which external auditors may test as part of ITGC
- **Multi-entity and consolidation:** group view across Indian entities and GSTINs

---

## Build order (suggested)

| Phase | Components | Why first |
|-------|-----------|-----------|
| **MVP (0–6 months)** | 1 (ERP + GST + TRACES connectors, tie-out), 3 (evidence vault), 4 (test engine), **5: GST + TDS/195 + 3CD readiness**, 7 (working papers + review), 9 (audit-ready pack v1), 11 (basic security) | Solves the highest-₹ problems (ITC, notices, disallowances) and gives the external auditor a usable pack |
| **Phase 2 (6–12 months)** | 5: TP / intercompany, payroll and statutory dues, CARO 3(vii) schedules, provisions and disputes; 8 (finding register, notice tracker, calendar); 10 (rules engine with IT Act 2025 mapping) | Full tax coverage and CARO / contingent-liability readiness |
| **Phase 3 (12–24 months)** | 2 (planning, RCM, Audit Committee workflow), 6 (R2R, revenue, P2P, payroll, ITGC/SoD), IFC testing, auditor portal, SOC 2 | Becomes a full internal audit platform that external auditors can rely on under SA 610 |

## Checklist: "ready for external audit"

- [ ] All data tied to the trial balance and to filed returns
- [ ] Audit trail confirmed on all year; edits explained
- [ ] GSTR-1/3B/2B/books reconciled; GSTR-9/9C pack ready
- [ ] TDS returns, challans and books reconciled; 195 / 15CA-CB evidence complete
- [ ] 3CD clause schedules drafted with exceptions resolved or explained
- [ ] TP intercompany data and 3CEB support ready
- [ ] CARO 3(vii) undisputed arrears list (over 6 months) and disputed-dues-by-forum list ready
- [ ] Tax provision, uncertain tax position and contingent-liability schedules ready
- [ ] Every finding has a management response; high-risk ones remediated and re-tested
- [ ] Working papers reviewed and signed off; external-auditor portal access granted
