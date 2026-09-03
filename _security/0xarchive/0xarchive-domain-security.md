---
api_specs:
- filename: openapi.json
  format: json
  label: 0xArchive REST API
  slug: 0xarchive-rest-api
  spec_type: OpenAPI
  url: https://0xarchive.io/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 0xarchive.io
  spf: true
hosts:
- cert_expires: Oct  3 21:34:14 2026 GMT
  host: docs.0xarchive.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 08:18:05 2026 GMT
  host: api.0xarchive.io
  hsts: true
  hsts_max_age: 31536000
  hsts_note: 'The automated probe recorded hsts: null for this host; a direct HEAD of https://api.0xarchive.io/health on 2026-09-01 returned "strict-transport-security: max-age=31536000; includeSubDomains", so HSTS IS served. The probe''s null is most likely because every path on this host except /health answers 401. Corrected here with the observation that established it.'
  https: true
  security_headers_observed:
  - 'strict-transport-security: max-age=31536000; includeSubDomains'
  - 'x-content-type-options: nosniff'
  - 'x-frame-options: DENY'
  - 'referrer-policy: strict-origin-when-cross-origin'
  - 'x-xss-protection: 1; mode=block'
  security_headers_source: HEAD https://api.0xarchive.io/health, 2026-09-01
  tls_version: TLSv1.3
- cert_expires: Oct 12 06:51:22 2026 GMT
  host: mcp.0xarchive.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 0Xarchive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 0xArchive, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 0xArchive
provider_slug: 0xarchive
slug: 0xarchive-domain-security
source_filename: 0xarchive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.0xarchive.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:34:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.0xarchive.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 08:18:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_note: >-\n    The automated probe recorded hsts: null for this host; a direct HEAD of\n    https://api.0xarchive.io/health on 2026-09-01 returned\n    \"strict-transport-security: max-age=31536000; includeSubDomains\", so HSTS IS served. The\n    probe's null is most likely because every path on this host except /health answers 401.\n    Corrected here with the observation that established it.\n  security_headers_observed:\n  - 'strict-transport-security: max-age=31536000; includeSubDomains'\n  - 'x-content-type-options: nosniff'\n  - 'x-frame-options: DENY'\n  - 'referrer-policy:\
  \ strict-origin-when-cross-origin'\n  - 'x-xss-protection: 1; mode=block'\n  security_headers_source: HEAD https://api.0xarchive.io/health, 2026-09-01\n- host: mcp.0xarchive.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 06:51:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 0xarchive.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nx-pipeline-note: >-\n  The automated probe covered the three hosts named in apis.yml apis[].baseURL and the OpenAPI\n  servers[] block. The apex host 0xarchive.io was probed separately during this pass and is\n  recorded below; it is the host that serves security.txt and the api-catalog.\nextra_hosts:\n- host: 0xarchive.io\n  https: true\n  http_status: 200\n  security_txt: true\n  security_txt_url: https://0xarchive.io/.well-known/security.txt\n  checked: '2026-09-01'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/0xarchive/refs/heads/main/security/0xarchive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- market data
- historical data
- crypto
- DeFi
- perpetuals
- derivatives
- order book
- Hyperliquid
- Lighter
- HIP-3
- HIP-4
- prediction markets
- WebSocket
- streaming
- historical replay
- Parquet
- bulk data
- MCP
- agent-native
- x402
- OpenAPI
- REST
---
