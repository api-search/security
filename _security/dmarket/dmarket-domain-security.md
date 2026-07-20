---
api_specs:
- filename: dmarket-trading-openapi.yml
  format: yaml
  label: DMarket Trading API
  slug: dmarket-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dmarket/refs/heads/main/openapi/dmarket-trading-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dmarket.com
  spf: true
hosts:
- cert_expires: Sep 28 11:38:36 2026 GMT
  host: dmarket.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 16:18:33 2026 GMT
  host: api.dmarket.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dmarket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DMarket, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DMarket
provider_slug: dmarket
slug: dmarket-domain-security
source_filename: dmarket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:38:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.dmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:18:33 2026 GMT\n  hsts: null\ndomains:\n- domain: dmarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dmarket/refs/heads/main/security/dmarket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Gaming
- Marketplace
- Trading
- Skins
- In-Game Items
- Blockchain
---
