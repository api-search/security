---
api_specs:
- filename: charles-schwab-accounts-api-openapi.yml
  format: yaml
  label: Charles Schwab Accounts API
  slug: charles-schwab-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-accounts-api-openapi.yml
- filename: charles-schwab-instruments-api-openapi.yml
  format: yaml
  label: Charles Schwab Instruments API
  slug: charles-schwab-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-instruments-api-openapi.yml
- filename: charles-schwab-market-hours-api-openapi.yml
  format: yaml
  label: Charles Schwab Market Hours API
  slug: charles-schwab-market-hours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-market-hours-api-openapi.yml
- filename: charles-schwab-movers-api-openapi.yml
  format: yaml
  label: Charles Schwab Movers API
  slug: charles-schwab-movers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-movers-api-openapi.yml
- filename: charles-schwab-options-api-openapi.yml
  format: yaml
  label: Charles Schwab Options API
  slug: charles-schwab-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-options-api-openapi.yml
- filename: charles-schwab-orders-api-openapi.yml
  format: yaml
  label: Charles Schwab Orders API
  slug: charles-schwab-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-orders-api-openapi.yml
- filename: charles-schwab-price-history-api-openapi.yml
  format: yaml
  label: Charles Schwab Price History API
  slug: charles-schwab-price-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-price-history-api-openapi.yml
- filename: charles-schwab-quotes-api-openapi.yml
  format: yaml
  label: Charles Schwab Quotes API
  slug: charles-schwab-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-quotes-api-openapi.yml
- filename: charles-schwab-transactions-api-openapi.yml
  format: yaml
  label: Charles Schwab Transactions API
  slug: charles-schwab-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-transactions-api-openapi.yml
- filename: charles-schwab-user-preferences-api-openapi.yml
  format: yaml
  label: Charles Schwab User Preferences API
  slug: charles-schwab-user-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-user-preferences-api-openapi.yml
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
- Account
- Banking
- Brokerage
- Financial-Services
- Investing
- Market Data
- Authentication
- Order
- Trading
- Fortune 500
---
