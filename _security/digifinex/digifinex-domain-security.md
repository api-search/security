---
api_specs:
- filename: digifinex-account-api-openapi.yml
  format: yaml
  label: DigiFinex Account API
  slug: digifinex-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-account-api-openapi.yml
- filename: digifinex-copy-trading-api-openapi.yml
  format: yaml
  label: DigiFinex Copy Trading API
  slug: digifinex-copy-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-copy-trading-api-openapi.yml
- filename: digifinex-margin-api-openapi.yml
  format: yaml
  label: DigiFinex Margin API
  slug: digifinex-margin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-margin-api-openapi.yml
- filename: digifinex-market-data-api-openapi.yml
  format: yaml
  label: DigiFinex Market Data API
  slug: digifinex-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-market-data-api-openapi.yml
- filename: digifinex-orders-api-openapi.yml
  format: yaml
  label: DigiFinex Orders API
  slug: digifinex-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-orders-api-openapi.yml
- filename: digifinex-trading-api-openapi.yml
  format: yaml
  label: DigiFinex Trading API
  slug: digifinex-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/openapi/digifinex-trading-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: digifinex.com
  spf: true
hosts:
- cert_expires: Dec 28 08:20:35 2026 GMT
  host: www.digifinex.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digifinex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DigiFinex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DigiFinex
provider_slug: digifinex
slug: digifinex-domain-security
source_filename: digifinex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digifinex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 08:20:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: digifinex.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digifinex/refs/heads/main/security/digifinex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Derivatives
- WebSocket
---
