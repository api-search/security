---
api_specs:
- filename: backpack-account-api-openapi.yml
  format: yaml
  label: Backpack Account API
  slug: backpack-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-account-api-openapi.yml
- filename: backpack-assets-api-openapi.yml
  format: yaml
  label: Backpack Assets API
  slug: backpack-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-assets-api-openapi.yml
- filename: backpack-borrow-lend-api-openapi.yml
  format: yaml
  label: Backpack Borrow Lend API
  slug: backpack-borrow-lend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-borrow-lend-api-openapi.yml
- filename: backpack-borrow-lend-markets-api-openapi.yml
  format: yaml
  label: Backpack Borrow Lend Markets API
  slug: backpack-borrow-lend-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-borrow-lend-markets-api-openapi.yml
- filename: backpack-capital-api-openapi.yml
  format: yaml
  label: Backpack Capital API
  slug: backpack-capital-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-capital-api-openapi.yml
- filename: backpack-markets-api-openapi.yml
  format: yaml
  label: Backpack Markets API
  slug: backpack-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-markets-api-openapi.yml
- filename: backpack-order-api-openapi.yml
  format: yaml
  label: Backpack Order API
  slug: backpack-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-order-api-openapi.yml
- filename: backpack-position-api-openapi.yml
  format: yaml
  label: Backpack Position API
  slug: backpack-position-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-position-api-openapi.yml
- filename: backpack-rfq-api-openapi.yml
  format: yaml
  label: Backpack RFQ API
  slug: backpack-rfq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-rfq-api-openapi.yml
- filename: backpack-strategy-api-openapi.yml
  format: yaml
  label: Backpack Strategy API
  slug: backpack-strategy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-strategy-api-openapi.yml
- filename: backpack-system-api-openapi.yml
  format: yaml
  label: Backpack System API
  slug: backpack-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-system-api-openapi.yml
- filename: backpack-trades-api-openapi.yml
  format: yaml
  label: Backpack Trades API
  slug: backpack-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-trades-api-openapi.yml
- filename: backpack-vaults-api-openapi.yml
  format: yaml
  label: Backpack Vaults API
  slug: backpack-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-vaults-api-openapi.yml
- filename: backpack-withdrawal-delays-api-openapi.yml
  format: yaml
  label: Backpack Withdrawal Delays API
  slug: backpack-withdrawal-delays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/openapi/backpack-withdrawal-delays-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: backpack.app
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: backpack.exchange
  spf: true
hosts:
- cert_expires: Aug 13 19:01:54 2026 GMT
  host: backpack.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: backpack.exchange
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 07:30:16 2026 GMT
  host: docs.backpack.exchange
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Backpack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Backpack, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Backpack
provider_slug: backpack
slug: backpack-domain-security
source_filename: backpack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backpack.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 19:01:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: backpack.exchange\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.backpack.exchange\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:30:16 2026 GMT\n  hsts: false\ndomains:\n- domain: backpack.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: backpack.exchange\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backpack/refs/heads/main/security/backpack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Crypto
- Exchange
- Wallet
- Trading
- Perpetuals
- Solana
- Web3
- DeFi
- xNFT
- Anchor
- Coral
- Centralized Exchange
- Self-Custody
---
