---
api_specs:
- filename: plug-openapi-original.yml
  format: yaml
  label: Malga API
  slug: malga-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: malga.io
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: malga.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 16:56:13 2026 GMT
  host: docs.malga.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: api.malga.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plug Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Malga, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Malga
provider_slug: plug
slug: plug-domain-security
source_filename: plug-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: malga.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\n- host: docs.malga.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:56:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.malga.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: malga.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/security/plug-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Payment Orchestration
- Payment Gateway
- Fintech
- Pix
- Tokenization
- Subscriptions
- Brazil
---
