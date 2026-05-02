# Privacy Compliance Manager — Feature & Functionality Survey

> Candidate #99 · Researched: 2026-05-02

## Solutions Analysed

| Tool | Type | Licence / Model | URL |
|------|------|-----------------|-----|
| OneTrust | Commercial SaaS | Proprietary; $10K minimum ACV | https://www.onetrust.com |
| TrustArc | Commercial SaaS | Proprietary; $15K–$100K+/yr | https://trustarc.com |
| Securiti.ai | Commercial SaaS | Proprietary; $50K–$500K+/yr | https://www.securiti.ai |
| DataGrail | Commercial SaaS | Proprietary; $30K–$150K/yr | https://www.datagrail.io |
| Transcend | Commercial SaaS | Proprietary; custom | https://transcend.io |
| Osano | Commercial SaaS | Proprietary; ~$199/mo (historical) | https://www.osano.com |
| Enzuzo | Commercial SaaS | Proprietary; $29–$199/mo | https://www.enzuzo.com |
| Exterro Privacy | Commercial SaaS | Proprietary; bundled with Exterro | https://www.exterro.com |
| OpenDSR | Open source (protocol) | Open specification; Apache Licence 2.0 implementations | https://opendsr.org |
| Secure Privacy | Commercial SaaS | Proprietary; from $10/mo/domain | https://secureprivacy.ai |

## Feature Analysis by Solution

### OneTrust

**Core features**
- Data mapping and processing activity records: automated and manual tools for building and maintaining Article 30 Records of Processing Activities (RoPA), with visual data flow diagrams showing how personal data moves between systems, third parties, and geographies
- DSR (Data Subject Request) automation: full lifecycle management from intake through identity verification, data discovery, redaction, and secure response delivery across GDPR, CPRA, LGPD, and 25+ US state laws
- Consent Management Platform (CMP): cookie consent banner management, preference centre, and IAB TCF v2.2-compliant consent signal management for digital advertising ecosystems
- Vendor and third-party risk management: privacy impact assessments, data processing agreements, and vendor risk scoring for the supply chain
- Privacy Impact Assessment (PIA) / DPIA workflows: templated and configurable risk assessments for new processing activities

**Differentiating features**
- Broadest module coverage in the market: the only platform that covers privacy, security, GRC, ESG, and ethics in a unified product portfolio
- Privacy Automation combining DSR, consent, data mapping, and compliance in a single platform experience with a unified data inventory
- 2026 evolution: moving from CMP-only to full governance stack — consent management is positioned as the entry point to a broader compliance programme, not the endpoint
- Largest partner and integration ecosystem in privacy compliance

**UX patterns**
- Workflow builder for configuring DSR routing, approval chains, and automated data system queries without engineering resources
- Data inventory heat maps showing data flows and third-party data sharing relationships visually
- Compliance posture dashboard with jurisdiction-by-jurisdiction readiness indicators

**Integration points**
- 350+ pre-built connectors to enterprise data systems (Salesforce, Workday, AWS S3, Google BigQuery, Snowflake, PostgreSQL, and others)
- IAB TCF v2.2 publisher and vendor integrations for programmatic advertising consent
- Legal hold and e-discovery integration with Exterro

**Known gaps**
- $10,000 minimum ACV as of March 2026; effectively excludes SMBs and many mid-market organisations
- Complex implementation; typically requires weeks of configuration and often professional services engagement
- Some modules feel like separate products loosely bundled; UX consistency across the platform can be inconsistent
- Pricing opacity drives buyers to alternatives; many mid-market buyers cite Enzuzo and Osano specifically as "OneTrust without the price"

**Licence / IP notes**
- Proprietary SaaS; $5.1B valuation (Insight Partners, 2021)
- No open-source components
- IAB TCF v2.2 integration requires IAB Europe membership and vendor registration; not freely deployable without compliance with IAB framework terms
- EU-US Data Privacy Framework certifications and Standard Contractual Clauses documented for EU deployments

---

### TrustArc

**Core features**
- Cookie consent management with per-domain configuration, auto-scanning for cookie categories, and IAB TCF v2.2 compliance
- CCPA and GDPR compliance assessments with templated questionnaires and gap analysis reporting
- Data inventory and processing activity records with manual and semi-automated data mapping
- Vendor risk management with privacy-specific assessment templates for data processors
- Consent analytics showing consent rates, opt-out trends, and jurisdiction-level breakdown

**Differentiating features**
- Strong privacy compliance pedigree — TrustArc (formerly TRUSTe) has operated since 1997 and is one of the most established brands in privacy compliance
- Cost-effective alternative to OneTrust for organisations needing solid GDPR/CCPA coverage without enterprise-tier pricing
- Domain-based pricing model makes budget predictable for organisations with defined digital property portfolios

**UX patterns**
- Compliance manager dashboard with task lists, upcoming deadlines, and regulatory change alerts
- Cookie scanner that automatically identifies and categorises cookies on scanned domains for consent configuration

**Integration points**
- Standard HRIS and CRM integrations for DSR data discovery
- Programmatic advertising platform integrations for TCF consent propagation

**Known gaps**
- Narrower GRC scope than OneTrust; vendor risk and security management less mature
- UI and UX in some modules feels dated compared with newer entrants
- AI-powered data discovery and classification less mature than Securiti.ai
- Pricing for 10+ domains ($50K–$100K+/year) approaches OneTrust territory

**Licence / IP notes**
- Proprietary SaaS; privately held (PE-backed)
- No open-source components

---

### Securiti.ai

**Core features**
- AI-powered data discovery and classification across structured databases, unstructured file stores, cloud storage, SaaS applications, and email — automatically identifying personal data by category (GDPR Art. 9 special categories, CCPA sensitive data)
- Unified privacy, security posture management, and AI governance platform — the only platform combining traditional privacy compliance with emerging AI governance obligations
- Automated RoPA generation from discovered data rather than manual questionnaire completion
- DSR fulfillment automation with connectors to 2,000+ data systems for automated data retrieval and redaction
- AI governance module: AI impact assessments, AI training data transparency documentation, and EU AI Act compliance workflows

**Differentiating features**
- Data discovery automation that scans live data systems continuously rather than relying on manual data mapping — directly addressing the fundamental operational gap in GDPR Article 30 compliance
- Unified privacy + AI governance: the only major platform designed from the outset to handle both traditional privacy regulation (GDPR/CCPA) and emerging AI regulation (EU AI Act, NIST AI RMF) in a single framework
- Scale: handles petabyte-scale data classification across hybrid multi-cloud environments
- PrivacyOps approach: operationalising privacy compliance as a continuous automated process rather than a point-in-time audit exercise

**UX patterns**
- Data intelligence graph visualising personal data locations, categories, and flows across the enterprise data landscape
- Command centre dashboard showing compliance posture across multiple regulations simultaneously
- Automated DSR orchestration that triggers data system queries, collects responses, applies redactions, and assembles response packages without manual coordination

**Integration points**
- 2,000+ connectors to cloud data stores (AWS, Azure, GCP), SaaS applications (Salesforce, Workday, ServiceNow), databases (PostgreSQL, MySQL, MongoDB, Snowflake, BigQuery), and file stores (SharePoint, S3, OneDrive)
- SIEM and SOAR integrations for security event correlation
- AI model registry integrations for AI governance

**Known gaps**
- Enterprise-only pricing ($50K–$500K+/year); no accessible tier for mid-market or SMB
- Complex implementation requiring significant data systems integration work
- AI governance module is newer and still maturing
- Heavy platform; organisations seeking lightweight consent management should look elsewhere

**Licence / IP notes**
- Proprietary SaaS; $1B+ valuation (General Atlantic, 2022)
- AI-powered data classification uses proprietary ML models; classification accuracy methodology not publicly documented
- EU AI Act compliance obligations apply to the platform's own AI classification capabilities as an AI system used in processing

---

### DataGrail

**Core features**
- DSR automation with the deepest integration library of any DSR-focused platform: 2,000+ pre-built connectors enable automated data discovery, retrieval, and response fulfilment across data systems
- Data discovery and mapping maintained continuously from live system connections, not manual questionnaires
- DSR portal with branded self-service interface for data subjects to submit requests
- Signal propagation: consent preference changes propagated to downstream data systems in real time

**Differentiating features**
- Best-in-class DSR automation by integration breadth; when a data subject requests deletion, DataGrail queries all connected systems simultaneously and orchestrates deletion across the entire data estate
- Trusted by major technology companies (Patreon, Grindr, and others); demonstrated capability at consumer-scale DSR volumes
- Privacy Signal Propagation: unique capability to relay preference changes (opt-out of sale, deletion requests) to downstream vendors in real time

**UX patterns**
- Data subject-facing portal with clean UX for submitting access, deletion, and correction requests
- Compliance team dashboard showing DSR volume, fulfilment timelines, and jurisdiction breakdown
- Integration health monitoring showing which connected systems are responding to automated queries

**Integration points**
- 2,000+ integrations with product databases (PostgreSQL, MySQL, MongoDB), cloud data stores, CRMs, marketing platforms, and data warehouses
- REST API for custom integration with proprietary internal systems
- Consent Management Platform integrations for signal reception

**Known gaps**
- Primarily a DSR and data discovery tool; not a full-stack privacy compliance platform
- Consent management and cookie banner management require separate tools
- Privacy impact assessments and vendor risk management not included
- Pricing ($30K–$150K/year) not accessible to SMBs

**Licence / IP notes**
- Proprietary SaaS; Silver Lake Waterman-backed ($30M Series B, 2022)
- No open-source components

---

### Transcend

**Core features**
- Privacy infrastructure platform with API-first architecture enabling technical teams to build DSR automation directly into their product data flows
- Consent management with granular preference management and consent signal propagation to downstream services
- Sombra: Transcend's privacy gateway that intercepts data flows and enforces privacy policies at the infrastructure level rather than application level
- Data discovery via query of connected systems for DSR fulfilment without data centralisation

**Differentiating features**
- Developer-first approach: Transcend is the only major privacy platform built primarily for engineering teams rather than compliance teams; integration is via SDK and API rather than UI configuration
- Privacy-at-infrastructure-level via Sombra — enforcement happens in the data flow, not after the fact, making compliance structurally embedded rather than layered on top
- Preferred by technical teams at SaaS companies who want to build privacy into their product architecture, not bolt it on

**UX patterns**
- Developer documentation-first; primary interface is API reference and SDK documentation
- Compliance team dashboard for monitoring DSR fulfilment status and consent analytics

**Integration points**
- SDK for web, mobile, and backend integration
- GraphQL and REST API for custom data system integration
- All major web and mobile advertising platforms for consent signal propagation

**Known gaps**
- Not suitable for non-technical compliance teams; requires engineering resources to implement and maintain
- No cookie banner out-of-the-box without engineering integration
- Limited vendor risk and PIA tooling
- Less suitable for organisations without strong engineering capabilities

**Licence / IP notes**
- Proprietary SaaS; Accel-backed ($25M Series B, 2022)
- No open-source components of note
- OpenDSR protocol specification (which Transcend co-authored) is open under Apache Licence 2.0; the Transcend implementation itself is proprietary

---

### Enzuzo

**Core features**
- Cookie consent management with auto-scanning, categorisation, and IAB TCF v2.2-compatible banner generation
- Privacy policy generator producing jurisdiction-specific policy text from a questionnaire workflow
- DSAR management with a branded request portal and manual fulfilment workflow
- Shopify and e-commerce platform integrations for small business compliance

**Differentiating features**
- Most affordable all-in-one privacy compliance platform for SMBs ($29–$199/month)
- Shopify-native integration making it the default choice for Shopify merchants requiring GDPR/CCPA cookie compliance
- Simple UX designed for non-compliance professionals; no legal or technical expertise required for deployment
- Full implementation typically achievable in under four weeks for SMBs

**UX patterns**
- Wizard-based setup guiding users through domain scanning, banner configuration, and policy generation
- Dashboard showing cookie consent rates, DSR request log, and policy version history

**Integration points**
- Shopify, WooCommerce, and Squarespace native app integrations
- Google Tag Manager for consent signal integration with analytics and advertising tags

**Known gaps**
- No enterprise data mapping, automated data discovery, or Article 30 RoPA management
- DSR fulfilment is manual; no automated data system querying
- Not suitable for organisations with complex data architectures, multiple subsidiaries, or enterprise compliance requirements

**Licence / IP notes**
- Proprietary SaaS; no open-source components

---

### OpenDSR (Protocol)

**Core features**
- Open API specification enabling interoperable Data Subject Request processing between a data controller and its data processors
- Standardised request types (access, deletion, portability) with defined JSON schemas
- Cryptographic request signing for authenticity verification
- Status callback mechanism for processors to report fulfilment status back to the controller

**Differentiating features**
- The only open standard for DSR workflow interoperability; co-authored by major technology companies (mParticle, Segment, Amplitude, and others)
- Apache Licence 2.0: permissive, patent-grant included; implementable in any commercial or open-source product without restriction

**UX patterns**
- Protocol specification only; no reference UI implementation
- Swagger/OpenAPI specification for developer implementation

**Integration points**
- Implementable on any platform that can make HTTP requests and process JSON

**Known gaps**
- Protocol specification only; no functional open-source implementation of a complete privacy compliance platform
- No UI, data mapping, consent management, or PIA tooling
- Requires significant custom development to build a usable system from the specification

**Licence / IP notes**
- Apache Licence 2.0 (permissive); patent licence grant included; freely implementable in commercial products
- No known patent encumbrances on DSR workflow patterns

---

## Cross-Cutting Feature Themes

### Table-Stakes Features
- Cookie consent management with auto-scanning, banner configuration, and IAB TCF v2.2 compliance for programmatic advertising
- DSAR intake portal with branded self-service interface for data subject request submission
- DSR lifecycle management: identity verification, data discovery, response assembly, delivery, and audit trail
- Data processing inventory / RoPA management aligned to GDPR Article 30
- Privacy policy and notice management with version history and jurisdiction-specific variants
- Consent audit trail: immutable record of consent given, changed, and withdrawn per data subject
- Role-based access control and SOC 2 Type II certification

### Differentiating Features
- Automated data discovery from live system connections rather than manual questionnaire-based data mapping
- Real-time consent signal propagation to downstream data processors and MarTech vendors
- Multi-jurisdiction DSR routing that applies the correct legal deadline and response template based on the requester's jurisdiction
- AI governance integration managing EU AI Act impact assessments alongside traditional privacy compliance
- Privacy-at-infrastructure-level enforcement (Transcend Sombra model) embedding compliance in data flows
- Cross-regulation compliance dashboard showing simultaneous posture against GDPR, CCPA/CPRA, LGPD, India DPDP, and 25+ US state laws

### Underserved Areas / Opportunities
- No mature open-source privacy compliance platform of any kind exists; OpenDSR is a protocol spec only
- Mid-market organisations priced out of OneTrust ($10K+ minimum) and without the technical capacity for Transcend
- AI governance and traditional privacy compliance in a unified framework (Securiti.ai is pioneering this but at enterprise-only pricing)
- Automated RoPA maintenance from live system scanning without manual questionnaire dependency
- Privacy compliance for organisations in jurisdictions with strong data residency requirements (government, healthcare, defence) that cannot use SaaS-only tools

### AI-Augmentation Candidates
- Continuous data inventory: AI that scans connected systems, classifies personal data by GDPR Article 9 / CCPA sensitive data category, and maintains a live, auditable RoPA without human curation
- Multi-jurisdiction DSR routing and fulfilment: AI agent that receives a DSR, determines applicable laws, queries connected systems, generates a redacted response package, and delivers it within the applicable statutory deadline
- Consent signal propagation audit: AI that detects processing-without-consent violations by comparing active processing against the consent audit trail across all connected systems
- AI Act compliance module: automated AI impact assessments, training data transparency documentation, and high-risk AI system registration workflows
- Regulatory change detection: AI monitoring of legislative and enforcement updates across 130+ jurisdictions that automatically flags compliance programme changes required

---

## Legal & IP Summary

- No mature open-source privacy compliance platform exists; OpenDSR (Apache Licence 2.0) is the only open artefact of significance and it is a protocol specification, not a functional platform
- GDPR (EU, 2018): foundational privacy regulation driving the entire market; Article 30 (RoPA), Article 17 (right to erasure), Article 20 (portability), and Article 22 (automated decision-making) are the primary compliance obligations requiring software support
- CCPA/CPRA (California, effective 2020/2023): dominant US privacy law; requires DSR workflows, opt-out of sale, and sensitive data protections
- 25+ US state privacy laws as of 2026 (Virginia VCDPA, Colorado CPA, Connecticut, Texas, Oregon, Montana, Illinois, and others): each with slightly different timelines, opt-out rights, and definitions; multi-state compliance management is a distinct software requirement
- Brazil LGPD, Canada PIPEDA/Law 25, India DPDP Act (2023): additional major privacy regimes for global organisations
- EU AI Act (effective 2026): creates AI governance obligations that intersect with privacy compliance; AI systems that process personal data or influence decisions about data subjects face additional transparency, conformity assessment, and human oversight requirements
- IAB TCF v2.2: the cookie consent framework for programmatic advertising; requires IAB Europe membership for publishers and vendors; implementable under the IAB terms but not freely open
- OpenDSR specification: Apache Licence 2.0 (permissive; patent-grant included); freely implementable
- ISO 29100 and ISO 27701: voluntary international standards; no IP restrictions on compliance
- NIST Privacy Framework 1.0: US voluntary standard; public domain, freely implementable
- No patent-encumbered techniques identified in standard privacy compliance workflows; AI data classification ML models may be subject to broad ML patents (currently unenforced in privacy tech context)

---

## Recommended Feature Scope

**Must-have (MVP)**
- Cookie consent management with auto-domain scanning, configurable banner, IAB TCF v2.2-compatible consent signal management, and consent audit trail
- DSAR intake portal with self-service submission, identity verification, and statutory deadline tracking per jurisdiction
- DSR lifecycle workflow: intake, routing, data system query coordination, redaction, response assembly, and delivery with audit trail
- Data processing inventory (RoPA) with manual and semi-automated data mapping across connected systems
- Privacy notice and policy management with version history and jurisdiction-specific variants
- HRIS and product database connectors for DSR data discovery (minimum: Salesforce, PostgreSQL, MySQL, AWS S3)
- SOC 2 Type II certification path and GDPR data processing agreement

**Should-have (v1.1)**
- Automated data discovery from live system connections for continuous RoPA maintenance without manual questionnaire dependency
- Multi-jurisdiction DSR routing applying correct legal deadline and response template based on requester jurisdiction
- Real-time consent signal propagation to downstream vendors and MarTech platforms
- Privacy Impact Assessment (PIA / DPIA) workflow with configurable risk assessment templates
- Vendor and data processor management with DPA tracking and privacy risk scoring
- EU Pay Transparency and US state pay transparency compliance hooks (for HR-adjacent deployments)

**Nice-to-have (backlog)**
- AI governance module: EU AI Act impact assessments, high-risk AI system inventory, and training data transparency documentation
- Regulatory change monitoring with automated programme update alerts across 130+ jurisdictions
- Privacy-at-infrastructure enforcement layer intercepting data flows at API gateway level
- Cross-regulation compliance dashboard showing simultaneous posture against GDPR, CCPA, LGPD, India DPDP, and US state laws
- Natural-language privacy analytics for compliance team self-service queries without SQL skills
