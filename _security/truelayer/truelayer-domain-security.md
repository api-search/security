---
api_specs:
- filename: truelayer-payments-openapi.yml
  format: yaml
  label: TrueLayer Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truelayer/refs/heads/main/openapi/truelayer-payments-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: truelayer.com
  spf: true
hosts:
- cert_expires: Sep 14 20:45:01 2026 GMT
  host: truelayer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:30:37 2026 GMT
  host: docs.truelayer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 18:14:12 2026 GMT
  host: api.truelayer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truelayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrueLayer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TrueLayer
provider_slug: truelayer
slug: truelayer-domain-security
source_filename: truelayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truelayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:45:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.truelayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:30:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.truelayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:14:12 2026 GMT\n  hsts: null\ndomains:\n- domain: truelayer.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truelayer/refs/heads/main/security/truelayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data API
- Financial Services
- Open Banking
- Payments
- PSD2
- UK Banking
- VRP
---
