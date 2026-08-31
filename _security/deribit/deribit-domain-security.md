---
api_specs:
- filename: asyncapi.yaml
  format: yaml
  label: Deribit WebSocket API
  slug: deribit-websocket-api
  spec_type: AsyncAPI
  url: https://docs.deribit.com/
- filename: deribit-account-management-api-openapi.yml
  format: yaml
  label: Deribit Account Management API
  slug: deribit-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-account-management-api-openapi.yml
- filename: deribit-authentication-api-openapi.yml
  format: yaml
  label: Deribit Authentication API
  slug: deribit-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-authentication-api-openapi.yml
- filename: deribit-block-rfq-api-openapi.yml
  format: yaml
  label: Deribit Block RFQ API
  slug: deribit-block-rfq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-block-rfq-api-openapi.yml
- filename: deribit-block-trade-api-openapi.yml
  format: yaml
  label: Deribit Block Trade API
  slug: deribit-block-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-block-trade-api-openapi.yml
- filename: deribit-combo-books-api-openapi.yml
  format: yaml
  label: Deribit Combo Books API
  slug: deribit-combo-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-combo-books-api-openapi.yml
- filename: deribit-market-data-api-openapi.yml
  format: yaml
  label: Deribit Market Data API
  slug: deribit-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-market-data-api-openapi.yml
- filename: deribit-portfolio-management-api-openapi.yml
  format: yaml
  label: Deribit Portfolio Management API
  slug: deribit-portfolio-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-portfolio-management-api-openapi.yml
- filename: deribit-session-management-api-openapi.yml
  format: yaml
  label: Deribit Session Management API
  slug: deribit-session-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-session-management-api-openapi.yml
- filename: deribit-subscription-management-api-openapi.yml
  format: yaml
  label: Deribit Subscription Management API
  slug: deribit-subscription-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-subscription-management-api-openapi.yml
- filename: deribit-supporting-api-openapi.yml
  format: yaml
  label: Deribit Supporting API
  slug: deribit-supporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-supporting-api-openapi.yml
- filename: deribit-trading-api-openapi.yml
  format: yaml
  label: Deribit Trading API
  slug: deribit-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-trading-api-openapi.yml
- filename: deribit-wallet-api-openapi.yml
  format: yaml
  label: Deribit Wallet API
  slug: deribit-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/openapi/deribit-wallet-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deribit.com
  spf: true
hosts:
- cert_expires: Sep 20 06:21:41 2026 GMT
  host: insights.deribit.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 19:39:18 2026 GMT
  host: docs.deribit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 06:21:41 2026 GMT
  host: www.deribit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deribit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deribit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deribit
provider_slug: deribit
slug: deribit-domain-security
source_filename: deribit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insights.deribit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:21:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: docs.deribit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 19:39:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.deribit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:21:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deribit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deribit/refs/heads/main/security/deribit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Derivatives
- Cryptocurrency
- Bitcoin
- Ethereum
- Options
- Futures
- Perpetuals
- Trading
- Market Data
- Block Trading
- WebSocket
- Financial
---
