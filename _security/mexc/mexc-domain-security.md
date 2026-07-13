---
api_specs:
- filename: mexc-spot-rest-api-openapi.json
  format: json
  label: MEXC Spot REST API
  slug: spot-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-spot-rest-api-openapi.json
- filename: mexc-futures-rest-api-openapi.json
  format: json
  label: MEXC Futures REST API
  slug: futures-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/openapi/mexc-futures-rest-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mexc.com
  spf: true
hosts:
- cert_expires: Sep 23 10:18:41 2026 GMT
  host: www.mexc.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 10:18:41 2026 GMT
  host: api.mexc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: wbs-api.mexc.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mexc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MEXC, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MEXC
provider_slug: mexc
slug: mexc-domain-security
source_filename: mexc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mexc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 10:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mexc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 10:18:41 2026 GMT\n  hsts: null\n- host: wbs-api.mexc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mexc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mexc/refs/heads/main/security/mexc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Exchange
- Trading
- Futures
- Market Data
- Finance
- Blockchain
---
