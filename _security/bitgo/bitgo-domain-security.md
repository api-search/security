---
api_specs:
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Wallets API
  slug: bitgo-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Addresses API
  slug: bitgo-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Transactions & Transfers API
  slug: bitgo-transactions-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Keychains & Keys API
  slug: bitgo-keychains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Webhooks API
  slug: bitgo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Wallet Policies API
  slug: bitgo-wallet-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Staking API
  slug: bitgo-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Trading & Settlement (Go Network) API
  slug: bitgo-trading-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Express API
  slug: bitgo-express-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
- filename: bitgo-openapi.yml
  format: yaml
  label: BitGo Enterprise & Users API
  slug: bitgo-enterprise-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/openapi/bitgo-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bitgo.com
  spf: true
hosts:
- cert_expires: Sep 19 17:00:23 2026 GMT
  host: www.bitgo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 22:46:35 2026 GMT
  host: developers.bitgo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 17:00:23 2026 GMT
  host: app.bitgo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitGo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BitGo
provider_slug: bitgo
slug: bitgo-domain-security
source_filename: bitgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bitgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:00:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.bitgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:46:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.bitgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:00:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bitgo.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitgo/refs/heads/main/security/bitgo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Digital Assets
- Custody
- Wallets
- Blockchain
- Crypto
- Staking
- Settlement
---
