---
api_specs:
- filename: charles-schwab-trader-api-openapi.yml
  format: yaml
  label: Charles Schwab Trader API
  slug: trader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-trader-api-openapi.yml
- filename: charles-schwab-market-data-api-openapi.yml
  format: yaml
  label: Charles Schwab Market Data API
  slug: market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-market-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: schwab.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: schwabapi.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: www.schwab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: developer.schwab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.schwabapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charles Schwab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charles Schwab, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Charles Schwab
provider_slug: charles-schwab
slug: charles-schwab-domain-security
source_filename: charles-schwab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.schwab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.schwab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.schwabapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: schwab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: schwabapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/security/charles-schwab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounts
- Banking
- Brokerage
- Financial Services
- Investing
- Market Data
- OAuth 2.0
- Orders
- Trading
- Fortune 500
---
