---
api_specs:
- filename: pagseguro-orders-api-openapi.yml
  format: yaml
  label: PagBank Orders API
  slug: pagbank-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-orders-api-openapi.yml
- filename: pagseguro-connect-api-openapi.yml
  format: yaml
  label: PagBank Connect API
  slug: pagbank-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-connect-api-openapi.yml
- filename: pagseguro-checkout-api-openapi.yml
  format: yaml
  label: PagBank Checkout API
  slug: pagbank-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-checkout-api-openapi.yml
- filename: pagseguro-accounts-api-openapi.yml
  format: yaml
  label: PagBank Account Registration API
  slug: pagbank-account-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-accounts-api-openapi.yml
- filename: pagseguro-charges-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Charges API
  slug: pagseguro-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-charges-api-openapi.yml
- filename: pagseguro-coupons-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Coupons API
  slug: pagseguro-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-coupons-api-openapi.yml
- filename: pagseguro-invoices-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Invoices API
  slug: pagseguro-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-invoices-api-openapi.yml
- filename: pagseguro-plans-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Plans API
  slug: pagseguro-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-plans-api-openapi.yml
- filename: pagseguro-refunds-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Refunds API
  slug: pagseguro-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-refunds-api-openapi.yml
- filename: pagseguro-subscribers-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Subscribers API
  slug: pagseguro-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-subscribers-api-openapi.yml
- filename: pagseguro-subscriptions-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Subscriptions API
  slug: pagseguro-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-subscriptions-api-openapi.yml
- filename: pagseguro-public-keys-api-openapi.yml
  format: yaml
  label: PagSeguro / PagBank Public Keys API
  slug: pagseguro-public-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagseguro-public-keys-api-openapi.yml
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
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Pagbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PagBank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PagBank
provider_slug: pagbank
slug: pagbank-domain-security
source_filename: pagbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagbank.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:43:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.pagbank.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:08:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pagseguro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pagbank.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pagseguro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/security/pagbank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Digital Banking
- Brazil
- Pix
- Fintech
- E-Commerce
- Point-of-Sale
- Recurring Payments
- Boleto
---
