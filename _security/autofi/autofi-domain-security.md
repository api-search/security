---
api_specs:
- filename: autofi-api-openapi.yml
  format: yaml
  label: AutoFi API
  slug: autofi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/openapi/autofi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: autofi.com
  spf: true
hosts:
- cert_expires: Oct 14 03:19:55 2026 GMT
  host: autofi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.autofi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api-uat.autofi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autofi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoFi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AutoFi
provider_slug: autofi
slug: autofi-domain-security
source_filename: autofi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autofi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 03:19:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.autofi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api-uat.autofi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: autofi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/security/autofi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Fintech
- Digital Retail
- Auto Finance
- Dealerships
- Sales Enablement
- Software-as-a-Service
- Lending
- Loan Origination
- Credit Decisioning
- Payment Calculation
- Prequalification
---
