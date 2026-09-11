---
api_specs:
- filename: aedifion-openapi.yml
  format: yaml
  label: aedifion HTTP API
  slug: aedifion-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/openapi/aedifion-openapi.yml
- filename: aedifion-mqtt-asyncapi.yml
  format: yaml
  label: aedifion MQTT API
  slug: aedifion-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/asyncapi/aedifion-mqtt-asyncapi.yml
certification_count: 2
certifications:
- DIN EN ISO/IEC 27001
- GDPR / DSGVO
description: ''
kind: trust-center
layout: security
name: Aedifion Trust Center
name_suffix: Trust Center
overview: Aedifion maintains a public trust center documenting DIN EN ISO/IEC 27001 and GDPR / DSGVO compliance.
provider_name: Aedifion
provider_slug: aedifion
slug: aedifion-trust-center
source_filename: aedifion-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nprobe: true\nurl: https://www.aedifion.com/sicherheit\nnote: >-\n  aedifion runs no dedicated trust-center subdomain - trust.aedifion.com and\n  security.aedifion.com do not resolve, and the automated probe recorded no hit. It does\n  publish a substantive security and compliance page on its main site, with a named certifying\n  body and the certificate itself available for download, plus a security architecture section\n  in the developer documentation. Recorded here because the compliance posture is genuinely\n  published, not because a trust portal exists.\ncertifications:\n- name: DIN EN ISO/IEC 27001\n  status: certified\n  since: '2023-12'\n  certifier: INFAZ Institut fuer Auditierung und Zertifizierung\n  scope: 'processes and systems in all business areas'\n  certificate_url: https://cdn.prod.website-files.com/6942a43e5bcce46ebe9f73a1/696e525b02ad6e609db2751c_2025_aedifion_certificate_iso-iec-27001_de.pdf\n  certificate_verified:\
  \ true\n  certificate_http_status: 200\n  certificate_content_type: application/pdf\n  certificate_bytes: 302351\n- name: GDPR / DSGVO\n  status: compliant\n  evidence: Privacy policy published; all processing in Germany.\nhosting:\n  provider: Hetzner Online GmbH\n  locations: [Nuremberg, Falkenstein]\n  country: Germany\n  provider_certification: DIN ISO/IEC 27001\n  dedicated_option: 'On demand, aedifion stores and processes your data on dedicated servers.'\nsecurity_posture:\n  transport_encryption: TLS between edge device and platform; SSH as an alternative\n  certificates: X.509 from Let's Encrypt, renewed quarterly\n  access_control: >-\n    Role-based access control with read or write granularity on individual datapoints;\n    federation with LDAP and Active Directory via OpenID Connect, OAuth and SAML\n  penetration_testing: >-\n    Edge devices \"must pass an extensive series of functional and penetration tests\" before\n    commissioning. No platform-level pentest report or\
  \ summary is published.\n  uptime_commitment: '97%'\ncontact:\n  general: contact@aedifion.com\n  phone: '+49 221 98650-770'\n  page: https://www.aedifion.com/kontakt\nevidence:\n- source: https://www.aedifion.com/sicherheit\n  status: 200\n  keywords: [ISO 27001, DIN EN ISO/IEC 27001, INFAZ, DSGVO, Informationssicherheit]\n- source: https://docs.aedifion.io/en/products/general/security/overview/\n  status: 200\n  keywords: [TLS, X.509, RBAC, penetration tests, ISO 27001, Hetzner]\n- source: https://cdn.prod.website-files.com/6942a43e5bcce46ebe9f73a1/696e525b02ad6e609db2751c_2025_aedifion_certificate_iso-iec-27001_de.pdf\n  status: 200\ngaps:\n- No SOC 2 report.\n- No trust portal or subprocessor list.\n- No published vulnerability disclosure policy, security.txt or bug bounty - see below.\nvulnerability_disclosure:\n  published: false\n  security_txt: false\n  bug_bounty: false\n  policy_url: null\n  note: >-\n    Probed /.well-known/security.txt on all six known hosts (all 404 or SPA\
  \ shell), and checked\n    /security, /responsible-disclosure and /vulnerability-disclosure. No responsible-disclosure\n    policy, no security@ address and no bug-bounty program was found. The only route for a\n    researcher is the general contact address. For an ISO 27001 certified operator of building\n    control systems, a published disclosure channel is the clearest gap in this profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/security/aedifion-trust-center.yml
summary_line: DIN EN ISO/IEC 27001, GDPR / DSGVO
tags:
- Building Automation
- Smart Buildings
- Energy Management
- Internet of Things
- Real Estate
- HVAC
- Sustainability
- Time Series
- Analytics
- MQTT
- Building Operations
- ESG
- PropTech
- Germany
trust_url: https://www.aedifion.com/sicherheit
---
