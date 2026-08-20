---
api_specs:
- filename: robinhood-account-api-openapi.yml
  format: yaml
  label: Robinhood Account API
  slug: robinhood-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robinhood/refs/heads/main/openapi/robinhood-account-api-openapi.yml
- filename: robinhood-holdings-api-openapi.yml
  format: yaml
  label: Robinhood Holdings API
  slug: robinhood-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robinhood/refs/heads/main/openapi/robinhood-holdings-api-openapi.yml
- filename: robinhood-market-data-api-openapi.yml
  format: yaml
  label: Robinhood Market Data API
  slug: robinhood-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robinhood/refs/heads/main/openapi/robinhood-market-data-api-openapi.yml
- filename: robinhood-orders-api-openapi.yml
  format: yaml
  label: Robinhood Orders API
  slug: robinhood-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robinhood/refs/heads/main/openapi/robinhood-orders-api-openapi.yml
- filename: robinhood-trading-pairs-api-openapi.yml
  format: yaml
  label: Robinhood Trading Pairs API
  slug: robinhood-trading-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robinhood/refs/heads/main/openapi/robinhood-trading-pairs-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "cloudflare.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: robinhood.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: robinhood.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: docs.robinhood.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: trading.robinhood.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Robinhood Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Robinhood, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Robinhood
provider_slug: robinhood
slug: robinhood-domain-security
source_filename: robinhood-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: robinhood.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.robinhood.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: trading.robinhood.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: robinhood.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"cloudflare.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robinhood/refs/heads/main/security/robinhood-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Cryptocurrency
- Trading
- Brokerage
- Investing
- Financial-Services
- Crypto
---
