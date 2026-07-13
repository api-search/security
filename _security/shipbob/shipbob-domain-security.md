---
api_specs:
- filename: shipbob-openapi.json
  format: json
  label: ShipBob Developer API
  slug: shipbob-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shipbob.com
  spf: true
hosts:
- cert_expires: Sep 23 15:51:24 2026 GMT
  host: www.shipbob.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:30:22 2026 GMT
  host: developer.shipbob.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 15:51:24 2026 GMT
  host: api.shipbob.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shipbob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShipBob, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ShipBob
provider_slug: shipbob
slug: shipbob-domain-security
source_filename: shipbob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipbob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:51:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.shipbob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:30:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.shipbob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:51:24 2026 GMT\n  hsts: null\ndomains:\n- domain: shipbob.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/security/shipbob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Fulfillment
- 3PL
- Ecommerce
- Inventory
- Warehousing
- Shipping
- Direct-to-Consumer
---
