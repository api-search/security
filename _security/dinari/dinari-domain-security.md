---
api_specs:
- filename: dinari-accounts-api-openapi.yml
  format: yaml
  label: Dinari Accounts API
  slug: dinari-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-accounts-api-openapi.yml
- filename: dinari-corporate-actions-api-openapi.yml
  format: yaml
  label: Dinari Corporate Actions API
  slug: dinari-corporate-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-corporate-actions-api-openapi.yml
- filename: dinari-entities-api-openapi.yml
  format: yaml
  label: Dinari Entities API
  slug: dinari-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-entities-api-openapi.yml
- filename: dinari-kyc-api-openapi.yml
  format: yaml
  label: Dinari KYC API
  slug: dinari-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-kyc-api-openapi.yml
- filename: dinari-managed-orders-api-openapi.yml
  format: yaml
  label: Dinari Managed Orders API
  slug: dinari-managed-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-managed-orders-api-openapi.yml
- filename: dinari-market-data-api-openapi.yml
  format: yaml
  label: Dinari Market Data API
  slug: dinari-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-market-data-api-openapi.yml
- filename: dinari-order-requests-api-openapi.yml
  format: yaml
  label: Dinari Order Requests API
  slug: dinari-order-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-order-requests-api-openapi.yml
- filename: dinari-orders-api-openapi.yml
  format: yaml
  label: Dinari Orders API
  slug: dinari-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-orders-api-openapi.yml
- filename: dinari-wallets-api-openapi.yml
  format: yaml
  label: Dinari Wallets API
  slug: dinari-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-wallets-api-openapi.yml
- filename: dinari-withdrawals-api-openapi.yml
  format: yaml
  label: Dinari Withdrawals API
  slug: dinari-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/openapi/dinari-withdrawals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dinari.com
  spf: true
hosts:
- cert_expires: Oct 14 21:51:25 2026 GMT
  host: dinari.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 01:39:23 2026 GMT
  host: api-enterprise.sbt.dinari.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dinari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dinari, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dinari
provider_slug: dinari
slug: dinari-domain-security
source_filename: dinari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dinari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:51:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-enterprise.sbt.dinari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:39:23 2026 GMT\n  hsts: null\ndomains:\n- domain: dinari.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dinari/refs/heads/main/security/dinari-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tokenized Securities
- Stocks
- ETFs
- Brokerage
- Market Data
- Blockchain
- Stablecoin
- Fintech
- KYC
- Order
- Wallets
---
