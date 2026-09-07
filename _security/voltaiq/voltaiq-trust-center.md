---
certification_count: 3
certifications:
- SOC 2 Type II
- GDPR
- ITAR
description: ''
kind: trust-center
layout: security
name: Voltaiq Trust Center
name_suffix: Trust Center
overview: Voltaiq maintains a public trust center documenting SOC 2 Type II, GDPR, and ITAR compliance.
provider_name: Voltaiq
provider_slug: voltaiq
slug: voltaiq-trust-center
source_filename: voltaiq-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nprobe: true\nsource: https://www.voltaiq.com/security\nurl: https://www.voltaiq.com/security\nnote: >-\n  Voltaiq does not run a hosted trust portal (trust.voltaiq.com does not resolve). Its\n  security and compliance posture is published as a single first-party page at\n  voltaiq.com/security, which names its certifications explicitly. Enriched by hand from that\n  page after probe-security-programs.py detected it.\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n  evidence: >-\n    \"Voltaiq holds SOC 2 Type II certification, conducts annual third-party penetration\n    testing, and is compliant with GDPR and ITAR.\"\n- name: GDPR\n  status: compliant\n  evidence: '\"compliant with GDPR and ITAR\"'\n- name: ITAR\n  status: supported\n  evidence: >-\n    \"Built on the foundations of SOC 2, ITAR, GDPR, and AWS security best practices.\"\nassurance:\n  third_party_pentest: annual\n  audit_cadence: annual\n  evidence: >-\n\
  \    \"conducts annual third-party penetration testing\" / \"audited annually by a third party\"\ncontrols:\n- Single-tenant - dedicated infrastructure and a dedicated AWS VPC for each customer\n- Data encrypted at rest and in flight\n- Secure HTTPS browser access\n- Outbound-only data upload - no inbound connections to the customer network required\n- SAML 2.0 SSO and identity federation (Okta, Azure AD, Microsoft 365)\n- Role-based access controls, customer-controlled user access and permissions\n- Customer-selectable AWS region for data residency\nevidence:\n- source: https://www.voltaiq.com/security\n  status: 200\n  keywords:\n  - soc 2 type ii\n  - gdpr\n  - itar\n  - saml 2.0\n  - penetration testing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltaiq/refs/heads/main/security/voltaiq-trust-center.yml
summary_line: SOC 2 Type II, GDPR, ITAR
tags:
- Company
- Batteries
- Energy Storage
- Manufacturing
- Analytics
- Industrial IoT
- Data Management
- Quality
- Electric Vehicles
- Enterprise Software
trust_url: https://www.voltaiq.com/security
---
