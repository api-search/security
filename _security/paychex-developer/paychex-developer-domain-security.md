---
api_specs:
- filename: paychex-payroll-companies-openapi.yml
  format: yaml
  label: Paychex Payroll Companies API
  slug: paychex-payroll-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-payroll-companies-openapi.yml
- filename: paychex-workers-openapi.yml
  format: yaml
  label: Paychex Workers API
  slug: paychex-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-workers-openapi.yml
- filename: paychex-time-openapi.yml
  format: yaml
  label: Paychex Time API
  slug: paychex-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-time-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paychex.com
  spf: true
hosts:
- cert_expires: Aug 20 06:33:57 2026 GMT
  host: developer.paychex.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: api.paychex.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Paychex Developer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paychex, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paychex
provider_slug: paychex-developer
slug: paychex-developer-domain-security
source_filename: paychex-developer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.paychex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:33:57 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.paychex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: paychex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/security/paychex-developer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Benefits
- HCM
- HR
- Paychex Flex
- Payroll
- Time and Attendance
- Workforce
- Fortune 1000
---
