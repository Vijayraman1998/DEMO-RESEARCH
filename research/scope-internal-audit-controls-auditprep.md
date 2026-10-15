# Confirmed scope: internal audit + control testing + audit prep

*Date: 15 Oct 2026. Decision: the product covers **internal audit, control testing (IFC/ICFR and SOX-style) and external-audit preparation**. The compliance calendar and notice/litigation tracker are dropped. Deep tax-compliance engines become one audit area among many, not the product.*

Items marked † are from general knowledge and were not confirmed by a source found in this research. All sizing is a bottom-up estimate on assumed counts and assumed spend.

---

## 1. What is in and what is out

| Component (from `product-components-audit-ready.md`) | Status |
|------|--------|
| 1. Data and integration layer | **In, core.** ERP, payroll, GST and TRACES data, audit-trail/edit-log ingestion, tie-out to trial balance |
| 2. Governance and planning (charter, risk assessment, RCM library, audit plan) | **In, promoted to core.** This is what makes the work rely-able under SA 610. It was Phase 3 before. |
| 3. Evidence and document management | **In, core** |
| 4. Test execution engine (full-population, design + operating effectiveness) | **In, core** |
| 5. Tax modules | **Reduced.** GST and TDS stay as **audit areas** (reconciliation, exception testing, CARO statutory-dues schedules). **Out:** refund computation, 15CA/CB workflow, 3CEB/Master File packs, transfer-pricing benchmarking. |
| 6. Full internal audit modules (R2R, revenue, P2P, payroll, fixed assets, treasury, ITGC/SoD, related parties) | **In, core.** Moves from Phase 3 to Phase 1–2. |
| 7. Working papers and review (maker-checker, sign-off, re-performable AI) | **In, core** |
| 8. Findings and remediation tracking | **Split.** Finding register, management response and re-testing are **in**. Compliance calendar and notice/litigation tracker are **out**. |
| 9. Reporting and external-audit handoff (Audit Committee report, IFC report, PBC pack, auditor portal) | **In, core.** This is the "audit prep" half of the promise. |
| 10. Rules engine | **Reduced** to audit content (control libraries, CARO/IFC criteria, standards mapping), not a live tax-rules engine |
| 11. Security and trust | **In, core** |

**New explicit component: IFC / ICFR and SOX-style control testing**
- Risk-control matrix per process, control owners, key vs non-key controls
- Design effectiveness (walkthroughs) and operating effectiveness (attribute testing)
- Deficiency evaluation and roll-up: deficiency → significant deficiency → material weakness †
- Entity-level controls and ITGC linkage
- Management's assessment pack for the Sec 143(3)(i) IFC report, and SOX 404 testing packs where the parent is US-listed †

---

## 2. Who buys now

| Buyer | Owns | Changed from |
|-------|------|--------------|
| **Head of Internal Audit / Chief Audit Executive** | Internal audit plan, findings, Audit Committee reporting | **New primary buyer** |
| **CFO / Financial Controller** | IFC/ICFR assessment, audit prep, auditor fees and timelines | **New co-primary buyer** |
| Head of Tax | GST/TDS audit areas only | Demoted to influencer |
| Audit Committee chair | Assurance coverage | Influencer |

This is a meaningful change: the earlier plan sold to the Head of Tax. Discovery calls must now be re-aimed at CAEs and controllers.

---

## 3. Sizing for this scope

### Stage A: tech industry (immediate market, ~4,150 entities)

**TAM, current spend ≈ ₹2,700 cr (~$307M)**

| Segment | Entities | Internal audit | IFC + audit prep | Each | Total |
|---------|----------|----------------|------------------|------|-------|
| Mega GCCs + large IT | 190 | ₹2.5 cr | ₹1 cr | ₹3.5 cr | ₹665 cr |
| Mid-to-large GCCs | 1,530 | ₹60 L | ₹25 L | ₹85 L | ₹1,301 cr |
| Mid Indian IT/ITES | 500 | ₹50 L | ₹20 L | ₹70 L | ₹350 cr |
| Mid-market GCCs | 480 | ₹20 L | ₹10 L | ₹30 L | ₹144 cr |
| Small IT/ITES | 1,000 | ₹10 L | ₹5 L | ₹15 L | ₹150 cr |
| SaaS entities | 450 | ₹13 L | ₹7 L | ₹20 L | ₹90 cr |
| **Total** | **4,150** | | | | **≈ ₹2,700 cr** |

**TAM, software ≈ ₹675 cr (~$77M)**

| Segment | Entities | ACV (assumption) | Total |
|---------|----------|------------------|-------|
| Mega GCCs + large IT | 190 | ₹70 L | ₹133 cr |
| Mid-to-large GCCs | 1,530 | ₹22 L | ₹337 cr |
| Mid Indian IT/ITES | 500 | ₹18 L | ₹90 cr |
| Mid-market GCCs | 480 | ₹9 L | ₹43 cr |
| Small IT/ITES | 1,000 | ₹4 L | ₹40 cr |
| SaaS entities | 450 | ₹7 L | ₹32 cr |
| **Total** | | | **≈ ₹675 cr** |

**SAM ≈ ₹480 cr (~$55M)**

| Segment | Entities | ACV | SAM |
|---------|----------|-----|-----|
| Mid-to-large GCCs | 1,530 | ₹22 L | ₹337 cr |
| Mid Indian IT/ITES (₹200–2,000 cr) | 500 | ₹18 L | ₹90 cr |
| Mid-market GCCs | 480 | ₹9 L | ₹43 cr |
| SaaS above $10M revenue | 150 | ₹7 L | ₹10 cr |
| **Total** | **2,660** | | **≈ ₹480 cr** |

*Excluded:* 190 mega GCCs and large IT companies (parent-group tools and Big 4 entrenched), ~1,300 small IT/SaaS entities (budget too low for direct sales).

**SOM ≈ ₹40–55 cr ARR by year 5** (250–350 customers, about 8–11% of SAM).

### Stage B: all sectors (end state)

| Layer | Spend TAM | Software TAM |
|-------|-----------|--------------|
| Internal audit, all mandated entities | ₹28,300 cr | ₹4,900 cr |
| IFC + audit prep, incremental | ₹3,500 cr | ₹700 cr |
| **Total** | **≈ ₹32,000 cr (~$3.6B)** | **≈ ₹5,600 cr (~$640M)** |

**SAM ≈ ₹2,285 cr (~$260M)**

| Segment | Entities | ACV | SAM |
|---------|----------|-----|-----|
| Tech (Stage A SAM) | 2,660 | — | ₹480 cr |
| Manufacturing: pharma, auto, chemicals, FMCG (₹500–5,000 cr) | ~6,000 | ₹16 L | ₹960 cr |
| Services, retail, healthcare, infra (₹500–5,000 cr) | ~3,000 | ₹13 L | ₹390 cr |
| NBFCs / HFCs under RBIA | 650 | ₹18 L | ₹117 cr |
| ₹200–500 cr companies via audit and CA firms | ~7,500 | ₹4.5 L | ₹338 cr |
| **Total** | **~19,800** | | **≈ ₹2,285 cr** |

**SOM ≈ ₹90–135 cr ARR by year 7** (about 4–6% of SAM).

### How this compares to the wider scope

| | Internal audit + controls + audit prep | All four budget lines (incl. tax engine, compliance, notices) |
|---|---|---|
| Tech SAM | ₹480 cr | ₹650 cr |
| All-sector SAM | ₹2,285 cr | ₹3,100 cr |
| Year-5 SOM (tech) | ₹40–55 cr | ₹50–70 cr |

Narrowing costs roughly **25–26% of SAM**. In exchange you get one coherent product, two aligned buyers instead of four, and no head-on fight with Clear.

---

## 4. The tension to be honest about, and how it resolves

In the sector scoring in `go-to-market-recommendation.md`, **software/IT scored lowest (15/22) for full internal audit** because the operational audit universe is thin: no plants, no inventory, no branch network. That scoring assumed classic operational internal audit.

**The resolution is control testing, which is the opposite case.**
- Many GCC parents are **US-listed, so SOX 404 control testing is performed from the India centre** †. Indian subsidiaries also need IFC testing under Sec 143(3)(i) †.
- Control testing is **document and system work**, so it needs no site visits. That fits the no-physical-audit constraint exactly.
- Control testing is highly **repetitive and rules-based**, which makes it the best possible target for automation.
- GCC finance and controllership teams are large, and this work is already centralised in India.

**So the positioning should lead with control testing, not operational internal audit:** *"Test every key control continuously, not a sample once a year, and hand your statutory auditor a pack they can rely on."*

**Where tech is still weak:** P2P, inventory and branch audits barely exist. Expect to sell roughly 60% control testing and audit prep, 40% operational internal audit (R2R, revenue, payroll, ITGC) in tech. Manufacturing is where the operational modules earn their keep, which is the Stage B argument.

---

## 5. Competitive set has changed

Dropping the tax engine moves you **out of Clear's path and into the audit-platform market**:

| Now competing with | Note |
|--------------------|------|
| **Wolters Kluwer TeamMate+** | The default at large Indian internal audit teams ([PKC](https://www.pkcindia.com/blog/internal-audit-tools/)) |
| **AuditBoard** | Cloud audit, risk and SOX platform; appears in Indian shortlists ([AI Accountant](https://www.aiaccountant.com/blog/ai-audit-tools-india-guide)) |
| **MetricStream** | 615 of its 716 staff are in India; about 6% of customers are Indian ([businessofgcc](https://www.businessofgcc.com/gcc-partners/metricstream), [iDatalabs](https://idatalabs.com/tech/products/metricstream)) |
| **Diligent HighBond (ACL)** | Audit management plus analytics ([Shanlax](https://www.shanlaxjournals.in/journals/index.php/sijash/article/download/10640/9034/)) |
| **eTHIC (NCS)** | Strong in Indian banking; less so in tech ([ncssoft.in](https://ncssoft.in/)) |
| **Audit360, Complinity, Risk Hawk** | Indian audit-workflow tools; reviews say analytics are limited ([Capterra](https://www.capterra.in/software/1094543/Audit360)) |
| **Big 4 platforms** (Omnia, Aura/Halo, Canvas/Helix, Clara) | Bundled with advisory ([Shanlax](https://www.shanlaxjournals.in/journals/index.php/sijash/article/download/10640/9034/)) |

**No longer a direct competitor:** Clear, Masters India, IRIS/Sovos, Litigation Shift. These become **integration partners** (pull their GST data) rather than rivals.

**Honest read:** this is a harder, more mature competitive set than the tax-tech one. The defensible wedge is **India mid-market + GCC, full-population testing, AI working papers**, where TeamMate+ and MetricStream are too expensive and Audit360-class tools are too shallow on analytics.

---

## 6. Revised build order

| Phase | Components |
|-------|-----------|
| **MVP (0–6 months)** | 1 (ERP + payroll connectors, trial-balance tie-out, audit-trail ingestion), 3 (evidence vault), 4 (test engine), **IFC/control testing: RCM library, design + operating-effectiveness testing, deficiency roll-up**, 7 (working papers with maker-checker), 9 (IFC report + PBC pack v1), 11 (basic security, India data residency) |
| **Phase 2 (6–12 months)** | 6 (R2R/journal testing, revenue for SaaS, payroll, ITGC/SoD, related parties), 8 (finding register with re-testing), GST/TDS audit areas and CARO statutory-dues schedules, auditor portal |
| **Phase 3 (12–24 months)** | 2 (risk assessment, annual plan, Audit Committee workflow), 10 (audit content library aligned to IIA 2025 and ICAI SIAs), full P2P/inventory modules for the manufacturing expansion, SOC 2 |

## 7. Re-aimed discovery questions

1. How many key controls do you test a year, and how long does one cycle take?
2. Do you run SOX 404 testing for the parent as well as Indian IFC? Who does it?
3. How many person-days go into the auditor's PBC list each year?
4. How many audit observations repeat year on year?
5. What do you use today — TeamMate, AuditBoard, Excel? What is missing?
6. Who signs: the Chief Audit Executive, the Controller, or both?
