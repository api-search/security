---
api_specs:
- filename: cryptoquant-exchange-flows-api-openapi.yml
  format: yaml
  label: CryptoQuant Exchange Flows API
  slug: cryptoquant-exchange-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptoquant/refs/heads/main/openapi/cryptoquant-exchange-flows-api-openapi.yml
- filename: cryptoquant-market-data-api-openapi.yml
  format: yaml
  label: CryptoQuant Market Data API
  slug: cryptoquant-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptoquant/refs/heads/main/openapi/cryptoquant-market-data-api-openapi.yml
- filename: cryptoquant-miner-api-openapi.yml
  format: yaml
  label: CryptoQuant Miner API
  slug: cryptoquant-miner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptoquant/refs/heads/main/openapi/cryptoquant-miner-api-openapi.yml
- filename: cryptoquant-on-chain-api-openapi.yml
  format: yaml
  label: CryptoQuant On-Chain API
  slug: cryptoquant-on-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptoquant/refs/heads/main/openapi/cryptoquant-on-chain-api-openapi.yml
- filename: cryptoquant-stablecoins-api-openapi.yml
  format: yaml
  label: CryptoQuant Stablecoins API
  slug: cryptoquant-stablecoins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptoquant/refs/heads/main/openapi/cryptoquant-stablecoins-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cryptoquant.com
  spf: true
hosts:
- cert_expires: Aug 21 07:58:39 2026 GMT
  host: cryptoquant.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 07:58:39 2026 GMT
  host: api.cryptoquant.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cryptoquant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CryptoQuant, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CryptoQuant
provider_slug: cryptoquant
slug: cryptoquant-domain-security
source_filename: cryptoquant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cryptoquant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 07:58:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cryptoquant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 07:58:39 2026 GMT\n  hsts: null\ndomains:\n- domain: cryptoquant.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptoquant/refs/heads/main/security/cryptoquant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Cryptocurrency
- On-Chain Analytics
- Market Data
- Derivatives
---
