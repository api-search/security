---
api_specs:
- filename: fyndiq-merchant-api-openapi.yml
  format: yaml
  label: Fyndiq Merchant API
  slug: fyndiq-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyndiq/refs/heads/main/openapi/fyndiq-merchant-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fyndiq.se
  spf: true
hosts:
- cert_expires: Oct 12 03:46:31 2026 GMT
  host: www.fyndiq.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:46:31 2026 GMT
  host: merchants-api.fyndiq.se
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:46:31 2026 GMT
  host: merchants-api.sandbox.fyndiq.se
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fyndiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fyndiq, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fyndiq
provider_slug: fyndiq
slug: fyndiq-domain-security
source_filename: fyndiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fyndiq.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:46:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: merchants-api.fyndiq.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:46:31 2026 GMT\n  hsts: null\n- host: merchants-api.sandbox.fyndiq.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:46:31 2026 GMT\n  hsts: null\ndomains:\n- domain: fyndiq.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fyndiq/refs/heads/main/security/fyndiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Marketplace
- E-Commerce
- Retail
- Products
- Orders
- Sweden
---
