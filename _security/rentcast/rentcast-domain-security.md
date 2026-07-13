---
api_specs:
- filename: rentcast-openapi.json
  format: json
  label: RentCast API
  slug: rentcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentcast/refs/heads/main/openapi/rentcast-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rentcast.io
  spf: true
hosts:
- cert_expires: Sep 10 23:21:09 2026 GMT
  host: www.rentcast.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:48:02 2026 GMT
  host: developers.rentcast.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 11:25:02 2026 GMT
  host: app.rentcast.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rentcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RentCast, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RentCast
provider_slug: rentcast
slug: rentcast-domain-security
source_filename: rentcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rentcast.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:21:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.rentcast.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:48:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.rentcast.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:25:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: rentcast.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentcast/refs/heads/main/security/rentcast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Data
- Valuation
- Rental Market
- AVM
---
