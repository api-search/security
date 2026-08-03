---
api_specs:
- filename: ascend-elements-wordpress-rest-openapi.yml
  format: yaml
  label: Ascend Elements WordPress REST API
  slug: ascend-elements-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ascend-elements/refs/heads/main/openapi/ascend-elements-wordpress-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ascendelements.com
  spf: true
hosts:
- cert_expires: Oct 28 16:15:29 2026 GMT
  edge: 'Cloudflare in front of WP Engine (server: cloudflare, x-powered-by: WP Engine)'
  host: ascendelements.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_note: 'The mechanical probe recorded hsts null because it HEADs the site root, and ascendelements.com answers every front-end HTML path with HTTP 503 (Retry-After: 600) to non-browser clients. HSTS was observed directly on the API host path instead: GET https://ascendelements.com/wp-json/wp/v2/posts returned `strict-transport-security: max-age=63072000; includeSubDomains;` on 2026-08-02.'
  https: true
  other_headers_observed:
  - 'x-content-type-options: nosniff'
  - 'x-robots-tag: noindex'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ascend Elements Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ascend Elements, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ascend Elements
provider_slug: ascend-elements
slug: ascend-elements-domain-security
source_filename: ascend-elements-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ascendelements.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 16:15:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    The mechanical probe recorded hsts null because it HEADs the site root, and\n    ascendelements.com answers every front-end HTML path with HTTP 503 (Retry-After: 600) to\n    non-browser clients. HSTS was observed directly on the API host path instead:\n    GET https://ascendelements.com/wp-json/wp/v2/posts returned\n    `strict-transport-security: max-age=63072000; includeSubDomains;` on 2026-08-02.\n  other_headers_observed:\n  - 'x-content-type-options: nosniff'\n  - 'x-robots-tag: noindex'\n  edge: 'Cloudflare in front of WP Engine (server: cloudflare, x-powered-by: WP Engine)'\ndomains:\n- domain: ascendelements.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ascend-elements/refs/heads/main/security/ascend-elements-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Battery Materials
- Battery Recycling
- Lithium-Ion
- Critical Minerals
- Cathode Precursor
- Electric Vehicles
- Circular Economy
- Advanced Manufacturing
- Sustainability
- Supply Chain
- Content Management
---
