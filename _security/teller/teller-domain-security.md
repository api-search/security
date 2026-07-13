---
api_specs:
- filename: teller-openapi.yml
  format: yaml
  label: Teller API
  slug: teller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teller/refs/heads/main/openapi/teller-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: teller.io
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: teller.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: api.teller.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teller Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teller, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Teller
provider_slug: teller
slug: teller-domain-security
source_filename: teller-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teller.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.teller.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: teller.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teller/refs/heads/main/security/teller-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Financial Data
- FinTech
- Open Banking
- Transactions
- Unified API
---
