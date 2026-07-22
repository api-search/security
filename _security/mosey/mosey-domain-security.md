---
api_specs:
- filename: mosey-openapi.json
  format: json
  label: Mosey API
  slug: mosey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/openapi/mosey-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mosey.com
  spf: true
hosts:
- cert_expires: Sep 28 20:47:44 2026 GMT
  host: docs.mosey.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: api.mosey.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mosey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mosey, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mosey
provider_slug: mosey
slug: mosey-domain-security
source_filename: mosey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.mosey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:47:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mosey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mosey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosey/refs/heads/main/security/mosey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compliance
- Regulatory Technology
- State Compliance
- Tax
- Payroll
- HR
- Business Operations
---
