---
api_specs:
- filename: denim-openapi-original.json
  format: json
  label: Denim Public API
  slug: denim-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/openapi/denim-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: denim.com
  spf: true
hosts:
- cert_expires: Oct  2 03:22:10 2026 GMT
  host: denim.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 01:59:07 2026 GMT
  host: staging.denim.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Denim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Denim, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Denim
provider_slug: denim
slug: denim-domain-security
source_filename: denim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: denim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:22:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: staging.denim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:59:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: denim.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/denim/refs/heads/main/security/denim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Freight
- Factoring
- Payments
- Logistics
- Trucking
- Fintech
- Back Office
---
