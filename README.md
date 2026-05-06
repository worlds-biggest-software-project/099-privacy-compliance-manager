# Privacy Compliance Manager

> Part of the [worlds-biggest-software-project](https://github.com/worlds-biggest-software-project) initiative.
>
> An AI-native, open-source privacy compliance platform that unifies GDPR/CCPA data mapping, DSR workflow, and consent management without enterprise-tier pricing or vendor lock-in.

Privacy Compliance Manager is a self-hostable platform for privacy, compliance, and engineering teams that need to operationalise GDPR, CCPA/CPRA, LGPD, India DPDP, and 25+ US state privacy laws. It combines automated data discovery, multi-jurisdiction Data Subject Request (DSR) fulfilment, IAB TCF v2.2-compatible consent management, and Article 30 Records of Processing Activities (RoPA) into a single coherent framework — addressing the gap left by expensive enterprise SaaS and the absence of any mature open-source equivalent.

---

## Why Privacy Compliance Manager?

- **No mature open-source platform exists.** OpenDSR is a protocol specification only; there is no functional OSS privacy compliance platform with UI, data mapping, consent management, and DSR automation.
- **Mid-market is priced out.** OneTrust enforces a $10,000 minimum ACV (March 2026); TrustArc reaches $50K–$100K+/year for 10+ domains; Securiti.ai runs $50K–$500K+/year. Organisations between SMB tools and enterprise platforms have no good option.
- **Manual RoPA is the industry's universal failure mode.** Most organisations maintain Article 30 records as perpetually-stale spreadsheets. Continuous, automated data inventory from live systems is an unmet need across every market segment.
- **Data residency rules out SaaS for many buyers.** Healthcare, financial services, government, and defence organisations cannot send sensitive compliance data to third-party SaaS — there is no self-hostable alternative today.
- **AI Act compliance is not addressed by legacy tools.** Privacy platforms built before 2024 were not designed for EU AI Act and NIST AI RMF obligations that intersect with traditional privacy compliance.

---

## Key Features

### Consent Management

- Cookie consent management with auto-domain scanning and configurable banners
- IAB TCF v2.2-compatible consent signal management for programmatic advertising
- Preference centre with granular per-purpose and per-vendor controls
- Immutable consent audit trail recording grant, change, and withdrawal events per data subject
- Real-time consent signal propagation to downstream data processors and MarTech vendors

### Data Subject Request (DSR) Workflow

- Branded self-service DSAR intake portal with identity verification
- Multi-jurisdiction routing applying the correct statutory deadline and response template based on requester jurisdiction
- Automated data system queries across connected stores for access, deletion, correction, and portability requests
- Redaction, response assembly, and secure delivery with full audit trail
- Statutory deadline tracking for GDPR (30 days), CCPA (45 days), and 25+ US state law variants

### Data Inventory & RoPA

- Automated data discovery from live system connections rather than manual questionnaires
- Personal data classification by GDPR Article 9 special categories and CCPA sensitive data definitions
- Continuous, auditable Article 30 Record of Processing Activities maintained without manual curation
- Visual data flow diagrams showing movement between systems, third parties, and geographies
- Connector library for common data stores (PostgreSQL, MySQL, MongoDB, Salesforce, Snowflake, BigQuery, AWS S3)

### Assessments & Vendor Risk

- Privacy Impact Assessment (PIA) and DPIA workflows with configurable templates
- Vendor and data processor management with Data Processing Agreement (DPA) tracking
- Privacy risk scoring for the supply chain
- Privacy notice and policy management with version history and jurisdiction-specific variants

### AI Governance & Multi-Regulation Posture

- EU AI Act impact assessments and high-risk AI system inventory
- AI training data transparency documentation aligned to NIST AI RMF
- Cross-regulation compliance dashboard covering GDPR, CCPA/CPRA, LGPD, India DPDP, and US state laws simultaneously
- Regulatory change monitoring across 130+ jurisdictions with programme update alerts

---

## AI-Native Advantage

AI is foundational rather than additive. Continuous classification agents scan connected systems and maintain a live RoPA without manual curation, addressing the most universal operational gap in GDPR Article 30 compliance. DSR fulfilment runs as an autonomous agent that determines applicable laws from the requester's jurisdiction, queries connected systems, applies redactions, and assembles compliant response packages within statutory deadlines. Consent propagation auditing detects processing-without-consent violations by reconciling active processing against the consent audit trail across the connected estate — providing genuine compliance assurance rather than compliance theatre.

---

## Tech Stack & Deployment

- **Self-hosted first**, with cloud and hybrid deployment modes; designed for organisations with strict data residency requirements (healthcare, financial services, government, defence).
- **Open standards**: IAB TCF v2.2 for consent signals; OpenDSR (Apache Licence 2.0) for inter-organisation DSR interoperability; ISO 29100 and ISO 27701 alignment; NIST Privacy Framework 1.0 mapping.
- **Pluggable connector library** for PostgreSQL, MySQL, MongoDB, Salesforce, Snowflake, BigQuery, AWS S3, SharePoint, and Google Workspace, with a REST API for custom integrations.
- **API-first** architecture so engineering teams can embed privacy enforcement into product data flows alongside UI-driven configuration for compliance teams.

---

## Market Context

The broad Privacy Management Software market is projected to grow from **$4.80B in 2026 to $27.48B by 2033** at a **28.4% CAGR** (SkyQuestt), driven by 130+ countries enacting privacy legislation and 25+ active US state privacy laws. Incumbent pricing ranges from ~$10/month/domain (Secure Privacy) and $29–$199/month (Enzuzo) at the SMB end, through $30K–$150K/year (DataGrail) in mid-market, up to $50K–$500K+/year for enterprise unified platforms (Securiti.ai). Primary buyers are Chief Privacy Officers, Data Protection Officers, and legal/compliance teams at mid-market and enterprise organisations — particularly those priced out of OneTrust's $10K minimum and unable to use SaaS-only tools due to data residency obligations.

---

## Project Status

> This project is in the **research and specification phase**.  
> Contributions, feedback, and domain expertise are welcome.

---

## Contributing

We welcome contributions from developers, domain experts, and potential users.
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Important:** All contributions must be your own original work or clearly attributed
open-source material with a compatible licence. Copyright infringement and licence
violations will not be tolerated and will result in immediate removal of the offending
contribution. If you are unsure whether a piece of code, text, or other material is
safe to contribute, open an issue and ask before submitting.

---

## Licence

Licence to be determined. See [discussion](#) for context.
