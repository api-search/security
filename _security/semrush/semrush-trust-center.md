---
api_specs:
- filename: semrush-hermes-partner-api-api-openapi.yml
  format: yaml
  label: Semrush Hermes Partner API API
  slug: semrush-hermes-partner-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-hermes-partner-api-api-openapi.yml
- filename: semrush-jwt-issuer-api-openapi.yml
  format: yaml
  label: Semrush JWT Issuer API
  slug: semrush-jwt-issuer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-jwt-issuer-api-openapi.yml
- filename: semrush-partner-service-api-openapi.yml
  format: yaml
  label: Semrush Partner Service API
  slug: semrush-partner-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-partner-service-api-openapi.yml
certifications:
- PCI DSS
- GDPR
- CCPA
- LGPD
description: Semrush publishes a public security page in place of a trust center. It is prose rather than a portal — there is no document request flow, no downloadable audit report, and no subprocessor list linked from it — but it names concrete compliance programs and describes the controls behind them. It is localized into fourteen languages, which is unusual and suggests it is treated as a sales artifact.
kind: trust-center
layout: security
name: Semrush Trust Center
name_suffix: Trust Center
overview: Semrush maintains a public trust center documenting PCI DSS, GDPR, CCPA, and LGPD compliance.
provider_name: Semrush
provider_slug: semrush
slug: semrush-trust-center
source_filename: semrush-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.semrush.com/company/security/\nprovider: Semrush\nproviderId: semrush\ndescription: >-\n  Semrush publishes a public security page in place of a trust center. It is prose rather\n  than a portal — there is no document request flow, no downloadable audit report, and no\n  subprocessor list linked from it — but it names concrete compliance programs and describes\n  the controls behind them. It is localized into fourteen languages, which is unusual and\n  suggests it is treated as a sales artifact.\n\ntrust_center:\n  exists: true\n  type: security-page\n  url: https://www.semrush.com/company/security/\n  portal: false\n  document_request_flow: false\n  subprocessor_list_linked: false\n  localized:\n  - de\n  - es\n  - fr\n  - it\n  - ja\n  - ko\n  - nl\n  - pl\n  - pt\n  - sv\n  - tr\n  - vi\n  - zh\n\ncertifications:\n- name: PCI DSS\n  status: compliant\n  attestation: >-\n    \"We have fully implemented and support\
  \ all processes related to PCI DSS compliance. Once\n    a year, we confirm our compliance by passing an independent QSA audit.\"\n  audit_cadence: annual\n  auditor_type: independent QSA\n  report_available: false\n- name: GDPR\n  status: compliant\n  effective: '2018-05-25'\n  attestation: >-\n    Semrush states its products adhere to GDPR requirements, with data-minimization measures\n    described on the page.\n- name: CCPA\n  status: monitored\n  attestation: >-\n    Semrush states it monitors and complies with CCPA, LGPD and other national privacy\n    legislation.\n- name: LGPD\n  status: monitored\n\nnot_claimed:\n- name: SOC 2\n  note: >-\n    No SOC 2 Type I or Type II claim appears anywhere on the security page. Notable for a\n    data platform of this size selling to enterprise.\n- name: ISO/IEC 27001\n  note: No ISO 27001 certification is claimed.\n- name: HIPAA\n- name: FedRAMP\n\ncontrol_domains_described:\n- Information security policies, reviewed and communicated to affected\
  \ personnel\n- HR security — NDAs for employees and contractors, annual security awareness training\n- Application security — separate staging, testing and development environments\n- Weekly penetration testing of new features\n- Patch management across company infrastructure\n- Physical security and compliance of data centers\n\ninfrastructure:\n  providers:\n  - name: AWS\n    compliance_reference: https://aws.amazon.com/compliance/\n  - name: Google Cloud\n    compliance_reference: https://cloud.google.com/security/compliance\n  - name: Digital Realty\n    compliance_reference: https://www.digitalrealty.com/data-center-solutions/security-compliance/compliance\n  note: >-\n    Semrush points at its data-center providers' compliance certificates rather than holding\n    an equivalent certification of its own at the application layer.\n\ncontact: security@semrush.com\nlegal:\n  privacy_policy: https://www.semrush.com/company/legal/privacy-policy/\n  terms_of_service: https://www.semrush.com/company/legal/terms-of-service/\n\
  \nx-evidence:\n- url: https://www.semrush.com/company/security/\n  http_status: 200\n- url: https://trust.semrush.com/\n  http_status: null\n  note: DNS does not resolve — no dedicated trust-center subdomain exists.\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/security/semrush-trust-center.yml
summary_line: PCI DSS, GDPR, CCPA, LGPD
tags:
- Data
- Search Engines
- SEO
- Marketing
- Marketing Intelligence
- Content Marketing
- Advertising
- Competitive Intelligence
- Keyword Research
- Backlinks
- Rank Tracking
- AI Search Visibility
- Local SEO
- MCP
trust_url: ''
---
