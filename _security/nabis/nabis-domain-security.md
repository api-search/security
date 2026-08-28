---
api_specs:
- filename: nabis-platform-api-v2-openapi.yml
  format: yaml
  label: Nabis Platform API v2
  slug: nabis-platform-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nabis/refs/heads/main/openapi/nabis-platform-api-v2-openapi.yml
- filename: nabis-platform-api-v1-openapi.json
  format: json
  label: Nabis Platform API v1 (deprecated)
  slug: nabis-platform-api-v1-deprecated
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nabis/refs/heads/main/openapi/nabis-platform-api-v1-openapi.json
- filename: nabis-universal-qr-code-openapi.yaml
  format: yaml
  label: Nabis Universal QR Code API (design specification)
  slug: nabis-universal-qr-code-api-design-specification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nabis/refs/heads/main/openapi/nabis-universal-qr-code-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nabis.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nabis.pro
  spf: false
hosts:
- cert_expires: Oct 21 02:25:06 2026 GMT
  host: www.nabis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: developers.nabis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: platform-api.nabis.pro
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nabis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nabis, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nabis
provider_slug: nabis
slug: nabis-domain-security
source_filename: nabis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nabis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 02:25:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.nabis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\n- host: platform-api.nabis.pro\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nabis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nabis.pro\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nx-notes:\n- host: platform-api.nabis.pro\n  detail: >-\n    The automated probe recorded hsts: null (the API host root returns a 404 JSON body). An\n    authenticated-path probe on 2026-08-26 of GET https://platform-api.nabis.pro/v2/nabis-days-off\n    returned HTTP 401 carrying Strict-Transport-Security:\
  \ max-age=15552000; includeSubDomains, plus\n    Content-Security-Policy, X-Content-Type-Options: nosniff, Referrer-Policy: no-referrer,\n    X-Frame-Options: SAMEORIGIN and Cross-Origin-Opener-Policy: same-origin. HSTS IS present on the\n    API host; the max-age is 180 days, shorter than the 365 days on www.nabis.com.\n- domain: nabis.pro\n  detail: >-\n    The API is served from nabis.pro, a second registrable domain with no SPF, no DMARC, no CAA and\n    no DNSSEC — weaker than nabis.com, which at least has SPF and DMARC (p=none). Developers are\n    told to call platform-api.nabis.pro by docs served from developers.nabis.com, so the two-domain\n    split is also a phishing surface: a consumer has no published way to tell a real nabis.pro\n    hostname from a lookalike.\n- host: developers.nabis.com\n  detail: HSTS not set on the developer portal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nabis/refs/heads/main/security/nabis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cannabis
- Distribution
- Wholesale
- Marketplace
- Logistics
- Supply Chain
- Inventory
- Orders
- Invoicing
- Retail
- Compliance
- Track and Trace
- California
- New York
---
