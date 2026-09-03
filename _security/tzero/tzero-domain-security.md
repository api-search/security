---
api_specs:
- filename: tzero-issuance-secondary-markets-openapi.json
  format: json
  label: tZERO Issuance & Secondary Markets API
  slug: issuance-secondary-markets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tzero/refs/heads/main/openapi/tzero-issuance-secondary-markets-openapi.json
- filename: tzero-institutional-openapi.json
  format: json
  label: tZERO Institutional API
  slug: institutional
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tzero/refs/heads/main/openapi/tzero-institutional-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tzero.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: t0direct.com
  method: probed-by-hand
  spf: false
hosts:
- cert_expires: Nov  2 07:28:10 2026 GMT
  host: www.tzero.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 04:36:49 2026 GMT
  host: apidocs.tzero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:43:17 2026 GMT
  host: gateway-web-api.tzero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 20:50:59 2026 GMT
  host: api.t0direct.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  method: probed-by-hand
  tls_version: TLSv1.3
- cert_expires: Oct 30 00:25:27 2026 GMT
  host: platform.tzero.com
  https: true
  method: probed-by-hand
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tzero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tZERO, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: tZERO
provider_slug: tzero
slug: tzero-domain-security
source_filename: tzero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 07:28:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.tzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 04:36:49 2026 GMT\n  hsts: false\n- host: gateway-web-api.tzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:43:17 2026 GMT\n  hsts: null\n- host: api.t0direct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 20:50:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  method: probed-by-hand\n- host: platform.tzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 00:25:27 2026 GMT\n  method: probed-by-hand\ndomains:\n- domain: tzero.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: t0direct.com\n  dnssec:\
  \ false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  method: probed-by-hand\nnote: The mechanical probe reads apis.yml Website/Portal/humanURL/baseURL and OpenAPI servers[]. api.t0direct.com\n  and platform.tzero.com were probed by hand on the same day with the same method and appended below; t0direct.com\n  is a second registrable domain tZERO operates for its institutional surface and it carries no DNSSEC, CAA, SPF\n  or DMARC record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tzero/refs/heads/main/security/tzero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Digital Securities
- Tokenization
- Capital Markets
- Trading
- Alternative Trading System
- Transfer Agent
- Custody
- Blockchain
- Financial Services
- Securities
- Market Data
- FIX Protocol
---
