---
api_specs:
- filename: stamped-merchant-data-openapi.json
  format: json
  label: Stamped Merchant Data API (V3)
  slug: stamped-merchant-data-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamped/refs/heads/main/openapi/stamped-merchant-data-openapi.json
- filename: stamped-loyalty-operations-openapi.json
  format: json
  label: Stamped Loyalty Operations API (V3)
  slug: stamped-loyalty-operations-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamped/refs/heads/main/openapi/stamped-loyalty-operations-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stamped.io
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: stamped.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 02:51:16 2026 GMT
  host: developers.stamped.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stamped Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stamped, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stamped
provider_slug: stamped
slug: stamped-domain-security
source_filename: stamped-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stamped.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\n- host: developers.stamped.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 02:51:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stamped.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stamped/refs/heads/main/security/stamped-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Reviews
- Ratings
- Loyalty
- E-Commerce
- Customer Marketing
- Shopify
---
