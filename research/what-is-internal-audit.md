# What internal audit is, and where AI fits (India)

*Date: 14 Oct 2026. A primer for an AI / automation startup focused on internal audit. Read this before the TAM, competitor and GTM files. Items marked † are from general knowledge and were not confirmed by a source found in this research.*

---

## 1. What internal audit is

Internal audit is an **independent, objective function inside a company**. It checks whether the company's **risk management, internal controls and governance** actually work, and reports to the **Audit Committee of the board**, not to the people it audits.

In plain terms, internal audit answers:
- Are processes followed?
- Is money leaking?
- Are we compliant?
- Are the numbers reliable?
- What could go wrong next?

It then recommends fixes and tracks them until they are closed.

### Internal audit vs statutory audit

| | **Internal audit** | **Statutory (external) audit** |
|---|---|---|
| Purpose | Improve controls, risk management and operations | Give an opinion on whether the financial statements are true and fair |
| Who appoints | Board (Sec 138), with scope set by the Audit Committee | Shareholders (Sec 139) |
| Who performs | In-house team, or an outsourced / co-sourced CA or advisory firm. **Cannot be the statutory auditor.** | Independent CA firm |
| Frequency | Continuous or rolling through the year, often quarterly reports | Annual (plus quarterly limited reviews for listed companies) |
| Scope | Any process: finance, operations, IT, compliance, fraud, ESG | Financial statements, IFC over financial reporting, CARO |
| Output | Findings, risk ratings, management action plans, Audit Committee reports | Audit opinion |

**How the two connect:** under CARO 2020 clause 3(xiv), the statutory auditor must report whether the company has an internal audit system that matches its size, and whether the statutory auditor considered the internal audit reports. ([TaxGuru](https://taxguru.in/company-law/applicability-caro-2020-ifc-reporting-internal-audit-cash-flow-ind.html)) Weak internal audit therefore shows up in the statutory audit report.

---

## 2. Legal and professional framework in India

| Item | What it says |
|------|-------------|
| **Companies Act Sec 138 + Companies (Accounts) Rule 13** | Internal audit is mandatory for all listed companies, unlisted public companies above the thresholds, and private companies with turnover ≥ ₹200 cr or borrowings > ₹100 cr. The Audit Committee or board sets the scope, frequency and method. ([TaxGuru](https://taxguru.in/company-law/internal-audit-applicability-private-companies-india.html)) |
| **Sec 177 (Audit Committee)** † | Reviews internal controls, internal audit findings, related-party transactions and the vigil (whistle-blower) mechanism |
| **Sec 134(5)(e) and 143(3)(i): Internal Financial Controls (IFC)** † | Directors certify that IFC are adequate. Statutory auditors report on IFC over financial reporting. Internal audit usually does the IFC testing. ([WIRC-ICAI IFC material](https://old.wirc-icai.org/images/material/Internal_Financial_Controls-IFCOR.pdf)) |
| **CARO 2020 clause 3(xiv)** | Statutory auditor comments on the adequacy of internal audit |
| **Audit trail rule (Rule 3(1) of the Accounts Rules)** | Edit logs must be kept in accounting software, and auditors report on them. Internal audit is expected to check them. |
| **RBI risk-based internal audit (RBIA)** | Banks, deposit-taking NBFCs and HFCs, larger NBFCs and HFCs, and urban cooperative banks with assets ≥ ₹500 cr. ([Business Standard](https://www.business-standard.com/amp/article/economy-policy/rbi-makes-risk-based-internal-audit-mandatory-for-select-nbfcs-ucbs-121020302071_1.html)) |
| **SEBI LODR (listed companies)** † | Audit Committee reviews internal audit reports, and the CEO/CFO certify internal controls |
| **ICAI Standards on Internal Audit (SIAs)** | Historically "recommended". A restructured set (planning, execution, reporting, quality) was in exposure draft in 2025 and **may become mandatory**. A draft **SIA 240 covers the use of technology and tools**, including data analytics and AI. ([ICAI](https://www.icai.org/post/1194), [ICAI IA Board](https://internalaudit.icai.org/?p=2600), [SIA 240 draft](https://internalaudit.icai.org/wp-content/uploads/2025/09/SIA-240.pdf)) |
| **IIA Global Internal Audit Standards (2024, effective 9 Jan 2025)** | Global standard with 5 domains and 15 principles: Purpose; Ethics & Professionalism; Governing the function; Managing the function; Performing services. Used by IIA-certified (CIA) teams and MNC subsidiaries. ([KPMG](https://kpmg.com/ie/en/insights/audit/2024-global-internal-audit-standards.html)) |

**Startup implication:** if ICAI's new SIAs become mandatory, and SIA 240 explicitly covers technology, then documentation, evidence and quality requirements rise. That creates demand for tools that produce standards-compliant working papers.

---

## 3. What internal audit checks: the "audit universe"

A medium-sized company's annual plan typically has **15–25 audit engagements** ([CorpReady](https://corpready.in/resources/articles/216-internal-audit-process.html)). Common areas, drawn from the ICAI checklist and practitioner sources ([ICAI KB](https://kb.icai.org/pdfs/PDFFile663b0b7ae22563.36932492.pdf), [VJM Global](https://www.vjmglobal.com/feeds/blog/scope-internal-audit-india)):

| Area | What gets checked (examples) |
|------|------------------------------|
| **Procure-to-Pay (P2P)** | Vendor onboarding and KYC, duplicate vendors or invoices, PO–GRN–invoice 3-way match, approval limits, split POs, payments to related parties |
| **Order-to-Cash (O2C)** | Customer credit limits, pricing and discount overrides, revenue cut-off, credit notes, receivables ageing, collections |
| **Inventory & warehousing** | Physical verification vs books, slow-moving or obsolete stock, write-offs, stock transfers between depots |
| **Record-to-Report (R2R) / book close** | Manual journal entries, entries posted on weekends or by unusual users, provisions, reconciliations, audit-trail edits |
| **Hire-to-Retire / payroll** | Ghost employees, payroll vs attendance, full-and-final settlements, statutory deductions (PF, ESI, TDS) |
| **Fixed assets & capex** | Capitalisation, asset tagging and verification, capex approvals vs budget |
| **Treasury, cash & bank** | Bank reconciliations, borrowings and covenants, investments, cash handling |
| **Taxation** | GST (GSTR-1/3B/2B reconciliation, ITC), TDS/TCS, income tax provisions and notices |
| **Statutory & regulatory compliance** | Labour laws, environment, Companies Act, SEBI and sector regulators (RBI, FSSAI, CDSCO) |
| **IT general controls (ITGC)** | User access, segregation of duties in SAP or Oracle, change management, backups, cyber |
| **Branch / plant / store audits** | On-site operational checks across many locations, a big share of effort in retail, BFSI and manufacturing |
| **Fraud & investigations / whistle-blower cases** | Forensic reviews, conflict-of-interest checks |
| **Emerging areas** | ESG/BRSR data, third-party/vendor risk, AI and data governance, cyber |

---

## 4. How an internal audit is done: lifecycle, pain points and AI opportunity

| Stage | What happens | Manual pain today | Where AI / automation helps |
|-------|-------------|-------------------|-----------------------------|
| **1. Risk assessment & annual plan** | Build the audit universe, rate risks, get the plan approved by the Audit Committee | Done in Excel. Risk ratings are subjective, and last year's plan is copied. | Data-driven risk scoring from ERP data, past findings, news and regulatory changes. Auto-drafted annual plan. |
| **2. Engagement planning** | Understand the process, write the risk-control matrix (RCM), define tests, send data requests | Process walkthroughs, writing RCMs from scratch, chasing data | Auto-generated RCMs and test programmes from standard libraries and the company's SOPs |
| **3. Data collection & fieldwork** | Pull data from ERP, Tally or SAP, sample transactions, collect evidence (invoices, approvals, contracts) | Data extraction is the bottleneck. Evidence is PDFs and emails. Document work can take **up to 71% of audit prep time** (PwC, via [FieldGuide](https://www.fieldguide.io/resource-articles/ai-audit-preparation-reporting)). | ERP connectors. **Full-population testing instead of samples.** Document AI to read invoices and contracts and match them to ledger entries. |
| **4. Testing & analysis** | Test control design and operating effectiveness, analytics, exceptions | Sample-based (for example 25 of 10,000). Excel analytics. IDEA/ACL need specialists. | Anomaly detection (duplicates, unusual journals, split POs, SoD conflicts), continuous controls monitoring, AI triage of exceptions |
| **5. Working papers & review** | Document tests and conclusions, then manager or partner review | Hours of documentation and review notes. Quality is inconsistent. | Auto-drafted working papers from the tests run. AI first-pass review against SIA/IIA standards. |
| **6. Reporting** | Draft observations (condition, criteria, cause, effect, recommendation), management responses, Audit Committee deck | Many rounds of drafting and formatting the quarterly deck | AI-drafted observations and executive summaries. Audit Committee dashboards. |
| **7. Follow-up / action tracking** | Track whether management fixed issues by the due date | Email and Excel chasing. Repeat findings. | Automated follow-up, evidence of closure, re-testing of fixed controls |
| **8. IFC / ICFR testing** (annual) | Test key controls over financial reporting for the director and auditor certification | Repetitive yearly testing of the same controls | Reusable automated tests run continuously all year |

### Problems across the whole function

- **Talent:** more than half of Indian audit heads lack subject-matter experts, and only about 16% feel highly prepared for emerging risks ([IIA India–Protiviti 2025](https://www.industrialautomationindia.in/news/chief-audit-executives-ai-cybersecurity-risks-iia-protiviti-survey-2025)).
- **Low tech adoption:** only about 4% of teams globally report significant GenAI progress ([AuditBoard](https://cfotech.in/story/auditboard-study-reveals-internal-audit-struggles-in-2025)).
- **Hindsight, not foresight:** most work is quarterly and sample-based, while regulators (GSTN, the income tax system, RBI) now analyse 100% of data.
- **Fragmented data:** data sits across ERPs, Tally instances at branches, spreadsheets and email.

---

## 5. What this means for the startup: refocused on internal audit

**Positioning:** an *AI internal audit platform* that lets a small in-house team or an outsourced audit firm cover the **whole audit universe** with **full-population testing**, using auto-generated working papers and reports that conform to ICAI SIA and IIA standards.

**Suggested product sequence:**

1. **Data and analytics core.** Tally, SAP and Oracle connectors, plus a library of ready-made tests for P2P, O2C, R2R and payroll: duplicates, 3-way match, unusual journals, SoD and audit-trail edits. *These are the highest-volume, most repetitive audits.*
2. **AI working papers and reporting.** RCM generation, observation drafting and the Audit Committee deck. *This saves the most audit hours.*
3. **Continuous controls monitoring and IFC testing all year.** *This makes the product a subscription rather than a project.*
4. **Specialised modules.** Tax (GST/TDS/ITC), branch audits (mobile), ITGC/SoD, ESG/BRSR, and BFSI RBIA.

Tax becomes **one module among several**, not the whole product.

**Target customers (updated):**
- Companies with ₹500–5,000 cr turnover that must have internal audit (in-house teams of 2–10 people).
- Outsourced internal audit and CA firms, as a channel. One firm serves many mandated companies.
- NBFCs, HFCs and cooperative banks under RBIA, later.

**First customer conversations should validate:**
- Which audit areas take the most hours.
- How data is pulled today.
- Who writes working papers and how long that takes.
- What the Audit Committee asks for.
- Who owns the internal audit budget, and how much it is.
