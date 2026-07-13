---
api_specs:
- filename: llms.txt
  format: yaml
  label: Bithumb REST API
  slug: bithumb-rest-api
  spec_type: OpenAPI
  url: https://apidocs.bithumb.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bithumb.com
  spf: true
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.bithumb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 08:40:17 2026 GMT
  host: apidocs.bithumb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: api.bithumb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bithumb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bithumb, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bithumb
provider_slug: bithumb
slug: bithumb-domain-security
source_filename: bithumb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bithumb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: false\n- host: apidocs.bithumb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:40:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bithumb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bithumb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bithumb/refs/heads/main/security/bithumb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Exchange
- Trading
- South Korea
- KRW
- Bitcoin
- Market Data
- WebSocket
---
