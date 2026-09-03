---
api_specs:
- filename: openapi.json
  format: json
  label: TheCarApi REST API
  slug: thecarapi-rest-api
  spec_type: OpenAPI
  url: https://thecarapi.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thecarapi.com
  spf: false
hosts:
- cert_expires: Oct  8 11:06:43 2026 GMT
  host: thecarapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 16:02:07 2026 GMT
  host: api.thecarapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thecarapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheCarApi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TheCarApi
provider_slug: thecarapi
slug: thecarapi-domain-security
source_filename: thecarapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thecarapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:06:43 2026 GMT\n  hsts: false\n- host: api.thecarapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 16:02:07 2026 GMT\n  hsts: null\ndomains:\n- domain: thecarapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thecarapi/refs/heads/main/security/thecarapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Automotive
- Vehicle Data
- Car Auctions
- Used Cars
- Vehicle Inventory
- Classifieds
- Market Intelligence
- Pricing
- VIN
- Image CDN
- Europe
- Korea
- Japan Auctions
---
