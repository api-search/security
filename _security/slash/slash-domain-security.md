---
api_specs:
- filename: slash-openapi-original.json
  format: json
  label: Slash Public API
  slug: slash-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slash/refs/heads/main/openapi/slash-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: slash.com
  spf: true
hosts:
- cert_expires: Oct 11 10:20:24 2026 GMT
  host: slash.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 02:00:17 2026 GMT
  host: api.slash.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slash, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Slash
provider_slug: slash
slug: slash-domain-security
source_filename: slash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 10:20:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.slash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 02:00:17 2026 GMT\n  hsts: null\ndomains:\n- domain: slash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slash/refs/heads/main/security/slash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Payments
- Financial Services
- Fintech
- Corporate Cards
- Business Banking
- Invoicing
- Expense Management
- Treasury
- FDX
---
