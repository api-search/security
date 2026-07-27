---
api_specs:
- filename: knight-frank-api-v3-openapi.json
  format: json
  label: KnightFrank Api v3
  slug: knight-frank-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/openapi/knight-frank-api-v3-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knightfrank.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prd-knightfrank.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.knightfrank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: api-v3.web.prd-knightfrank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knight Frank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knight Frank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Knight Frank
provider_slug: knight-frank
slug: knight-frank-domain-security
source_filename: knight-frank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.knightfrank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-v3.web.prd-knightfrank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: knightfrank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: prd-knightfrank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/security/knight-frank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- United Kingdom
- Property Listings
- Commercial Real Estate
- Valuation
- Brokerage
- Property Management
- Rentals
- PropTech
- Research
---
