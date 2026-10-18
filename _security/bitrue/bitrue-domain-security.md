---
api_specs:
- filename: bitrue-bitrue-api-api-openapi.yml
  format: yaml
  label: Bitrue Bitrue API
  slug: bitrue-bitrue-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-bitrue-api-api-openapi.yml
- filename: bitrue-etf-api-openapi.yml
  format: yaml
  label: Bitrue Etf API
  slug: bitrue-etf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-etf-api-openapi.yml
- filename: bitrue-fapi-api-openapi.yml
  format: yaml
  label: Bitrue Fapi API
  slug: bitrue-fapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-fapi-api-openapi.yml
- filename: bitrue-history-api-openapi.yml
  format: yaml
  label: Bitrue History API
  slug: bitrue-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-history-api-openapi.yml
- filename: bitrue-market-api-openapi.yml
  format: yaml
  label: Bitrue Market API
  slug: bitrue-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-market-api-openapi.yml
- filename: bitrue-mytrades-api-openapi.yml
  format: yaml
  label: Bitrue My Trades API
  slug: bitrue-mytrades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-mytrades-api-openapi.yml
- filename: bitrue-order-api-openapi.yml
  format: yaml
  label: Bitrue Order API
  slug: bitrue-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-order-api-openapi.yml
- filename: bitrue-poseidon-api-openapi.yml
  format: yaml
  label: Bitrue Poseidon API
  slug: bitrue-poseidon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-poseidon-api-openapi.yml
- filename: bitrue-sapi-api-openapi.yml
  format: yaml
  label: Bitrue Sapi API
  slug: bitrue-sapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-sapi-api-openapi.yml
- filename: bitrue-ticker-api-openapi.yml
  format: yaml
  label: Bitrue Ticker API
  slug: bitrue-ticker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-ticker-api-openapi.yml
- filename: bitrue-user-stream-api-openapi.yml
  format: yaml
  label: Bitrue User Stream API
  slug: bitrue-user-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-user-stream-api-openapi.yml
- filename: bitrue-withdraw-api-openapi.yml
  format: yaml
  label: Bitrue Withdraw API
  slug: bitrue-withdraw-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/openapi/bitrue-withdraw-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 iodef "mailto:support@bitrue.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bitrue.com
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: www.bitrue.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: openapi.bitrue.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: fapi.bitrue.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Bitrue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitrue, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bitrue
provider_slug: bitrue
slug: bitrue-domain-security
source_filename: bitrue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bitrue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openapi.bitrue.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\n- host: fapi.bitrue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bitrue.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:support@bitrue.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitrue/refs/heads/main/security/bitrue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Futures
- Market Data
- WebSocket
---
