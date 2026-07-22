---
api_specs:
- filename: meow-openapi.yaml
  format: yaml
  label: Meow API
  slug: meow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meow/refs/heads/main/openapi/meow-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meow.com
  spf: true
hosts:
- cert_expires: Sep 16 14:25:58 2026 GMT
  host: www.meow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meow
provider_slug: meow
slug: meow-domain-security
source_filename: meow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:25:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: meow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meow/refs/heads/main/security/meow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Fintech
- Business Banking
- Payments
- Cards
- Invoicing
- Treasury
- Cryptocurrency
- Webhooks
- MCP
- API
---
