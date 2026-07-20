---
api_specs:
- filename: hibachi-openapi.yml
  format: yaml
  label: Hibachi API
  slug: hibachi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hibachi/refs/heads/main/openapi/hibachi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: hibachi.xyz
  spf: true
hosts:
- cert_expires: Sep 10 22:08:54 2026 GMT
  host: hibachi.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 22:08:54 2026 GMT
  host: api.hibachi.xyz
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 22:08:54 2026 GMT
  host: data-api.hibachi.xyz
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hibachi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hibachi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Hibachi
provider_slug: hibachi
slug: hibachi-domain-security
source_filename: hibachi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hibachi.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 22:08:54 2026 GMT\n  hsts: null\n- host: api.hibachi.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 22:08:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: data-api.hibachi.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 22:08:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hibachi.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hibachi/refs/heads/main/security/hibachi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Defi
- Cryptocurrency
- Exchange
- Perpetual Futures
- Trading
- Derivatives
- Stablecoin
- WebSocket
- Blockchain
---
