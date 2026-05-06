# Standards & API Reference

> Project: Privacy Compliance Manager · Generated: 2026-05-06

## Industry Standards & Specifications

### ISO Standards

**ISO/IEC 27701:2025 — Privacy Information Management Systems (PIMS)**
- URL: https://www.iso.org/standard/27701
- The primary international standard for managing privacy compliance programs. The 2025 revision made it a standalone management system (no longer requiring ISO 27001 as a prerequisite), added AI-specific privacy controls, and removed 52 non-privacy controls to sharpen focus. Directly maps to GDPR, CCPA, LGPD, and other major regulations. Any privacy compliance platform claiming international alignment should support PIMS audit workflows derived from this standard.

**ISO/IEC 27001:2022 — Information Security Management Systems (ISMS)**
- URL: https://www.iso.org/standard/27001
- Foundation information security management standard. Privacy compliance platforms that bundle security posture features (e.g. Securiti.ai, OneTrust) typically include ISO 27001 controls in their risk register and assessment modules. Closely coupled with ISO 27701.

**ISO/IEC 29100:2011 — Privacy Framework**
- URL: https://www.iso.org/standard/45123.html
- Establishes common privacy terminology and a framework of privacy principles used across the ISO/IEC privacy standards family. Foundational reference for consent management, data minimisation, and individual participation principles—all core features of a privacy compliance manager.

**ISO/IEC 29101:2018 — Privacy Architecture Framework**
- URL: https://www.iso.org/standard/75293.html
- Provides guidance for planning, designing, and building ICT system architectures that protect personally identifiable information (PII). Relevant for defining the data flow and architecture layers of a privacy compliance platform itself.

**ISO/IEC 29134:2023 — Guidelines for Privacy Impact Assessment**
- URL: https://www.iso.org/standard/86012.html
- International standard defining the methodology and documentation requirements for Privacy Impact Assessments (PIAs) / Data Protection Impact Assessments (DPIAs). A privacy compliance manager must support PIA/DPIA workflows aligned to this standard to satisfy GDPR Article 35 requirements.

**ISO/IEC 27018:2019 — Protection of PII in Public Clouds**
- URL: https://www.iso.org/standard/76559.html
- Code of practice for protecting personally identifiable information in public cloud environments. Relevant to the hosting and processing architecture of SaaS privacy compliance platforms and their data processor obligations.

### W3C & IETF Standards

**W3C Privacy Principles**
- URL: https://www.w3.org/TR/privacy-principles/
- W3C's official articulation of privacy design principles for web standards and applications. Covers data minimisation, user control, transparency, and purpose limitation. Provides the conceptual framework that browser-based consent management and cookie compliance features should implement.

**W3C Global Privacy Control (GPC) Specification**
- URL: https://w3c.github.io/gpc/
- Browser-level HTTP signal (`Sec-GPC: 1`) allowing users to express a universal opt-out preference for sale or sharing of personal data. As of 2025, formally adopted as a W3C Privacy Working Group work item. California (AB 566, 2025) mandates all major browsers support GPC by January 2027. Privacy compliance platforms must detect and honour GPC signals as legally equivalent to manual opt-out in several US states.

**IETF RFC 6973 — Privacy Considerations for Internet Protocols**
- URL: https://datatracker.ietf.org/doc/html/rfc6973
- IETF guidance for building privacy considerations into protocol and API design. Covers data minimisation, anonymisation, unlinkability, and confidentiality. Directly applicable to the design of the compliance platform's own APIs and data exchange with third-party processors.

**IETF RFC 8942 — HTTP Client Hints**
- URL: https://datatracker.ietf.org/doc/html/rfc8942
- Mechanism by which servers can request client metadata. Relevant to consent signal propagation and fingerprinting risk analysis in cookie/tracker compliance modules.

### Data Model & API Specifications

**OpenDSR (formerly OpenGDPR)**
- URL: https://github.com/opengdpr/OpenDSR
- Open JSON specification enabling Controllers and Processors to communicate and manage Data Subject Requests (DSRs) in a uniform and interoperable manner. The de-facto API standard for automating DSR workflows across service providers. Any privacy compliance manager implementing DSR automation should support OpenDSR as the interchange format.

**IAB Europe Transparency and Consent Framework (TCF) v2.3**
- URL: https://iabeurope.eu/transparency-consent-framework/
- CMP API Spec: https://github.com/InteractiveAdvertisingBureau/GDPR-Transparency-and-Consent-Framework/blob/master/TCFv2/IAB%20Tech%20Lab%20-%20CMP%20API%20v2.md
- Industry standard governing how Consent Management Platforms (CMPs) signal user consent and legitimate interest to digital advertising vendors. TCF v2.3 (released June 2025) is the current version. Cookie compliance and consent management features must implement the TCF CMP API to support publishers and advertising tech stacks.

**IAB US Privacy String / GPP (Global Privacy Platform)**
- URL: https://iabtechlab.com/standards/global-privacy-platform/
- Successor to the US Privacy String; a unified signal framework encoding consent and privacy preferences across multiple US state privacy laws into a single string. Required for ad-tech integrations supporting CCPA, CPRA, and state-level opt-outs.

**OpenAPI Specification 3.1**
- URL: https://spec.openapis.org/oas/v3.1.0.html
- The industry standard for REST API description. Privacy compliance platforms expose their APIs documented in OpenAPI format; integrations and DSR automation rely on OpenAPI-described endpoints. Also relevant as the format for the F-Secure GDPR Subject Rights API spec (https://github.com/F-Secure/gdpr-subject-rights-api).

**JSON Schema (Draft 2020-12)**
- URL: https://json-schema.org/specification
- Standard for describing and validating JSON data structures. Used by OpenDSR, OpenAPI, and DSR automation platforms to validate privacy request payloads, consent records, and data inventory exports.

### Security & Authentication Standards

**OAuth 2.0 — RFC 6749**
- URL: https://datatracker.ietf.org/doc/html/rfc6749
- Authorization framework underpinning API access control for privacy platforms and their integrations. Scopes provide data-minimisation-aligned access control, directly supporting GDPR's requirement that third parties access only the data they need. All major privacy compliance platforms (OneTrust, BigID, Osano) use OAuth 2.0 for API authentication.

**OpenID Connect 1.0 (OIDC)**
- URL: https://openid.net/specs/openid-connect-core-1_0.html
- Identity layer on top of OAuth 2.0; enables consent-aware authentication, pairwise subject identifiers (preventing cross-application user tracking), and the `prompt=consent` parameter for forced consent re-collection. Directly supports GDPR data minimisation and consent compliance in authentication flows.

**OWASP Privacy Risks (LINDDUN Framework)**
- URL: https://owasp.org/www-project-top-10-privacy-risks/
- OWASP's catalogue of top privacy risks in web applications (linkability, identifiability, non-repudiation, detectability, disclosure, unawareness, non-compliance). Compliance platforms conducting privacy risk assessments should reference LINDDUN threat categories alongside OWASP security risks.

**NIST Privacy Framework 1.1 (Draft)**
- URL: https://www.nist.gov/privacy-framework
- NIST CSWP 40: https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.40.ipd.pdf
- Voluntary US framework for privacy risk management structured around Identify-P, Govern-P, Control-P, Communicate-P, and Protect-P functions. Cross-walks are published for GDPR, CCPA, CPRA, LGPD, and VCDPA. Increasingly adopted by US federal agencies and enterprise compliance programs. A privacy compliance manager should be able to generate NIST Privacy Framework profile reports.

**NIST SP 800-53 Rev. 5 — Privacy Controls**
- URL: https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r5.pdf
- Catalogue of security and privacy controls for federal information systems; the authoritative control set for US public sector compliance. Privacy controls (PT family) cover consent, individual access, data quality, and de-identification.

**NIST SP 800-122 — Guide to Protecting PII Confidentiality**
- URL: https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-122.pdf
- Practical guidance for categorising PII sensitivity and selecting appropriate safeguards. Relevant to data classification features within a compliance manager.

---

## Similar Products — Developer Documentation & APIs

### OneTrust

- **Description:** Market-leading privacy, security, and data governance platform covering consent management, data mapping, DSAR workflow, vendor risk, and DPIA. Serves 14,000+ enterprise customers.
- **API Documentation:** https://developer.onetrust.com/onetrust/reference/onetrust-api-reference
- **Developer Portal:** https://developer.onetrust.com/
- **SDKs/Libraries:** Next Generation CMP SDK for iOS, Android, Web (JavaScript), MAUI, React Native — https://developer.onetrust.com/onetrust/docs/onetrusts-next-generation-cmp-sdks
- **Developer Guide:** https://developer.onetrust.com/onetrust/docs/api-reference-maui-legacy
- **Standards:** REST/JSON; OpenAPI-documented; IAB TCF v2.x; IAB US Privacy / GPP; CCPA US Privacy String
- **Authentication:** OAuth 2.0 (client credentials for server-side); API Key for CMP SDK integrations
- **API Coverage:** Consent & Preferences, Data Subject Rights (DSAR), Data Mapping, Vendor Risk, AI Governance, Tech Risk & Compliance

### BigID

- **Description:** Enterprise data security and privacy platform focused on data discovery, classification, and privacy compliance automation. IDC MarketScape Leader 2025. Supports GDPR, CCPA, HIPAA, LGPD.
- **API Documentation:** https://developer.bigid.com/
- **API Tracker:** https://apitracker.io/a/bigid
- **SDKs/Libraries:** REST API, OpenAPI spec, GraphQL, CLI, IDE plugins
- **Standards:** REST/JSON; OpenAPI 3.x; GraphQL; MCP (Model Context Protocol) for LLM agent integration
- **Authentication:** OAuth 2.0; API Key
- **API Coverage:** Data source connectors, scan triggering, catalog queries, DSR automation, policy management, LLM agent integration via MCP

### Osano

- **Description:** Privacy management platform processing over 1 billion consents per month. Covers cookie consent, DSAR processing, vendor risk, and data mapping. Strong mid-market position.
- **API Documentation:** https://developers.osano.com/uc/core-api/openapi
- **Developer Docs:** https://developers.osano.com/
- **Standards:** REST/JSON; OpenAPI-documented; GPC (Global Privacy Control) signal support
- **Authentication:** API Key; OAuth 2.0
- **API Coverage:** Consent creation and retrieval, GPC signal handling, DSAR workflow, vendor monitoring

### Didomi

- **Description:** European consent management and preference management platform. Strong TCF compliance; supports Web, iOS, Android SDKs. Developer-first CMP with full programmatic API.
- **API Documentation:** https://developers.didomi.io/api-and-platform/consents
- **Web SDK API Reference:** https://developers.didomi.io/cmp/web-sdk/reference/api
- **Developer Portal:** https://developers.didomi.io/
- **SDKs/Libraries:** JavaScript Web SDK, iOS SDK, Android SDK, React Native SDK
- **Developer Guide:** https://developers.didomi.io/cmp/web-sdk/getting-started
- **Standards:** REST/JSON; IAB TCF v2.x; IAB CCPA US Privacy String; GPP
- **Authentication:** API Key; JWT
- **API Coverage:** Consent status checks, consent registration, user preference management, vendor list management, programmatic UI control

### Transcend

- **Description:** Privacy infrastructure platform with best-in-class DSR automation. API-first; 2,000+ native integrations for automated data discovery and deletion across SaaS tools. Favoured by engineering-led privacy teams.
- **API Documentation:** https://docs.transcend.io/docs/api
- **Standards:** REST/JSON; OpenDSR-compatible; OpenAPI-documented
- **Authentication:** OAuth 2.0; API Key
- **API Coverage:** DSR intake and orchestration, data silo discovery, consent management, preference management, data inventory

### DataGrail

- **Description:** Data privacy platform focused on DSR automation and real-time data mapping with 2,000+ pre-built integrations. Trusted by Databricks, Overstock, and other major tech companies.
- **API Documentation:** https://docs.datagrail.io/
- **Standards:** REST/JSON; OpenDSR framework; OpenAPI-documented
- **Authentication:** OAuth 2.0; API Key
- **API Coverage:** DSR submission and fulfillment, data system integrations, consent signal processing

### Privacera

- **Description:** Data access governance and privacy platform. Strong in Databricks, Spark, and cloud data platform integrations. Enterprise-grade ABAC and data masking.
- **API Documentation:** https://docs.privacera.com/
- **API Tracker:** https://apitracker.io/a/privacera
- **SDKs/Libraries:** REST API, OpenAPI spec
- **Standards:** REST/JSON; OpenAPI-documented
- **Authentication:** OAuth 2.0; API Key; LDAP/AD integration
- **API Coverage:** Data access policy management, data masking rules, audit logs, connector configuration

### mParticle DSR API

- **Description:** Customer data platform with a dedicated Data Subject Request API implementing the OpenDSR specification. Relevant as a reference implementation of DSR API design patterns.
- **API Documentation:** https://docs.mparticle.com/developers/apis/dsr-api/v3/
- **Standards:** OpenDSR v3; REST/JSON
- **Authentication:** API Key; OAuth 2.0
- **API Coverage:** DSR submission (access, portability, erasure, restriction), status tracking, callback notifications

---

## Notes

**Evolving regulatory signal standards:** The Global Privacy Control (GPC) landscape is shifting rapidly. California AB 566 (signed October 2025) mandates all major browsers support GPC by January 2027. This will make GPC signal detection a mandatory feature for any consent management or preference management module, not just a best-practice. Privacy compliance platforms built today should treat GPC as a first-class signal.

**OpenDSR as the interoperability standard:** The OpenDSR specification (formerly OpenGDPR) remains the only widely-adopted open standard for DSR interoperability between controllers and processors. However, adoption is uneven—major platforms support it but many SaaS vendors still require custom integrations. This is one of the clearest opportunities for an open-source AI-native platform to drive standardisation.

**IAB TCF v2.3:** Released June 2025, this resolves signalling ambiguity for vendor disclosure. Implementations targeting the advertising ecosystem must target TCF v2.3, not v2.2.

**NIST Privacy Framework 1.1:** As of early 2026, version 1.1 remains in draft (Initial Public Draft published). The final release is expected to bring full alignment with NIST CSF 2.0. Organizations doing compliance mapping should note that published crosswalks reference v1.0 and may need updating once 1.1 is finalised.

**MCP (Model Context Protocol) for privacy AI agents:** BigID's developer portal already documents MCP integration for LLM-based compliance agents (Claude, ChatGPT). This emerging pattern—exposing compliance data through MCP servers so AI agents can query and act on it—is an architectural direction worth building into a new AI-native platform from the outset.
