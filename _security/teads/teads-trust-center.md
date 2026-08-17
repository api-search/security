---
certifications:
- SOX (Sarbanes-Oxley)
- unnamed security accreditations
description: 'Teads publishes a "Security at Teads" trust page describing its security program: a formal ISMS, SOX compliance as a public company, annual third-party penetration testing, a HackerOne bug bounty, encryption in transit and at rest, regional data residency, and 24/7 internal SOC monitoring. Named certificate artifacts (SOC 2 / ISO 27001 reports) are NOT published — the page says Teads "holds several security accreditations" and directs requesters to a business representative, so those remain unnamed and gated.'
kind: trust-center
layout: security
name: Teads Trust Center
name_suffix: Trust Center
overview: Teads maintains a public trust center documenting SOX (Sarbanes-Oxley) and unnamed security accreditations compliance.
provider_name: Teads
provider_slug: teads
slug: teads-trust-center
source_filename: teads-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.teads.com/security/\ndescription: >-\n  Teads publishes a \"Security at Teads\" trust page describing its security\n  program: a formal ISMS, SOX compliance as a public company, annual third-party\n  penetration testing, a HackerOne bug bounty, encryption in transit and at\n  rest, regional data residency, and 24/7 internal SOC monitoring. Named\n  certificate artifacts (SOC 2 / ISO 27001 reports) are NOT published — the page\n  says Teads \"holds several security accreditations\" and directs requesters to a\n  business representative, so those remain unnamed and gated.\ntrust_page:\n  url: https://www.teads.com/security/\n  status: 200\n  title: Security at Teads\n  self_service_portal: false\n  note: >-\n    A static trust page, not a document-request portal (no Vanta/Drata/SafeBase\n    style trust center was found).\ncertifications:\n- name: SOX (Sarbanes-Oxley)\n  status: claimed\n  evidence: >-\n    \"As a\
  \ public company Teads is SOX compliant and also holds several security\n    accreditations.\"\n  named_report: false\n- name: unnamed security accreditations\n  status: claimed-unnamed\n  evidence: >-\n    Teads states it holds accreditations but does not name them; access is via a\n    business representative.\n  named_report: false\n  gap: >-\n    No SOC 2, ISO 27001, PCI DSS, HIPAA or FedRAMP artifact is named or\n    downloadable.\nprogram:\n  isms:\n    formal: true\n    evidence: \"There is a formally implemented and maintained Information Security Management System throughout the Enterprise.\"\n  risk_management: true\n  external_audits: true\n  penetration_testing:\n    cadence: annual\n    party: independent third parties\n  vulnerability_monitoring: continuous, real-time triage\n  secure_sdlc: true\n  security_awareness_training: all employees\n  soc: internal SOC monitored 24/7\n  bc_dr:\n    tested: annually\n    basis: business impact analyses\naccess_security:\n  logging:\
  \ All user access logged; log access on auditable least-privilege basis.\n  least_privilege: true\n  access_review_cadence: semiannual\n  sso: required for all employees, with frequent reauthentication\n  data_lake_access: MFA-protected VPN or SSH only\nnetwork_security:\n  waf: true\n  firewall_acls: strict\ndata_security:\n  encryption_in_transit: true\n  encryption_at_rest: true\n  minimum_tls: TLS 1.2\n  data_lifecycle: purged and deleted at end of life per retention policy\n  residency:\n    principle: Data is hosted in the region it is collected and does not transfer between regions.\n    cloud_regions: [USA, Ireland, Netherlands, Japan, Singapore]\n    on_premise: [USA, Netherlands, Singapore]\n    transfers: First-party analytical data may transfer under SCCs.\nai_policy:\n  published: true\n  claims:\n  - Teads only uses AI to improve productivity and optimize ROI of delivered services.\n  - Teads will never sell customer data.\n  - Humans remain involved in training and integration;\
  \ usage aligned to applicable regulations.\n  source: https://www.teads.com/security/\nfraud_and_phishing:\n  contact: scam@teads.com\n  policy: >-\n    Teads never contacts individuals through social media or personal accounts\n    to conduct business, and prohibits private transfer or sale of accounts.\nprivacy:\n  privacy_policy: https://www.teads.com/privacy-policy/\n  advertising_privacy_portal: https://privacy-policy.teads.com/\n  modern_slavery_statement: https://privacy-policy.teads.com/Modern-Slavery-Act-Statement.pdf\nevidence:\n- url: https://www.teads.com/security/\n  status: 200\n- url: https://www.teads.com/privacy-policy/\n  status: 200\n- url: https://privacy-policy.teads.com/\n  status: 200\n- url: https://www.teads.com/trust-center/\n  status: 404\n  note: No dedicated trust-center path exists; the security page is the trust surface.\ncross_links:\n  vulnerability_disclosure: security/teads-vulnerability-disclosure.yml\n  domain_security: security/teads-domain-security.yml\n\
  \  conformance: conformance/teads-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teads/refs/heads/main/security/teads-trust-center.yml
summary_line: SOX (Sarbanes-Oxley), unnamed security accreditations
tags:
- Company
- Advertising
- AdTech
- Advertising Technology
- Video Advertising
- Conversions API
- Contextual Advertising
- Mobile SDK
- Conversational AI
trust_url: ''
---
