---
api_specs:
- filename: kushki-card-payments-api-openapi.yml
  format: yaml
  label: Kushki Card Payments API
  slug: kushki-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-card-payments-api-openapi.yml
- filename: kushki-subscriptions-api-openapi.yml
  format: yaml
  label: Kushki Subscriptions API
  slug: kushki-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-subscriptions-api-openapi.yml
- filename: kushki-transfer-payments-api-openapi.yml
  format: yaml
  label: Kushki Transfer Payments API
  slug: kushki-transfer-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-transfer-payments-api-openapi.yml
- filename: kushki-cash-payments-api-openapi.yml
  format: yaml
  label: Kushki Cash Payments API
  slug: kushki-cash-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-cash-payments-api-openapi.yml
- filename: kushki-payouts-api-openapi.yml
  format: yaml
  label: Kushki Payouts API
  slug: kushki-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-payouts-api-openapi.yml
- filename: kushki-card-present-api-openapi.yml
  format: yaml
  label: Kushki Card Present API
  slug: kushki-card-present-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-card-present-api-openapi.yml
- filename: kushki-merchants-api-openapi.yml
  format: yaml
  label: Kushki Merchants and Branches API
  slug: kushki-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/openapi/kushki-merchants-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kushkipagos.com
  spf: true
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kushki.com
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: kushkipagos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: docs.kushki.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 20:21:09 2026 GMT
  host: api.kushkipagos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kushki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kushki, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kushki
provider_slug: kushki
slug: kushki-domain-security
source_filename: kushki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kushkipagos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.kushki.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kushkipagos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 20:21:09 2026 GMT\n  hsts: null\ndomains:\n- domain: kushkipagos.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kushki.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kushki/refs/heads/main/security/kushki-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- LatAm
- Andean Region
- Card Payments
- Subscriptions
- Cash
- Bank Transfers
- Payouts
- PSE
- Webpay
- SPEI
- PIX
- OXXO
- PagoEfectivo
- Fintech
- Ecuador
- Colombia
- Peru
- Chile
- Mexico
- Brazil
---
