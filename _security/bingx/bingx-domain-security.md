---
api_specs:
- filename: bingx-account-api-openapi.yml
  format: yaml
  label: BingX Account API
  slug: bingx-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-account-api-openapi.yml
- filename: bingx-agent-api-openapi.yml
  format: yaml
  label: BingX Agent API
  slug: bingx-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-agent-api-openapi.yml
- filename: bingx-coin-m-futures-api-openapi.yml
  format: yaml
  label: BingX Coin-M Futures API
  slug: bingx-coin-m-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-coin-m-futures-api-openapi.yml
- filename: bingx-copy-trading-api-openapi.yml
  format: yaml
  label: BingX Copy Trading API
  slug: bingx-copy-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-copy-trading-api-openapi.yml
- filename: bingx-fund-api-openapi.yml
  format: yaml
  label: BingX Fund API
  slug: bingx-fund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-fund-api-openapi.yml
- filename: bingx-other-api-openapi.yml
  format: yaml
  label: BingX Other API
  slug: bingx-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-other-api-openapi.yml
- filename: bingx-perpetual-futures-usdt-m-api-openapi.yml
  format: yaml
  label: BingX Perpetual Futures (USDT-M) API
  slug: bingx-perpetual-futures-usdt-m-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-perpetual-futures-usdt-m-api-openapi.yml
- filename: bingx-social-api-openapi.yml
  format: yaml
  label: BingX Social API
  slug: bingx-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-social-api-openapi.yml
- filename: bingx-spot-api-openapi.yml
  format: yaml
  label: BingX Spot API
  slug: bingx-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-spot-api-openapi.yml
- filename: bingx-sub-account-api-openapi.yml
  format: yaml
  label: BingX Sub Account API
  slug: bingx-sub-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-sub-account-api-openapi.yml
- filename: bingx-user-data-stream-api-openapi.yml
  format: yaml
  label: BingX User Data Stream API
  slug: bingx-user-data-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-user-data-stream-api-openapi.yml
- filename: bingx-wallet-api-openapi.yml
  format: yaml
  label: BingX Wallet API
  slug: bingx-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-wallet-api-openapi.yml
- filename: bingx-wealth-api-openapi.yml
  format: yaml
  label: BingX Wealth API
  slug: bingx-wealth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/openapi/bingx-wealth-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bingx.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: bingx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bingx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BingX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BingX
provider_slug: bingx
slug: bingx-domain-security
source_filename: bingx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bingx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bingx.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bingx/refs/heads/main/security/bingx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Financial Services
---
