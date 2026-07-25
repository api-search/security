---
api_specs:
- filename: thirdweb-authentication-api-openapi.yml
  format: yaml
  label: thirdweb Authentication API
  slug: thirdweb-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-authentication-api-openapi.yml
- filename: thirdweb-contracts-api-openapi.yml
  format: yaml
  label: thirdweb Contracts API
  slug: thirdweb-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-contracts-api-openapi.yml
- filename: thirdweb-engine-api-openapi.yml
  format: yaml
  label: thirdweb Engine API
  slug: thirdweb-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-engine-api-openapi.yml
- filename: thirdweb-insight-api-openapi.yml
  format: yaml
  label: thirdweb Insight API
  slug: thirdweb-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-insight-api-openapi.yml
- filename: thirdweb-nebula-api-openapi.yml
  format: yaml
  label: thirdweb Nebula API
  slug: thirdweb-nebula-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-nebula-api-openapi.yml
- filename: thirdweb-payments-api-openapi.yml
  format: yaml
  label: thirdweb Payments API
  slug: thirdweb-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-payments-api-openapi.yml
- filename: thirdweb-tokens-api-openapi.yml
  format: yaml
  label: thirdweb Tokens API
  slug: thirdweb-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-tokens-api-openapi.yml
- filename: thirdweb-transactions-api-openapi.yml
  format: yaml
  label: thirdweb Transactions API
  slug: thirdweb-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-transactions-api-openapi.yml
- filename: thirdweb-wallets-api-openapi.yml
  format: yaml
  label: thirdweb Wallets API
  slug: thirdweb-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/openapi/thirdweb-wallets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thirdweb.com
  spf: true
hosts:
- cert_expires: Oct  9 02:09:50 2026 GMT
  host: thirdweb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:42:49 2026 GMT
  host: portal.thirdweb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 13:07:48 2026 GMT
  host: api.thirdweb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thirdweb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for thirdweb, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: thirdweb
provider_slug: thirdweb
slug: thirdweb-domain-security
source_filename: thirdweb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thirdweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:09:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.thirdweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:42:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.thirdweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:07:48 2026 GMT\n  hsts: null\ndomains:\n- domain: thirdweb.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thirdweb/refs/heads/main/security/thirdweb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Blockchain
- Wallets
- Smart Contracts
- Payments
- Indexer
---
