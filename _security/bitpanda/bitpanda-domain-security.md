---
api_specs:
- filename: bitpanda-platform-openapi.yml
  format: yaml
  label: Bitpanda Platform API
  slug: bitpanda-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpanda/refs/heads/main/openapi/bitpanda-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bitpanda.com
  spf: true
hosts:
- cert_expires: Oct  9 16:17:50 2026 GMT
  host: bitpanda.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 22:29:42 2026 GMT
  host: developers.bitpanda.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 13:15:05 2026 GMT
  host: developer.bitpanda.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitpanda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitpanda, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bitpanda
provider_slug: bitpanda
slug: bitpanda-domain-security
source_filename: bitpanda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitpanda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:17:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.bitpanda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:29:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.bitpanda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 13:15:05 2026 GMT\n  hsts: null\ndomains:\n- domain: bitpanda.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitpanda/refs/heads/main/security/bitpanda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Fintech
- Trading
- Investing
- Stocks
- ETFs
- Precious Metals
- Portfolio
- Market Data
- MCP
- Agent Skills
---
