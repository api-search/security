---
api_specs:
- filename: bigone-account-api-openapi.yml
  format: yaml
  label: BigONE Account API
  slug: bigone-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-account-api-openapi.yml
- filename: bigone-asset-api-openapi.yml
  format: yaml
  label: BigONE Asset API
  slug: bigone-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-asset-api-openapi.yml
- filename: bigone-assets-api-openapi.yml
  format: yaml
  label: BigONE Assets API
  slug: bigone-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-assets-api-openapi.yml
- filename: bigone-deposit-api-openapi.yml
  format: yaml
  label: BigONE Deposit API
  slug: bigone-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-deposit-api-openapi.yml
- filename: bigone-funding-account-api-openapi.yml
  format: yaml
  label: BigONE Funding Account API
  slug: bigone-funding-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-funding-account-api-openapi.yml
- filename: bigone-market-data-api-openapi.yml
  format: yaml
  label: BigONE Market Data API
  slug: bigone-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-market-data-api-openapi.yml
- filename: bigone-order-api-openapi.yml
  format: yaml
  label: BigONE Order API
  slug: bigone-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-order-api-openapi.yml
- filename: bigone-ping-api-openapi.yml
  format: yaml
  label: BigONE Ping API
  slug: bigone-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-ping-api-openapi.yml
- filename: bigone-position-api-openapi.yml
  format: yaml
  label: BigONE Position API
  slug: bigone-position-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-position-api-openapi.yml
- filename: bigone-quote-api-openapi.yml
  format: yaml
  label: BigONE Quote API
  slug: bigone-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-quote-api-openapi.yml
- filename: bigone-ranges-api-openapi.yml
  format: yaml
  label: BigONE Ranges API
  slug: bigone-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-ranges-api-openapi.yml
- filename: bigone-trade-api-openapi.yml
  format: yaml
  label: BigONE Trade API
  slug: bigone-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-trade-api-openapi.yml
- filename: bigone-trades-api-openapi.yml
  format: yaml
  label: BigONE Trades API
  slug: bigone-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-trades-api-openapi.yml
- filename: bigone-transfer-api-openapi.yml
  format: yaml
  label: BigONE Transfer API
  slug: bigone-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-transfer-api-openapi.yml
- filename: bigone-withdrawal-api-openapi.yml
  format: yaml
  label: BigONE Withdrawal API
  slug: bigone-withdrawal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/openapi/bigone-withdrawal-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: big.one
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: big.one
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bigone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BigONE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BigONE
provider_slug: bigone
slug: bigone-domain-security
source_filename: bigone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: big.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: big.one\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigone/refs/heads/main/security/bigone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Derivatives
- Wallets
- Market Data
---
