---
certifications:
- SOC 2 Type 2
- ISO 27001
description: ''
kind: trust-center
layout: security
name: 1Touch Io Trust Center
name_suffix: Trust Center
overview: 1touch.io maintains a public trust center documenting SOC 2 Type 2 and ISO 27001 compliance.
provider_name: 1touch.io
provider_slug: 1touch-io
slug: 1touch-io-trust-center
source_filename: 1touch-io-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nprobe: true\nsource: https://www.1touch.io/resources/trust-and-security-center\nurl: https://www.1touch.io/resources/trust-and-security-center\nnote: No dedicated trust portal host (trust.1touch.io / security.1touch.io do not\n  resolve). The trust content is a page on the marketing site; audit reports are\n  offered on request under NDA rather than self-served.\ncertifications:\n- name: SOC 2 Type 2\n  status: audited annually\n  availability: report available on request under NDA\n- name: ISO 27001\n  status: certified\n  availability: stated on the trust page\nprogram:\n  name: Information Security Program (ISP)\n  areas:\n  - access controls\n  - encryption\n  - employee security training\n  - credential and key management\n  - physical security\n  - network and cloud security\n  - secure software development life cycle (SSDLC)\nplatform_security:\n  encryption_in_transit: TLS 1.2/1.3 enforced\n  encryption_at_rest: AES-256\n \
  \ granularity: raw / column / value level encryption\n  customer_managed_keys: true\n  authentication: OAuth2 / OpenID with multi-factor authentication\n  api_security: token-based API gateway, rate limiting, gateway protections\n  network: VPC-based architecture with segmentation and firewall allow-listing\n  monitoring: continuous security auditing and real-time anomaly detection\nsubprocessors:\n- name: Google Cloud Platform\n  location: USA\n  purpose: SaaS hosting\n- name: Coralogix\n  location: USA\n  purpose: centralized logging and analytics\ngaps:\n  status_page: none published\n  sla: none published\n  dpa: not linked from the trust page\n  terms_of_service: no terms-of-service page published (privacy and cookie policies\n    only)\nevidence:\n- source: https://www.1touch.io/resources/trust-and-security-center\n  http_status: 200\n  keywords:\n  - soc 2 type 2\n  - iso 27001\n  - information security program\n  - trust and security center\nx-evidence:\n  fetched: '2026-08-05'\n\
  \  url: https://www.1touch.io/resources/trust-and-security-center\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1touch-io/refs/heads/main/security/1touch-io-trust-center.yml
summary_line: SOC 2 Type 2, ISO 27001
tags:
- Company
- Data Security
- Data Discovery
- Data Classification
- DSPM
- Data Governance
- Privacy
- Compliance
- Mainframe
- Access Control
- AI Security
trust_url: https://www.1touch.io/resources/trust-and-security-center
---
