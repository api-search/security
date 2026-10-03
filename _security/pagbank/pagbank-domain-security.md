---
api_specs:
- filename: pagbank-accounts-api-openapi.yml
  format: yaml
  label: PagBank Accounts API
  slug: pagbank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-accounts-api-openapi.yml
- filename: pagbank-charges-api-openapi.yml
  format: yaml
  label: PagBank Charges API
  slug: pagbank-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-charges-api-openapi.yml
- filename: pagbank-checkout-api-openapi.yml
  format: yaml
  label: PagBank Checkout API
  slug: pagbank-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-checkout-api-openapi.yml
- filename: pagbank-connect-api-openapi.yml
  format: yaml
  label: PagBank Connect API
  slug: pagbank-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-connect-api-openapi.yml
- filename: pagbank-coupons-api-openapi.yml
  format: yaml
  label: PagBank Coupons API
  slug: pagbank-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-coupons-api-openapi.yml
- filename: pagbank-invoices-api-openapi.yml
  format: yaml
  label: PagBank Invoices API
  slug: pagbank-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-invoices-api-openapi.yml
- filename: pagbank-orders-api-openapi.yml
  format: yaml
  label: PagBank Orders API
  slug: pagbank-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-orders-api-openapi.yml
- filename: pagbank-plans-api-openapi.yml
  format: yaml
  label: PagBank Plans API
  slug: pagbank-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-plans-api-openapi.yml
- filename: pagbank-public-keys-api-openapi.yml
  format: yaml
  label: PagBank Public Keys API
  slug: pagbank-public-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-public-keys-api-openapi.yml
- filename: pagbank-refunds-api-openapi.yml
  format: yaml
  label: PagBank Refunds API
  slug: pagbank-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-refunds-api-openapi.yml
- filename: pagbank-subscribers-api-openapi.yml
  format: yaml
  label: PagBank Subscribers API
  slug: pagbank-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-subscribers-api-openapi.yml
- filename: pagbank-subscriptions-api-openapi.yml
  format: yaml
  label: PagBank Subscriptions API
  slug: pagbank-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/openapi/pagbank-subscriptions-api-openapi.yml
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
