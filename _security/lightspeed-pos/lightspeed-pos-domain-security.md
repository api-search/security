---
api_specs:
- filename: lightspeed-pos-retail-x-series-openapi.yml
  format: yaml
  label: Lightspeed Retail X-Series API (Vend)
  slug: retail-x-series
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightspeed-pos/refs/heads/main/openapi/lightspeed-pos-retail-x-series-openapi.yml
- filename: lightspeed-pos-retail-r-series-openapi.yml
  format: yaml
  label: Lightspeed Retail R-Series API
  slug: retail-r-series
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightspeed-pos/refs/heads/main/openapi/lightspeed-pos-retail-r-series-openapi.yml
- filename: lightspeed-pos-restaurant-k-series-openapi.yml
  format: yaml
  label: Lightspeed Restaurant K-Series API
  slug: restaurant-k-series
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightspeed-pos/refs/heads/main/openapi/lightspeed-pos-restaurant-k-series-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lightspeedhq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lightspeedapp.com
  spf: true
hosts:
- cert_expires: Sep 21 01:41:30 2026 GMT
  host: x-series-api.lightspeedhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:22:13 2026 GMT
  host: developers.lightspeedhq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:30:16 2026 GMT
  host: api.lightspeedapp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightspeed Pos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightspeed, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lightspeed
provider_slug: lightspeed-pos
slug: lightspeed-pos-domain-security
source_filename: lightspeed-pos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: x-series-api.lightspeedhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:41:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.lightspeedhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:22:13 2026 GMT\n  hsts: false\n- host: api.lightspeedapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:30:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: lightspeedhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lightspeedapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightspeed-pos/refs/heads/main/security/lightspeed-pos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- POS
- Retail
- Restaurant
- Ecommerce
---
