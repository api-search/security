---
api_specs:
- filename: coinsph-account-openapi.json
  format: json
  label: Coins.ph Coins Pro — Account
  slug: coinsph-coins-pro-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-account-openapi.json
- filename: coinsph-account-validation-openapi.json
  format: json
  label: Coins.ph Account Validation
  slug: coinsph-account-validation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-account-validation-openapi.json
- filename: coinsph-convert-openapi.json
  format: json
  label: Coins.ph Coins Pro — Convert
  slug: coinsph-coins-pro-convert
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-convert-openapi.json
- filename: coinsph-listenkey-openapi.json
  format: json
  label: Coins.ph Coins Pro — User Data Stream
  slug: coinsph-coins-pro-user-data-stream
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-listenkey-openapi.json
- filename: coinsph-markets-openapi.json
  format: json
  label: Coins.ph Coins Pro — Market Data
  slug: coinsph-coins-pro-market-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-markets-openapi.json
- filename: coinsph-payment-openapi.json
  format: json
  label: Coins.ph Payment / Partner Integration
  slug: coinsph-payment-partner-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-payment-openapi.json
- filename: coinsph-ramp-openapi.json
  format: json
  label: Coins.ph ON/OFF Ramp
  slug: coinsph-onoff-ramp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-ramp-openapi.json
- filename: coinsph-spot-openapi.json
  format: json
  label: Coins.ph Coins Pro — Spot Trading
  slug: coinsph-coins-pro-spot-trading
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-spot-openapi.json
- filename: coinsph-sub-account-openapi.json
  format: json
  label: Coins.ph Coins Pro — Sub-Account
  slug: coinsph-coins-pro-sub-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-sub-account-openapi.json
- filename: coinsph-system-openapi.json
  format: json
  label: Coins.ph Coins Pro — System
  slug: coinsph-coins-pro-system
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-system-openapi.json
- filename: coinsph-wallet-openapi.json
  format: json
  label: Coins.ph Coins Pro — Wallet
  slug: coinsph-coins-pro-wallet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/openapi/coinsph-wallet-openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: coins.ph
  spf: true
hosts:
- cert_expires: Sep  3 04:31:49 2026 GMT
  host: coins.ph
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinsph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coins.ph, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Coins.ph
provider_slug: coinsph
slug: coinsph-domain-security
source_filename: coinsph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coins.ph\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 04:31:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: coins.ph\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinsph/refs/heads/main/security/coinsph-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Cryptocurrency Exchange
- Payments
- Fintech
- Wallet
- Philippines
- Trading
---
