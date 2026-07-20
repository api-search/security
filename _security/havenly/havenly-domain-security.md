---
api_specs:
- filename: havenly-openapi.yml
  format: yaml
  label: Havenly API
  slug: havenly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: havenly.com
  spf: true
hosts:
- cert_expires: Oct  3 23:30:48 2026 GMT
  host: havenly.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:43:03 2026 GMT
  host: api-docs.havenly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:43:03 2026 GMT
  host: api.havenly.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Havenly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Havenly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Havenly
provider_slug: havenly
slug: havenly-domain-security
source_filename: havenly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: havenly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:30:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api-docs.havenly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:43:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.havenly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:43:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: havenly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/security/havenly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Interior Design
- Home Decor
- Furniture
- E-Commerce
- Marketplace
- Design
- Retail
- AI
---
