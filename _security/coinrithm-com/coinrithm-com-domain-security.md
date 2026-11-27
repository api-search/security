---
api_specs:
- filename: coinrithm-com-futures-api-openapi.yml
  format: yaml
  label: CoinRithm Futures API
  slug: coinrithm-com-futures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-futures-api-openapi.yml
- filename: coinrithm-com-identity-api-openapi.yml
  format: yaml
  label: CoinRithm Identity API
  slug: coinrithm-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-identity-api-openapi.yml
- filename: coinrithm-com-ledger-api-openapi.yml
  format: yaml
  label: CoinRithm Ledger API
  slug: coinrithm-com-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-ledger-api-openapi.yml
- filename: coinrithm-com-prediction-markets-api-openapi.yml
  format: yaml
  label: CoinRithm Prediction Markets API
  slug: coinrithm-com-prediction-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-prediction-markets-api-openapi.yml
- filename: coinrithm-com-public-crypto-data-api-openapi.yml
  format: yaml
  label: CoinRithm Public Crypto Data API
  slug: coinrithm-com-public-crypto-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-public-crypto-data-api-openapi.yml
- filename: coinrithm-com-public-market-data-api-openapi.yml
  format: yaml
  label: CoinRithm Public Market Data API
  slug: coinrithm-com-public-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-public-market-data-api-openapi.yml
- filename: coinrithm-com-public-pm-data-api-openapi.yml
  format: yaml
  label: CoinRithm Public Pm Data API
  slug: coinrithm-com-public-pm-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-public-pm-data-api-openapi.yml
- filename: coinrithm-com-reads-api-openapi.yml
  format: yaml
  label: CoinRithm Reads API
  slug: coinrithm-com-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-reads-api-openapi.yml
- filename: coinrithm-com-spot-api-openapi.yml
  format: yaml
  label: CoinRithm Spot API
  slug: coinrithm-com-spot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-spot-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coinrithm.com
  spf: true
hosts:
- cert_expires: Jan 27 00:28:25 2027 GMT
  host: coinrithm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CoinRithm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinRithm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CoinRithm
provider_slug: coinrithm-com
slug: coinrithm-com-domain-security
source_filename: coinrithm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinrithm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 00:28:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coinrithm.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/coinrithm-com/security/coinrithm-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Prediction Markets
- Crypto Prices
- Paper Trading
- Agentic Trading
- Research Service
- Live Market Data
---
