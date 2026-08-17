---
api_specs:
- filename: appsamurai-campaign-spend-api-openapi.yml
  format: yaml
  label: Appsamurai Campaign Spend API
  slug: appsamurai-campaign-spend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-campaign-spend-api-openapi.yml
- filename: appsamurai-storyly-external-api-openapi.json
  format: json
  label: Appsamurai Storyly External API
  slug: appsamurai-storyly-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-storyly-external-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appsamurai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_pct: 5
  dmarc_policy: quarantine
  dmarc_rua: mailto:admin@storyly.io
  dnssec: false
  domain: storyly.io
  spf: true
hosts:
- cert_expires: Oct 15 15:04:59 2026 GMT
  host: appsamurai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 08:20:21 2026 GMT
  host: help.appsamurai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: 308-redirects to appsamurai.com/help/.
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.appsamurai.com
  hsts: null
  http_status: 500
  https: true
  note: Answers JSON 500 on every path including root. Documented as http:// in the Help Center; :80 does 301 to https.
  tls_version: TLSv1.2
- cert_expires: Oct  2 12:32:41 2026 GMT
  host: www.storyly.io
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:11:57 2026 GMT
  host: storyly.io
  hsts: true
  hsts_max_age: 31536000
  http_status: 301
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.storyly.io
  hsts: false
  http_status: 404
  https: true
  note: Storyly External API host. No HSTS. CORS is wide open - Access-Control-Allow-Origin '*' with Allow-Credentials 'true'.
  tls_version: TLSv1.3
- cert_expires: Oct  9 07:02:45 2026 GMT
  host: docs.storyly.io
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: mcp.storyly.io
  hsts: false
  http_status: 404
  https: true
  note: MCP server host. Root 404s; /mcp and /sse answer.
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: dashboard.storyly.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appsamurai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appsamurai, probed live across 9 host(s) and 2 registrable domain(s). 9 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Appsamurai
provider_slug: appsamurai
slug: appsamurai-domain-security
source_filename: appsamurai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (2026-08-13)\nnotes: >-\n  Round 2 added the storyly.io hosts, which is where App Samurai's live API,\n  documentation and MCP surfaces actually run. Two findings worth naming.\n  First, TLS posture is good almost everywhere - TLSv1.3 and HSTS on every\n  storyly.io host that serves a site - but the two API hosts themselves,\n  api.appsamurai.com and api.storyly.io, send NO HSTS header, and\n  api.appsamurai.com is still on TLSv1.2.\n  Second, the AppSamurai Campaign Spend API is DOCUMENTED over cleartext:\n  the Help Center article publishes the base URL as\n  http://api.appsamurai.com/api/customer-pull/spent/{api_key}, and the API key is\n  a path segment. The host does 301 from :80 to TLS, so the credential is not\n  necessarily transmitted in the clear, but a documented http:// URL carrying a\n  secret in its path is a real defect in the published guidance.\n  Neither domain\
  \ has DNSSEC or a CAA record. Both publish SPF and DMARC;\n  appsamurai.com's DMARC policy is p=none (monitor only) and storyly.io's is\n  p=quarantine at pct=5, so neither is meaningfully enforcing.\n\nhosts:\n- host: appsamurai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:04:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.appsamurai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 08:20:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: 308-redirects to appsamurai.com/help/.\n- host: api.appsamurai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\n  http_status: 500\n  note: >-\n    Answers JSON 500 on every path including root. Documented as http:// in the\n    Help Center; :80 does 301 to https.\n- host: www.storyly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:32:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  http_status: 200\n- host:\
  \ storyly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:11:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  http_status: 301\n- host: api.storyly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n  http_status: 404\n  note: >-\n    Storyly External API host. No HSTS. CORS is wide open -\n    Access-Control-Allow-Origin '*' with Allow-Credentials 'true'.\n- host: docs.storyly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 07:02:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  http_status: 200\n- host: mcp.storyly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: false\n  http_status: 404\n  note: MCP server host. Root 404s; /mcp and /sse answer.\n- host: dashboard.storyly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  http_status:\
  \ 200\n\ndomains:\n- domain: appsamurai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: storyly.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 5\n  dmarc_rua: mailto:admin@storyly.io\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/security/appsamurai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile
- Advertising
- User Acquisition
- Marketing
- App Growth
- Attribution
- Analytics
- Mobile Marketing
- SDK
- Storyly
- Content Experience
- In-App Stories
- MCP
- Mobile Commerce
---
