---
api_specs:
- filename: optum-dental-attachment-api-openapi.yml
  format: yaml
  label: Optum Medical Network Eligibility and Claims API
  slug: optum-medical-network-eligibility-and-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-dental-attachment-api-openapi.yml
- filename: optum-attachment-openapi.yml
  format: yaml
  label: Optum Real (Medical) API
  slug: optum-real-medical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-attachment-openapi.yml
- filename: optum-dental-pre-care-estimate-api-openapi.yml
  format: yaml
  label: Optum Real for Dental API
  slug: optum-real-for-dental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-dental-pre-care-estimate-api-openapi.yml
- filename: optum-formatting-rule-api-openapi.yml
  format: yaml
  label: Optum Pharmacy Solutions API
  slug: optum-pharmacy-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-formatting-rule-api-openapi.yml
- filename: optum-edi-enrollment-v1-openapi.yml
  format: yaml
  label: Optum Payment and Reimbursement API
  slug: optum-payment-and-reimbursement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-edi-enrollment-v1-openapi.yml
- filename: optum-cms-common-facility-openapi.yml
  format: yaml
  label: Optum Insight Platform (Platform and Interoperability) API
  slug: optum-insight-platform-platform-and-interoperability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-cms-common-facility-openapi.yml
- filename: optum-abm-care-decision-support-api-openapi.yml
  format: yaml
  label: Optum Analytics and Insights API
  slug: optum-analytics-and-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-abm-care-decision-support-api-openapi.yml
- filename: optum-security-and-authorization-v2-openapi.yml
  format: yaml
  label: Optum API Tools — Security and Authorization
  slug: optum-api-tools-security-and-authorization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-security-and-authorization-v2-openapi.yml
description: ''
domains:
- caa:
  - 0 issuemail "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: optum.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.optum.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 12:43:52 2026 GMT
  host: developer.optum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 05:03:48 2026 GMT
  host: apigw.optum.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Optum
provider_slug: optum
slug: optum-domain-security
source_filename: optum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.optum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.optum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 12:43:52 2026 GMT\n  hsts: null\n- host: apigw.optum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 05:03:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: optum.com\n  dnssec: true\n  caa:\n  - 0 issuemail \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/security/optum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health Insurance
- Claims
- Eligibility
- FHIR
- Interoperability
- Pharmacy
- EDI
- X12
- Payments
- Prior Authorization
- Clearinghouse
- Revenue Cycle
- Dental
- Da Vinci
- Patient Access
- Remittance
- Attachments
- Payer Directory
---
