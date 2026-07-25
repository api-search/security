---
api_specs:
- filename: nordpool-intraday-asyncapi.yml
  format: yaml
  label: Nord Pool Intraday Trading API
  slug: nordpool-intraday-trading-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/asyncapi/nordpool-intraday-asyncapi.yml
- filename: nordpool-auction-api-openapi.yml
  format: yaml
  label: Nord Pool Auction API
  slug: nordpool-auction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-auction-api-openapi.yml
- filename: nordpool-balancemarket-api-openapi.yml
  format: yaml
  label: Nord Pool BalanceMarket API
  slug: nordpool-balancemarket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-balancemarket-api-openapi.yml
- filename: nordpool-day-ahead-prices-api-openapi.yml
  format: yaml
  label: Nord Pool Day-Ahead Prices API
  slug: nordpool-day-ahead-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-day-ahead-prices-api-openapi.yml
- filename: nordpool-exchangerate-api-openapi.yml
  format: yaml
  label: Nord Pool ExchangeRate API
  slug: nordpool-exchangerate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-exchangerate-api-openapi.yml
- filename: nordpool-intraday-api-openapi.yml
  format: yaml
  label: Nord Pool Intraday API
  slug: nordpool-intraday-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-intraday-api-openapi.yml
- filename: nordpool-powersystem-api-openapi.yml
  format: yaml
  label: Nord Pool PowerSystem API
  slug: nordpool-powersystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-powersystem-api-openapi.yml
- filename: nordpool-pricecurves-api-openapi.yml
  format: yaml
  label: Nord Pool PriceCurves API
  slug: nordpool-pricecurves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-pricecurves-api-openapi.yml
- filename: nordpool-system-api-openapi.yml
  format: yaml
  label: Nord Pool System API
  slug: nordpool-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-system-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nordpoolgroup.com
  spf: true
hosts:
- cert_expires: Sep 11 04:29:16 2026 GMT
  host: www.nordpoolgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 08:03:40 2026 GMT
  host: developers.nordpoolgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 04:29:16 2026 GMT
  host: data-api.nordpoolgroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nordpool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nord Pool, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nord Pool
provider_slug: nordpool
slug: nordpool-domain-security
source_filename: nordpool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nordpoolgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:29:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.nordpoolgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:03:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data-api.nordpoolgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:29:16 2026 GMT\n  hsts: null\ndomains:\n- domain: nordpoolgroup.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/security/nordpool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Day-Ahead Prices
- Electricity
- Energy Markets
- Power Exchange
- Intraday Trading
- Market Data
- Europe
---
