---
api_specs:
- filename: centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 API
  slug: cms-blue-button-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-medicare-and-medicaid-services/refs/heads/main/openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cms.gov
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: www.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: bluebutton.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.bluebutton.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Centers For Medicare And Medicaid Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centers for Medicare and Medicaid Services, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Centers for Medicare and Medicaid Services
provider_slug: centers-for-medicare-and-medicaid-services
slug: centers-for-medicare-and-medicaid-services-domain-security
source_filename: centers-for-medicare-and-medicaid-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bluebutton.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bluebutton.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cms.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centers-for-medicare-and-medicaid-services/refs/heads/main/security/centers-for-medicare-and-medicaid-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- BCDA
- Blue Button
- CMS
- Claims
- DPC
- FHIR
- Federal Government
- Healthcare
- Interoperability
- Marketplace
- Medicaid
- Medicare
- Open Data
- Provider Data
- Socrata
---
