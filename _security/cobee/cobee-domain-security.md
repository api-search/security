---
api_specs:
- filename: cobee-public-api-openapi-original.json
  format: json
  label: Cobee Public API
  slug: cobee-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cobee/refs/heads/main/openapi/cobee-public-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cobee.io
  spf: true
hosts:
- cert_expires: Oct 10 19:46:51 2026 GMT
  host: cobee.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: pre-public-api.cobee.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: public-api.cobee.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cobee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cobee by Pluxee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cobee by Pluxee
provider_slug: cobee
slug: cobee-domain-security
source_filename: cobee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cobee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 19:46:51 2026 GMT\n  hsts: false\n- host: pre-public-api.cobee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\n- host: public-api.cobee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cobee.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cobee/refs/heads/main/security/cobee-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Employee Benefits
- Compensation
- Human Resources
- Payroll
- Fintech
- Spain
- Flexible Benefits
---
