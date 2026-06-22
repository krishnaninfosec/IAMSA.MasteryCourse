# IAM Solution Architect — Mastery Program

*From requirement to defensible solution — across Directory Services, Access Management, IGA, PAM, EPM, PKI and Identity Proofing, plus the cross-cutting CIAM and ISPM/ITDR/CIEM.*

> ### ▶ Live learning portal
> \*\*\[https://krishnaninfosec.github.io/IAMSA.MasteryCourse/](https://krishnaninfosec.github.io/IAMSA.MasteryCourse/)\*\*
>
> The portal is a self-contained learning system: the module-by-module course, \*\*active-recall flashcards with spaced repetition\*\*, quick self-checks, progress tracking and a fast-reference section. Your progress and review schedule are saved in your browser.

\---

## Contents

* [What this is](#what-this-is)
* [How the program works](#how-the-program-works)
* [The module syllabus](#the-module-syllabus)
* [How each module is taught (the template)](#how-each-module-is-taught-the-template)
* [Module 0 — Foundations](#module-0--foundations)
* [Where CIAM, ISPM and EPM fit](#where-ciam-ispm-and-epm-fit)
* [Product landscape by tower](#product-landscape-by-tower)
* [SI \& Transform delivery framework](#si--transform-delivery-framework)
* [Run / Managed Services framework](#run--managed-services-framework)
* [Estimation \& staffing primer](#estimation--staffing-primer)
* [Automation \& AI across IAM](#automation--ai-across-iam)
* [Licensing \& commercials primer](#licensing--commercials-primer)
* [The retention system](#the-retention-system)
* [Glossary](#glossary)
* [Sources](#sources)
* [Repository structure](#repository-structure)

\---

## What this is

A structured self-study program and reusable reference for becoming a strong **IAM Solution Architect** — someone who can read an RFP, extract scope, break it into activities, estimate effort, propose a staffing plan, lay it out phase-wise and role-wise, and **justify every number** to a sceptical reviewer.

It is built on three principles:

1. **Layer the foundation first.** Directory Services and Access Management underpin everything else, so they come before IGA and PAM.
2. **Learn each tower through one consistent lens.** Every tower module follows the same seven-part template, so comparison across towers becomes automatic.
3. **Learn estimation by doing it.** Each tower ends with a worked estimate, not just theory.

\---

## How the program works

You move through the material one tower at a time in short, repeatable sessions, keeping the curriculum open as the map. Each session:

* Teaches one sub-topic in plain language with an analogy and a worked example.
* Adds a **Solution Architect lens** (how the concept shows up when scoping and estimating) and an **"In an RFP, listen for:"** cue.
* Ends a module with a **reflection prompt** that runs a sample requirement end-to-end.
* Logs progress in the companion tracker so nothing is lost between sessions.

Navigation cues used during sessions: **`next`** to continue · **`go deeper`** to expand · **`estimate this`** to jump to a costing exercise.

\---



## The module syllabus

Fourteen modules, sequenced foundation-up. Hours are focused-learning planning figures.

|Module|Title|Hrs|Core outcome|
|-|-|-|-|
|**M0**|Foundations \& IAM operating model|3|Speak the language; map any requirement to a tower.|
|**M1**|Directory Services|4|Design the identity foundation and sync/consolidation approach.|
|**M2**|Access Management (SSO, MFA, Federation, Passwordless)|6|Scope app onboarding and authentication modernisation.|
|**M3**|Identity Governance \& Administration (IGA)|9|Scope JML, access requests, roles and certifications at scale.|
|**M4**|Privileged Access Management (PAM)|8|Scope vaulting, session control and JIT for privileged accounts.|
|**M4B**|Endpoint Privilege Management (EPM)|5|Scope local-admin removal, application control and elevation across endpoints.|
|**M5**|PKI \& Certificate Lifecycle Management|6|Scope CA build/modernisation and certificate automation.|
|**M6**|Identity Proofing \& Verification|4|Scope proofing to assurance levels and fraud controls.|
|**M7**|Customer Identity \& Access Management (CIAM)|5|Scope external/consumer identity, consent and scale.|
|**M8**|Identity Security Posture Management (ISPM, ITDR, CIEM)|4|Scope posture, threat detection and cloud entitlements across towers.|
|**M9**|Estimation, Staffing \& Project Planning|7|Build defensible estimates, pyramids and phase plans cross-tower.|
|**M10**|Run / Managed Services operating model|6|Design L1–L3 managed services with volume-reduction levers.|
|**M11**|Commercials \& Licensing|4|Compare licensing models and shape competitive pricing.|
|**M12**|RFP-to-Solution Capstone|6|Take a sample RFP end-to-end: scope → estimate → staffing → plan → justification.|

> SI/Transform, Run, automation/AI, licensing and estimation appear \*inside\* every tower module. Modules 9–11 are the cross-tower deep dives that consolidate those skills.

\---

## How each module is taught (the template)

Every tower module (M1–M8, including M4B) follows the same seven parts:

|#|Part|What it covers|
|-|-|-|
|1|Concepts \& capabilities|What the tower does, the building blocks, the vocabulary.|
|2|Product landscape|Leading products, strengths, and gotchas that change effort.|
|3|SI \& Transform|Build / migration / upgrade / integration — phases, WBS, effort drivers.|
|4|Run / Managed Services|L1–L3 operations, BAU, SLAs, operating model.|
|5|Automation \& AI|Where to cut volume and effort; where AI genuinely helps.|
|6|Licensing \& commercials|How products are licensed and the cost levers.|
|7|Worked estimation|A realistic mini-estimate: effort, roles, phase plan.|

And at the sub-topic level, the teaching shape is:

**Detailed explanation → Solution Architect lens → "In an RFP, listen for:" cue**, with each module closing on a **reflection prompt**.

\---

## Module 0 — Foundations

The shape of the whole field before going tower by tower. These six ideas are the lens for reading every RFP.

### 1\. What IAM is, and authentication vs authorization

IAM is a discipline, not a product: managing digital identities and what they may do across every system. Two core verbs sit at its heart — **authentication** ("are you who you say you are?") and **authorization** ("what are you allowed to do?") — wrapped in **administration** and **governance**. A clean model is four jobs: *authenticate, authorize, administer, govern*. Identities come in three families: workforce, external, and non-human (service accounts, workloads, bots, AI agents — the fastest-growing).

> \*\*Solution Architect lens\*\* — Sort every RFP line into authenticate / authorize / administer / govern. That sort tells you which towers are in play and how effort splits before you ever estimate.
>
> \*\*In an RFP, listen for:\*\* "single sign-on", "MFA", "joiner/leaver", "access review", "least privilege", "audit finding".

### 2\. The identity lifecycle: Joiner – Mover – Leaver (JML)

Every identity moves through **Joiner → Mover → Leaver**. Joiner: birthright access on day one. Mover: old access removed as new is granted (where privilege creep happens). Leaver: prompt revocation — the most common audit finding when it fails. An authoritative source (usually HR) triggers JML events; its data quality decides how much can be automated.

> \*\*Solution Architect lens\*\* — Most IGA scope and run volume is JML at scale. A client's JML maturity is the fastest gauge of problem size and automation upside.
>
> \*\*In an RFP, listen for:\*\* "manual onboarding", "leavers still have access", "spreadsheet-driven", "termination delays".

### 3\. The six towers and how they interconnect

* **Directory Services** — the foundation; authoritative store of identities and attributes.
* **Access Management** — runtime login: SSO, MFA, federation.
* **IGA** — "should this person have this access?": provisioning, requests, roles, certifications.
* **PAM** — the vault for powerful accounts: vaulting, session control, JIT.
* **PKI / CLM** — certificates and keys for machine identity and encryption.
* **Identity Proofing** — "is this real person who they claim to be?" at enrolment.

They stack: Proofing verifies → Directory stores → IGA provisions → Access Management authenticates daily → PAM elevates when needed → PKI secures machine-to-machine. *One hire, one day, six towers.*

> \*\*Solution Architect lens\*\* — Map each requirement to a tower before estimating. A multi-tower RFP is not the sum of independent builds; the dependencies (directory before IGA, AM before CIAM) drive sequencing and integration effort.

### 4\. The standards you must recognise

|Standard|What it does|
|-|-|
|SAML 2.0|XML browser-SSO federation; dominant in enterprise apps.|
|OIDC / OAuth 2.0|Modern token authentication (OIDC) and delegated authorization (OAuth).|
|SCIM|Automated provisioning/de-provisioning to SaaS.|
|LDAP|Directory query/modify protocol.|
|FIDO2 / WebAuthn|Phishing-resistant passwordless (passkeys, security keys).|
|X.509|Certificate format underpinning PKI and TLS.|
|NIST SP 800-63-4|Assurance levels for proofing (IAL), authentication (AAL), federation (FAL).|

> \*\*Solution Architect lens\*\* — The protocol an app speaks decides its onboarding cost. Pull the protocol split from the app inventory first — that ratio is the parametric multiplier behind AM and IGA estimates.
>
> \*\*In an RFP, listen for:\*\* "header-based auth", "Kerberos", "no API" → expensive; "supports SAML/OIDC/SCIM" → cheap.

### 5\. NIST 800-63 assurance levels (IAL / AAL / FAL)

NIST SP 800-63-4 (finalised mid-2025) defines graded assurance: **IAL** (proofing), **AAL** (authentication), **FAL** (federation). Revision 4 restructures proofing into four types and adds controls for injection attacks and forged media (deepfakes), plus support for passkeys and wallets.

> \*\*Solution Architect lens\*\* — Assurance levels are a scoping signal, not a checkbox. A high IAL/AAL requirement cascades into stronger proofing, phishing-resistant MFA and extra evidence/testing effort. Price the cascade, not just the line.

### 6\. Capability towers vs delivery functions (the matrix)

Towers are the **"what"** (vertical capabilities). **Delivery functions** are the **"how"** (horizontal disciplines) that cut across every tower:

|Delivery function|Heaviest in|
|-|-|
|Architecture \& design|Design phase; Solution Architect band|
|Business analysis|Discovery \& Design; run change requests|
|Engineering / build|Build \& use-case phases; L3 in run|
|Testing / QA|Unit / SIT / UAT; regression in run|
|Project / delivery management|All phases (PMO overlay)|
|Operations / run|Entire run framework (L1–L3, BAU)|
|Audit, risk \& compliance|Design controls; run evidence; IGA/ISPM capability|
|Reporting \& analytics|Design requirements; run reporting; IGA/ISPM analytics|

> \*\*Solution Architect lens\*\* — You never staff a tower in isolation — you staff the \*\*matrix\*\*. Your \*role-wise view\* is bands (seniority) × functions (discipline); your \*phase-wise view\* is those functions over time. Read tower names for scope; read team/function names for delivery shape and run pricing.

> \*\*Reflection\*\* — Take an RFP line such as \*"automate joiner and leaver access for 12,000 staff and pass our next access audit."\* Run it through the four jobs, place it in towers, name the one number that drives the estimate, and say which delivery functions you'd staff in discovery.

\---

## Where CIAM, ISPM and EPM fit

These three are frequently miscategorised. Getting them right signals you understand the field, not just the products.

* **CIAM** is **not a new capability tower** — it's an *applied cross-tower domain*: Access Management + Directory + Identity Proofing (plus light governance) aimed at external/consumer identities at scale, with usage-based (per-MAU) licensing. Taught as **M7**.
* **ISPM** is **not a tower** — it's a *cross-cutting posture layer* over all towers, alongside **ITDR** (reactive threat detection/response) and **CIEM** (cloud entitlement management). No standalone analyst quadrant; it reads from the towers you are already building. Taught as **M8**.
* **EPM** is the **endpoint arm of the privileged-access family** — privilege elevation and delegation (PEDM) applied to endpoints: removing standing local admin and elevating per-application. Best scoped *with* PAM. Taught as **M4B**.

\---

## Product landscape by tower

*Positions summarise 2025–2026 analyst coverage; not endorsements. Current as of mid-2026.*

### Directory Services

Microsoft Entra ID (formerly Azure AD) · Active Directory DS · Okta Universal Directory · Ping (PingDirectory) · Oracle Unified/Internet Directory · Radiant Logic (virtual directory) · OpenLDAP / 389 DS.

### Access Management

**Microsoft Entra ID · Okta · Ping Identity** (leaders) · IBM Security Verify · Cisco Duo (MFA) · RSA SecurID.

### IGA

**SailPoint · Saviynt** (leaders) · Microsoft Entra ID Governance · One Identity · Omada · Oracle Identity Governance · SAP / IBM.

### PAM

**CyberArk · BeyondTrust · Delinea** (leaders) · One Identity Safeguard · Wallix / ARCON · ManageEngine PAM360 · Saviynt PAM.

### Endpoint Privilege Management (EPM)

**CyberArk EPM · BeyondTrust Endpoint Privilege Management · Delinea Privilege Manager** (leaders) · ThreatLocker · Admin By Request · Microsoft Intune EPM (Windows-only today) · Securden / Action1 / ManageEngine.

### PKI \& CLM

Microsoft AD CS · CyberArk Certificate Manager (formerly Venafi) · Keyfactor · DigiCert · AppViewX · Sectigo / Entrust · HashiCorp Vault PKI.

### Identity Proofing

Onfido (now Entrust) · Jumio · Socure · ID.me · Incode / iProov / Persona / AU10TIX · Microsoft Entra Verified ID.

### CIAM

**Okta Customer Identity / Auth0 · Ping (+ ForgeRock) · Microsoft Entra External ID** (leaders) · Thales OneWelcome · Transmit Security / SAP CDC · AWS Cognito / LoginRadius / Frontegg / Descope.

### ISPM / ITDR / CIEM

Microsoft (Entra posture + ITDR) · Silverfort · CrowdStrike Falcon Identity · Radiant Logic · SailPoint / Saviynt (ISPM) / Veza.

\---

## SI \& Transform delivery framework

**Project types:** greenfield/new build · migration · upgrade · new feature · integration/onboarding · enhancement.

**Phase model (the reusable spine):**

1. Requirements \& Discovery
2. Design
3. Build \& Setup
4. Use-case Implementation
5. Unit Testing
6. System Integration Testing (SIT)
7. User Acceptance Testing (UAT)
8. Deployment \& Go-Live
9. Hypercare

**Environments:** price at least **Non-Production and Production** — every config, connector and use case must be promoted and re-verified, so environment count multiplies build/test effort.

**Effort drivers:** count and protocol-mix of apps/accounts/certificates · number and complexity of use cases · environments and HA/DR · source-data quality · standards-based vs custom integration · compliance/audit scope · migration data volume.

\---

## Run / Managed Services framework

|Tier|Nature|IAM examples|
|-|-|-|
|**L1**|First response; scripted, high-volume|Password resets, access-request status, unlocks, triage.|
|**L2**|Config \& known-problem resolution|Connector/workflow fixes, standard app onboarding, campaign support.|
|**L3**|Deep expertise / engineering|Complex defects, new connectors, tuning, vendor escalation.|

**BAU beyond L1–L3:** application/account onboarding · certification campaigns · role \& SoD upkeep · JML exception handling · certificate/credential rotation · patching \& upgrades · audit support \& evidence · service reporting \& SLA management.

**Operating-model levers:** shift model (8×5 / 24×7 / follow-the-sun) · onshore/nearshore/offshore mix · SLA tiers · documented volume baselines.

\---

## Estimation \& staffing primer

**Four approaches:** Bottom-up (WBS — most defensible) · Parametric (unit × count) · Analogous (scale from past) · Top-down (% allocation). *Build bottom-up, cross-check with the others; where they diverge, you've found an assumption worth examining.*

**Staffing pyramid (bands):** Solution Architect/Lead → Senior Engineer/Consultant → Engineer/Developer → Analyst/Offshore. A **staffing plan = bands (seniority) × functions (discipline)** — that cross-tabulation is your role-wise view.

**The estimate-to-justification chain — keep it traceable:**

> \*\*Requirement → Scope item → Activities (WBS) → Effort driver \& assumption → Effort → Role split → FTE → Cost → Phase plan\*\*

If a reviewer challenges a number, walk back up the chain to the assumption and the driver.

\---

## Automation \& AI across IAM

* **Volume reduction at L1** — self-service password reset, self-service access requests, chatbot deflection.
* **Workflow automation** — automated JML, birthright provisioning/de-provisioning.
* **AI-assisted governance** — outlier/peer-group analytics; certifications focus on the few anomalies.
* **Intelligent recommendations** — role mining and access recommendations.
* **Certificate \& credential automation** — discovery, renewal, rotation (essential under shrinking cert lifetimes).
* **Delivery productivity** — AI-assisted connector/config/test generation, documentation, RFP analysis.
* **Non-human \& agentic identity** — governing service accounts, workloads and AI agents with the same rigour as humans.

> Quantify automation twice in a proposal: as a productivity factor that reduces effort/price, and as a client benefit (fewer tickets, faster onboarding, lower audit risk).

\---

## Licensing \& commercials primer

|Model|What to watch|
|-|-|
|Per identity / per user|Common in IGA and AM; watch contractors, B2B, non-human counts.|
|Per managed/privileged account|Common in PAM; vaulted accounts and sessions drive cost.|
|Per endpoint / per user|Common in EPM; endpoint count and OS mix drive cost.|
|Per certificate / per CA|PKI/CLM; shrinking lifetimes raise volumes.|
|Per transaction / verification|Identity proofing; scales with onboarding volume.|
|Per MAU / authentication|CIAM; cost swings on traffic, not headcount.|
|Module / capability-based|Many platforms price provisioning, governance, analytics separately.|
|SaaS vs perpetual + support|SaaS shifts to opex and includes upgrades; on-prem adds infra/upgrade projects.|

> Implementation, training and run usually dwarf initial licensing in total cost of ownership — so effort optimisation often beats licence haggling.

\---

## The retention system

The portal is built to defeat the "I forget the early modules" problem with three evidence-based mechanics:

* **Active recall** — flashcards you answer before flipping, not passages you re-read.
* **Spaced repetition** — a Leitner schedule (intervals of 1 / 3 / 7 / 16 / 35 days) resurfaces a card right before you'd forget it; new cards only enter the review queue once you've studied them.
* **Self-checks** — quick retrieval-practice questions with instant feedback.

\---

## Glossary

|Term|Meaning|
|-|-|
|AAL / IAL / FAL|Authentication / Identity / Federation Assurance Levels (NIST SP 800-63-4).|
|BAU|Business as usual — recurring run activities.|
|CIAM|Customer IAM — identity for external/consumer users.|
|CIEM|Cloud Infrastructure Entitlement Management.|
|CLM|Certificate Lifecycle Management.|
|EPM|Endpoint Privilege Management — remove local admin, elevate apps just-in-time.|
|IGA|Identity Governance \& Administration.|
|ISPM|Identity Security Posture Management.|
|ITDR|Identity Threat Detection \& Response.|
|JIT|Just-in-time access.|
|JML|Joiner-Mover-Leaver.|
|MAU|Monthly Active Users — common CIAM licensing metric.|
|NHI|Non-human identity — service accounts, workloads, bots, agents.|
|PAM|Privileged Access Management.|
|PEDM|Privilege Elevation \& Delegation Management (EPM is PEDM at the endpoint).|
|PKI|Public Key Infrastructure.|
|RBAC / ABAC|Role- / Attribute-based access control.|
|SCIM|System for Cross-domain Identity Management.|
|SoD|Segregation of Duties.|
|SSO|Single Sign-On.|
|WBS|Work Breakdown Structure.|
|ZSP|Zero Standing Privilege.|

\---

## Sources
 
- NIST SP 800-63-4, *Digital Identity Guidelines* (finalised 2025).
- Gartner Magic Quadrants 2025: Access Management; Identity Governance & Administration; Privileged Access Management.
- CA/Browser Forum — phased reduction of TLS certificate lifetimes.
- Vendor documentation: Microsoft Entra, Okta, Ping, SailPoint, Saviynt, CyberArk, BeyondTrust, Delinea, ThreatLocker, Keyfactor, DigiCert, AppViewX, Entrust.

\---
## Repository structure

```
IAMSA.MasteryCourse/
├── index.html                          # the learning portal (served by GitHub Pages)
├── README.md                           # this file
├── Resources/
    ├── IAM\_Mastery\_Curriculum.docx     # full curriculum \& reference guide
    ├── IAM\_Mastery\_Tracker.xlsx        # progress tracker + product landscape + estimation cheat-sheet
    └── IAM\_Discovery\_Questionnaire.xlsx # RFP discovery questionnaire (per-tower + volume metrics)

\---
