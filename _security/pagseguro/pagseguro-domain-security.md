---
api_specs:
- filename: pagseguro-accounts-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Accounts API
  slug: pagseguro-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-accounts-api-openapi.yml
- filename: pagseguro-charges-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Charges API
  slug: pagseguro-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-charges-api-openapi.yml
- filename: pagseguro-checkout-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Checkout API
  slug: pagseguro-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-checkout-api-openapi.yml
- filename: pagseguro-connect-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Connect API
  slug: pagseguro-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-connect-api-openapi.yml
- filename: pagseguro-coupons-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Coupons API
  slug: pagseguro-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-coupons-api-openapi.yml
- filename: pagseguro-invoices-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Invoices API
  slug: pagseguro-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-invoices-api-openapi.yml
- filename: pagseguro-orders-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Orders API
  slug: pagseguro-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-orders-api-openapi.yml
- filename: pagseguro-plans-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Plans API
  slug: pagseguro-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-plans-api-openapi.yml
- filename: pagseguro-publickeys-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank PublicKeys API
  slug: pagseguro-publickeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-publickeys-api-openapi.yml
- filename: pagseguro-refunds-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Refunds API
  slug: pagseguro-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-refunds-api-openapi.yml
- filename: pagseguro-subscribers-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Subscribers API
  slug: pagseguro-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-subscribers-api-openapi.yml
- filename: pagseguro-subscriptions-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Subscriptions API
  slug: pagseguro-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/openapi/pagseguro-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pagbank.com.br
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pagseguro.com
  spf: true
hosts:
- cert_expires: Oct  3 22:43:13 2026 GMT
  host: pagbank.com.br
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 03:08:37 2026 GMT
  host: developer.pagbank.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: api.pagseguro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pagseguro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PagSeguro / PagBank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PagSeguro / PagBank
provider_slug: pagseguro
slug: pagseguro-domain-security
source_filename: pagseguro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagbank.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:43:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.pagbank.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:08:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pagseguro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pagbank.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pagseguro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagseguro/refs/heads/main/security/pagseguro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Checkout
- Pix
- Boleto
- Cards
- Subscriptions
- Recurring
- POS
- Card Reader
- Marketplace
- Split
- Payouts
- Digital Bank
- Brazil
- Latin America
- Fintech
---
