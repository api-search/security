---
api_specs:
- filename: nomba-accounts-api-openapi.yml
  format: yaml
  label: Nomba Accounts API
  slug: nomba-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-accounts-api-openapi.yml
- filename: nomba-authentication-api-openapi.yml
  format: yaml
  label: Nomba Authentication API
  slug: nomba-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-authentication-api-openapi.yml
- filename: nomba-card-charge-api-openapi.yml
  format: yaml
  label: Nomba Card Charge API
  slug: nomba-card-charge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-card-charge-api-openapi.yml
- filename: nomba-checkout-orders-api-openapi.yml
  format: yaml
  label: Nomba Checkout Orders API
  slug: nomba-checkout-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-checkout-orders-api-openapi.yml
- filename: nomba-corridors-api-openapi.yml
  format: yaml
  label: Nomba Corridors API
  slug: nomba-corridors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-corridors-api-openapi.yml
- filename: nomba-exchange-rates-api-openapi.yml
  format: yaml
  label: Nomba Exchange Rates API
  slug: nomba-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-exchange-rates-api-openapi.yml
- filename: nomba-order-management-api-openapi.yml
  format: yaml
  label: Nomba Order Management API
  slug: nomba-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-order-management-api-openapi.yml
- filename: nomba-payouts-api-openapi.yml
  format: yaml
  label: Nomba Payouts API
  slug: nomba-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-payouts-api-openapi.yml
- filename: nomba-saved-cards-api-openapi.yml
  format: yaml
  label: Nomba Saved Cards API
  slug: nomba-saved-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-saved-cards-api-openapi.yml
- filename: nomba-tokenized-cards-api-openapi.yml
  format: yaml
  label: Nomba Tokenized Cards API
  slug: nomba-tokenized-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-tokenized-cards-api-openapi.yml
- filename: nomba-transactions-api-openapi.yml
  format: yaml
  label: Nomba Transactions API
  slug: nomba-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-transactions-api-openapi.yml
- filename: nomba-transfers-api-openapi.yml
  format: yaml
  label: Nomba Transfers API
  slug: nomba-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-transfers-api-openapi.yml
- filename: nomba-virtual-accounts-api-openapi.yml
  format: yaml
  label: Nomba Virtual Accounts API
  slug: nomba-virtual-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-virtual-accounts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nomba.com
  spf: true
hosts:
- cert_expires: Aug 18 18:47:32 2026 GMT
  host: nomba.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 10:39:02 2026 GMT
  host: developer.nomba.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 10:39:02 2026 GMT
  host: api.nomba.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nomba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomba, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nomba
provider_slug: nomba
slug: nomba-domain-security
source_filename: nomba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nomba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 18:47:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: developer.nomba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:39:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nomba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:39:02 2026 GMT\n  hsts: null\ndomains:\n- domain: nomba.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/security/nomba-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- Banking
- Transfers
- Virtual Accounts
- Checkout
- Cross-Border Payments
- Cards
---
