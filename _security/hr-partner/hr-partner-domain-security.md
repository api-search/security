---
api_specs:
- filename: hr-partner-rest-api-openapi.yml
  format: yaml
  label: HR Partner REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hr-partner/refs/heads/main/openapi/hr-partner-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hrpartner.io
  spf: true
hosts:
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: hrpartner.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: developer.hrpartner.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: api.hrpartner.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hr Partner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HR Partner, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HR Partner
provider_slug: hr-partner
slug: hr-partner-domain-security
source_filename: hr-partner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hrpartner.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: false\n- host: developer.hrpartner.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: false\n- host: api.hrpartner.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hrpartner.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hr-partner/refs/heads/main/security/hr-partner-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- HR
- HRIS
- Human Resources
- Employee Records
- Leave Management
- Recruitment
- Applicant Tracking
- Onboarding
- Performance Management
- Timesheets
- Expense Management
- Document Library
- eSignature
- SaaS
- Australia
---
