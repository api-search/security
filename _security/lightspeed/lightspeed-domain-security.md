---
api_specs:
- filename: reference
  format: yaml
  label: Lightspeed Retail X-Series API
  slug: retail-x-series
  spec_type: OpenAPI
  url: https://x-series-api.lightspeedhq.com/reference
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lightspeedhq.com
  spf: true
hosts:
- cert_expires: Sep 30 14:22:13 2026 GMT
  host: www.lightspeedhq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 01:41:30 2026 GMT
  host: x-series-api.lightspeedhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.lightspeedhq.com
  https: false
kind: domain-security
layout: security
method: probed
name: Lightspeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightspeed Commerce, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lightspeed Commerce
provider_slug: lightspeed
slug: lightspeed-domain-security
source_filename: lightspeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lightspeedhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:22:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: x-series-api.lightspeedhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:41:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lightspeedhq.com\n  https: false\ndomains:\n- domain: lightspeedhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightspeed/refs/heads/main/security/lightspeed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Point of Sale
- POS
- Retail
- Restaurant
- Inventory
- Loyalty
- Payments
- E-Commerce
- Omnichannel
---
