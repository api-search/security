---
certifications:
- SOC 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Spate Trust Center
name_suffix: Trust Center
overview: Spate maintains a public trust center documenting SOC 2 and GDPR compliance.
provider_name: Spate
provider_slug: spate
slug: spate-trust-center
source_filename: spate-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.spate.nyc/security-at-spate\nnote: >-\n  Spate publishes a single \"Security At Spate\" page rather than a hosted\n  trust portal (no trust.spate.nyc, no Vanta/Drata/SafeBase surface — those\n  hostnames do not resolve to a Spate property). The page is real, substantive\n  and names its certifications, so it is recorded as the trust surface, with\n  the caveat that no artifacts (report, certificate, subprocessor list) are\n  downloadable or requestable from it.\n\ntrust_center:\n  url: https://www.spate.nyc/security-at-spate\n  hosted_platform: null\n  self_serve_artifacts: false\n  nda_gated_request_flow: false\n  contact: security@spate.nyc\n\ncertifications:\n- name: SOC 2\n  status: claimed\n  type: unspecified\n  auditor: not named\n  report_available: false\n  quote: >-\n    \"SOC 2 (System and Organization Controls 2) is a framework for assessing\n    the controls related to security, availability, processing\
  \ integrity,\n    confidentiality, and privacy\"\n- name: GDPR\n  status: claimed\n  scope: regulatory adherence\n  quote: >-\n    \"we adhere to other relevant regulatory requirements including GDPR\"\n\ncontrols_published:\n- Automated vulnerability scanning of infrastructure and codebase\n- Penetration testing at least once annually\n- Security awareness training for employees\n- Stringent access controls and continuous infrastructure monitoring\n- Encryption of sensitive data in transit and at rest\n- Application secrets encrypted and stored in Google Cloud Secret Manager\n- Documented incident response with detailed incident logs and post-incident review\n- Third-party risk assessment and contractual oversight\n- Regular internal and external audits by accredited auditors\n\nrelated_policies:\n- name: Data Collection Policy\n  url: https://help.spate.nyc/en/article/data-collection-policy\n  note: >-\n    Governs Spate's own collection of public web data — lawfulness,\n    publicly-available-only\
  \ sourcing, data minimization, anonymization and\n    aggregation. Directly relevant to a buyer assessing the provenance of\n    the trend data the API returns.\n- name: SLA\n  url: https://help.spate.nyc/en/article/sla-service-level-agreement\n- name: Privacy Policy\n  url: https://www.spate.nyc/privacy-policy\n- name: Your Privacy Rights\n  url: https://www.spate.nyc/your-privacy-rights\n\ngaps:\n- No subprocessor list published.\n- No data-residency statement.\n- SOC 2 Type I vs Type II not distinguished.\n- No downloadable or request-gated evidence of any named certification.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spate/refs/heads/main/security/spate-trust-center.yml
summary_line: SOC 2, GDPR
tags:
- Company
- Enterprise Saas
- Market Intelligence
- Trend Forecasting
- Consumer Insights
- Social Listening
- Analytics
- Beauty
- MCP
- AI Agents
- Trend Data
- Consumer Packaged Goods
trust_url: ''
---
