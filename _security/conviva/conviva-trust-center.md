---
certifications:
- ISO/IEC 27001:2022
description: Conviva publishes a Trust Center page covering compliance certification, data protection, encryption, access management, monitoring and vulnerability management. It is a narrative trust page, not a document-portal trust center (no SafeBase/Vanta/Drata portal, no downloadable audit reports behind an NDA request flow).
kind: trust-center
layout: security
name: Conviva Trust Center
name_suffix: Trust Center
overview: Conviva maintains a public trust center documenting ISO/IEC 27001:2022 compliance.
provider_name: Conviva
provider_slug: conviva
slug: conviva-trust-center
source_filename: conviva-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nprobe: true\nsource: https://www.conviva.ai/security/\nurl: https://www.conviva.ai/security/\nname: Conviva Trust Center\ndescription: >-\n  Conviva publishes a Trust Center page covering compliance certification, data protection,\n  encryption, access management, monitoring and vulnerability management. It is a narrative\n  trust page, not a document-portal trust center (no SafeBase/Vanta/Drata portal, no\n  downloadable audit reports behind an NDA request flow).\n\n# Only ISO/IEC 27001:2022 is claimed as Conviva's OWN certification. SOC 1 / SOC 2 are\n# explicitly attributed to the third-party cloud platforms Conviva hosts on, NOT to Conviva.\ncertifications:\n- name: ISO/IEC 27001:2022\n  scope: Conviva (own certification)\n  evidence: >-\n    \"Conviva is certified under ISO/IEC 27001:2022, the globally recognized standard for\n    information security management systems (ISMS).\"\nregulatory_compliance:\n- name: GDPR\n  evidence:\
  \ \"Conviva's services are compliant with the EU General Data Protection Regulation (GDPR)\"\n- name: UK GDPR\n  evidence: \"Conviva's services are compliant with ... UK GDPR\"\n- name: CCPA\n  evidence: \"Conviva's services are compliant with ... the California Consumer Privacy Act (CCPA)\"\n\ninherited_certifications:\n- name: SOC 1\n  scope: third-party cloud hosting platforms (not Conviva)\n- name: SOC 2\n  scope: third-party cloud hosting platforms (not Conviva)\n- name: ISO 27001\n  scope: third-party cloud hosting platforms (not Conviva)\ninherited_note: >-\n  \"Conviva hosts its cloud infrastructure on trusted third-party platforms that comply with\n  industry-recognized standards such as SOC 1, SOC 2, and ISO 27001, among others.\" This is an\n  inherited-control statement about hosting providers, not a Conviva audit report.\n\npractices:\n  encryption: In-transit and at-rest encryption of customer data.\n  access_management: Multi-factor authentication and role-based access control.\n\
  \  monitoring: Continuous monitoring for security threats, performance issues and service disruption.\n  vulnerability_management:\n    third_party_testing: Annual third-party penetration testing.\n    scanning: Continuous scanning of applications and infrastructure for vulnerabilities.\n  data_transfers: Standard Contractual Clauses (SCCs) for personal data transfers outside the EEA and UK.\n\ncontacts:\n  privacy: privacy@conviva.ai\n  support: support@conviva.com\n  security_disclosure: null   # no dedicated security@ address or coordinated-disclosure channel published\n\nrelated:\n  privacy_policy: https://legal.conviva.ai/privacy-policy/\n  terms_of_use: https://legal.conviva.ai/terms-of-use/\n  gdpr: https://legal.conviva.ai/gdpr/\n  cookie_policy: https://legal.conviva.ai/cookie-policy/\n  ccpa: https://legal.conviva.ai/ccpa-page/\n  subprocessors: https://legal.conviva.ai/conviva-subprocessors/\n  privacy_request_portal: https://privacyportal.onetrust.com/webform/68049a8d-acc0-4473-b871-a599fe9c9650/2a3e0a9e-438d-4a49-8a69-ca9d5d423428\n\
  \  status_page: https://status.conviva.com/\n\ngaps:\n- No /.well-known/security.txt on conviva.com, conviva.ai, docs.conviva.ai or api.conviva.com (all 404).\n- No published coordinated vulnerability disclosure policy, bug bounty, or security@ reporting address.\n- SOC 2 is inherited from hosting providers only; Conviva publishes no SOC 2 report of its own.\n\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://www.conviva.ai/security/\n  http_status: 200\n  emails_decoded_from: Cloudflare data-cfemail obfuscation on the page\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conviva/refs/heads/main/security/conviva-trust-center.yml
summary_line: ISO/IEC 27001:2022
tags:
- Analytics
- Streaming
- Video
- Observability
- Monitoring
- Media
- Quality of Experience
- Real-Time
- Telemetry
- Agents
- MCP
- Company
trust_url: https://www.conviva.ai/security/
---
