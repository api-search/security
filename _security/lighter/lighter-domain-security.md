---
api_specs:
- filename: lighter-account-api-openapi.yml
  format: yaml
  label: Lighter account API
  slug: lighter-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-account-api-openapi.yml
- filename: lighter-announcement-api-openapi.yml
  format: yaml
  label: Lighter announcement API
  slug: lighter-announcement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-announcement-api-openapi.yml
- filename: lighter-block-api-openapi.yml
  format: yaml
  label: Lighter block API
  slug: lighter-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-block-api-openapi.yml
- filename: lighter-bridge-api-openapi.yml
  format: yaml
  label: Lighter bridge API
  slug: lighter-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-bridge-api-openapi.yml
- filename: lighter-candlestick-api-openapi.yml
  format: yaml
  label: Lighter candlestick API
  slug: lighter-candlestick-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-candlestick-api-openapi.yml
- filename: lighter-funding-api-openapi.yml
  format: yaml
  label: Lighter funding API
  slug: lighter-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-funding-api-openapi.yml
- filename: lighter-info-api-openapi.yml
  format: yaml
  label: Lighter info API
  slug: lighter-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-info-api-openapi.yml
- filename: lighter-notification-api-openapi.yml
  format: yaml
  label: Lighter notification API
  slug: lighter-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-notification-api-openapi.yml
- filename: lighter-order-api-openapi.yml
  format: yaml
  label: Lighter order API
  slug: lighter-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-order-api-openapi.yml
- filename: lighter-referral-api-openapi.yml
  format: yaml
  label: Lighter referral API
  slug: lighter-referral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-referral-api-openapi.yml
- filename: lighter-root-api-openapi.yml
  format: yaml
  label: Lighter root API
  slug: lighter-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-root-api-openapi.yml
- filename: lighter-tokenlist-api-openapi.yml
  format: yaml
  label: Lighter tokenlist API
  slug: lighter-tokenlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-tokenlist-api-openapi.yml
- filename: lighter-transaction-api-openapi.yml
  format: yaml
  label: Lighter transaction API
  slug: lighter-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-transaction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lighter.xyz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elliot.ai
  spf: true
hosts:
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: lighter.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 18:12:40 2026 GMT
  host: apidocs.lighter.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: mainnet.zklighter.elliot.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lighter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lighter, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lighter
provider_slug: lighter
slug: lighter-domain-security
source_filename: lighter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lighter.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.lighter.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:12:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mainnet.zklighter.elliot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lighter.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: elliot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/security/lighter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trading
- Cryptocurrency
- Decentralized Finance
- Perpetual Futures
- Exchange
- Blockchain
- Zero Knowledge
- Market Data
- WebSockets
---
