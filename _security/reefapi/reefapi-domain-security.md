---
api_specs:
- filename: reefapi-openapi.json
  format: json
  label: ReefAPI REST API
  slug: reefapi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reefapi.com
  spf: true
hosts:
- cert_expires: Nov  3 01:42:48 2026 GMT
  host: reefapi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 01:42:48 2026 GMT
  host: api.reefapi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  hsts_note: 'Re-probed 2026-08-31. The automated pass recorded hsts null because GET https://api.reefapi.com/ returns 404 (the API is POST-only, path-scoped); the 404 response nevertheless carries ''strict-transport-security: max-age=15552000; includeSubDomains'', as does a POST to a real operation. HSTS is served.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reefapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReefAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ReefAPI
provider_slug: reefapi
slug: reefapi-domain-security
source_filename: reefapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reefapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 01:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.reefapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 01:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    Re-probed 2026-08-31. The automated pass recorded hsts null because\n    GET https://api.reefapi.com/ returns 404 (the API is POST-only, path-scoped);\n    the 404 response nevertheless carries\n    'strict-transport-security: max-age=15552000; includeSubDomains',\n    as does a POST to a real operation. HSTS is served.\ndomains:\n- domain: reefapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/security/reefapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- web-data
- data-aggregation
- web-scraping
- serp
- e-commerce
- social-media
- real-estate
- jobs
- travel
- news
- finance
- reviews
- company-intelligence
- mcp
- agent-native
- rest
- openapi
- llms-txt
- api-catalog
- free-tier
- credits
- gateway
---
