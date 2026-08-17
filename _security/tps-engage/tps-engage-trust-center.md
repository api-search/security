---
api_specs:
- filename: tps-engage-play-api-openapi.yml
  format: yaml
  label: TPS Engage Play API
  slug: tps-engage-play-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/openapi/tps-engage-play-api-openapi.yml
- filename: tps-engage-prefetch-api-openapi.yml
  format: yaml
  label: TPS Engage Prefetch API
  slug: tps-engage-prefetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/openapi/tps-engage-prefetch-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Tps Engage Trust Center
name_suffix: Trust Center
overview: TPS Engage maintains a public trust center covering its security and compliance posture.
provider_name: TPS Engage
provider_slug: tps-engage
slug: tps-engage-trust-center
source_filename: tps-engage-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://seeblindspot.com/trust-and-security/\ndocs: https://seeblindspot.com/legal/\nsummary: >-\n  Blindspot publishes a genuine, self-hosted trust page at /trust-and-security/,\n  backed by a full legal hub at /legal/ with twelve policy documents including a\n  maintained subprocessor list and an accessibility conformance statement. It holds\n  no third-party security certifications and says so plainly rather than implying\n  otherwise: \"Formal third-party certifications, where pursued, will be listed here\n  as they are obtained.\" The compliance posture that IS published is privacy- and\n  accessibility-shaped (GDPR-style DPA, named DPO, 30-day subprocessor notice, WCAG\n  2.2 AA), not audit-shaped. There is no third-party trust portal (Vanta/Drata/\n  SafeBase) and no downloadable evidence pack.\ntrust_center:\n  present: true\n  self_hosted: true\n  url: https://seeblindspot.com/trust-and-security/\n  provider: none\
  \ (own site)\n  requires_nda: false\n  requires_login: false\ncertifications: []\ncertifications_note: >-\n  No SOC 2, ISO 27001, ISO 27701, PCI DSS, HIPAA or FedRAMP claim is made. The page\n  states certifications \"where pursued, will be listed here as they are obtained\",\n  which is an honest null rather than an unverifiable badge — worth noting because\n  unbacked cert claims are common in this sector.\ncompliance_program:\n  published: true\n  regimes:\n  - regime: GDPR / EU data protection\n    evidence: >-\n      \"A Data Processing Addendum is available to customers\" (obtainable from\n      dpo@seeblindspot.com). Named Data Protection Officer contact published.\n      EEA customer data is hosted in EU data centres. EEA contracting entity is\n      SC FREEDOM MASK SRL (Bucharest, Romania).\n  - regime: Subprocessor transparency\n    evidence: >-\n      Maintained public subprocessor list at https://seeblindspot.com/subprocessors/\n      with service and processing location per\
  \ vendor, plus a commitment to \"at least\n      30 days' notice before adding or replacing a subprocessor that processes\n      customer personal data, so they can review or object on reasonable\n      data-protection grounds.\"\n  - regime: US state privacy / opt-out\n    evidence: >-\n      Dedicated \"Your Privacy Choices\" page (https://seeblindspot.com/your-privacy-choices/)\n      alongside a cookie policy and a mobile-advertising-ID explainer\n      (https://seeblindspot.com/mobile-advertising-ids/).\n  - regime: WCAG 2.2 AA accessibility\n    evidence: >-\n      Published accessibility statement at\n      https://seeblindspot.com/accessibility-statement/ claiming WCAG 2.2 AA\n      conformance with a barrier-reporting route.\n  - regime: Advertising content standards\n    evidence: >-\n      Published advertising policy (allowed/prohibited creative, restricted\n      categories, review process) at https://seeblindspot.com/advertising-policy/ and\n      an acceptable use & enforcement\
  \ policy at\n      https://seeblindspot.com/acceptable-use-policy/.\nsecurity_practices:\n  source: https://seeblindspot.com/trust-and-security/\n  encryption_in_transit: 'TLS 1.2+ (\"Encryption of data in transit (TLS 1.2+) and of stored personal data at rest\")'\n  encryption_at_rest: true\n  access_control: >-\n    \"Access control on a least-privilege basis, with multi-factor authentication for\n    administrative and remote access\"\n  logging: '\"Logging, monitoring, and alerting across key systems\"'\n  vulnerability_management: '\"Vulnerability and patch management and secure software-development practices\"'\n  backups: '\"Backups and tested restoration for resilience\"'\n  hosting: >-\n    \"The Platform runs on Amazon Web Services (AWS)\" — EU data centres for EEA\n    customer data, US data centres otherwise. AWS is resold via DoiT International\n    per the subprocessor list.\n  penetration_testing: not published\n  data_retention: not published\nsubprocessors:\n  url: https://seeblindspot.com/subprocessors/\n\
  \  notice_period: 30 days\n  count: 13\n  vendors:\n  - {name: DoiT International / AWS, service: Cloud hosting, location: EU and US}\n  - {name: Pipedrive, service: CRM, location: EU / US}\n  - {name: Cookiebot (Usercentrics), service: Cookie consent, location: EU}\n  - {name: SendGrid (Twilio), service: Transactional email, location: US / EU}\n  - {name: MailerLite, service: Marketing email, location: EU}\n  - {name: PostHog, service: Product analytics, location: EU / US}\n  - {name: Google Analytics, service: Analytics, location: US / EU}\n  - {name: LogRocket, service: Session analytics, location: US}\n  - {name: Mapbox, service: Maps, location: US}\n  - {name: Gleap, service: Support widget, location: EU / US}\n  - {name: Usermaven, service: Analytics, location: EU / US}\n  - {name: Narrative, service: Audience/attribution data, location: US}\n  - {name: Accretive, service: Measurement, location: US}\ncontacts:\n  security: security@seeblindspot.com\n  privacy: dpo@seeblindspot.com\n\
  \  support: support@seeblindspot.com\n  billing: billing@seeblindspot.com\nlegal_documents:\n  url: https://seeblindspot.com/legal/\n  documents:\n  - {name: Terms of Service, url: https://seeblindspot.com/terms-of-service/}\n  - {name: Privacy Policy, url: https://seeblindspot.com/privacy-policy/}\n  - {name: Cookie Policy, url: https://seeblindspot.com/cookie-policy/}\n  - {name: Your Privacy Choices, url: https://seeblindspot.com/your-privacy-choices/}\n  - {name: Accessibility Statement, url: https://seeblindspot.com/accessibility-statement/}\n  - {name: Advertising Policy, url: https://seeblindspot.com/advertising-policy/}\n  - {name: Refund & Credits Policy, url: https://seeblindspot.com/refund-and-credits-policy/}\n  - {name: Support & Disputes Policy, url: https://seeblindspot.com/support-and-disputes-policy/}\n  - {name: Acceptable Use & Enforcement Policy, url: https://seeblindspot.com/acceptable-use-policy/}\n  - {name: Subprocessors, url: https://seeblindspot.com/subprocessors/}\n\
  \  - {name: Trust & Security, url: https://seeblindspot.com/trust-and-security/}\n  - {name: Agency Addendum, url: https://seeblindspot.com/agency-addendum/}\nobserved:\n- url: https://seeblindspot.com/trust-and-security/\n  status: 200\n  checked: '2026-08-13'\n- url: https://seeblindspot.com/legal/\n  status: 200\n  checked: '2026-08-13'\n- url: https://seeblindspot.com/subprocessors/\n  status: 200\n  checked: '2026-08-13'\n- url: https://seeblindspot.com/trust/\n  status: 404\n  checked: '2026-08-13'\ngaps:\n- No third-party audit or certification of any kind.\n- No published penetration-test cadence or summary letter.\n- No published data-retention schedule.\n- No machine-readable security.txt pointing at the trust page (see security/tps-engage-vulnerability-disclosure.yml).\n- No uptime/availability commitment (see lifecycle/tps-engage-lifecycle.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tps-engage/refs/heads/main/security/tps-engage-trust-center.yml
summary_line: trust center published
tags:
- Company
- Advertising
- DOOH
- Digital Billboards
- Programmatic Advertising
- Media Buying
- Out-of-Home
trust_url: ''
---
