---
api_specs:
- filename: moov-api-openapi.yml
  format: yaml
  label: Moov API
  slug: moov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/openapi/moov-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moov.io
  spf: true
hosts:
- cert_expires: Oct  6 21:33:43 2026 GMT
  host: docs.moov.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 18:49:20 2026 GMT
  host: moov.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: api.moov.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moov, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moov
provider_slug: moov
slug: moov-domain-security
source_filename: moov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.moov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:33:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: moov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:49:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moov.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moov.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/security/moov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Embedded Finance
- Financial Infrastructure
- Money Movement
- Payments
- Transfers
---
