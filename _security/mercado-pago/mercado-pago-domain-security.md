---
api_specs:
- filename: mercado-pago-asyncapi.yml
  format: yaml
  label: Mercado Pago Webhooks / Notifications
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/asyncapi/mercado-pago-asyncapi.yml
- filename: mercado-pago-authentication-api-openapi.yml
  format: yaml
  label: Mercado Pago Authentication API
  slug: mercado-pago-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-authentication-api-openapi.yml
- filename: mercado-pago-cards-api-openapi.yml
  format: yaml
  label: Mercado Pago Cards API
  slug: mercado-pago-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-cards-api-openapi.yml
- filename: mercado-pago-chargebacks-api-openapi.yml
  format: yaml
  label: Mercado Pago Chargebacks API
  slug: mercado-pago-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-chargebacks-api-openapi.yml
- filename: mercado-pago-claims-api-openapi.yml
  format: yaml
  label: Mercado Pago Claims API
  slug: mercado-pago-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-claims-api-openapi.yml
- filename: mercado-pago-customers-api-openapi.yml
  format: yaml
  label: Mercado Pago Customers API
  slug: mercado-pago-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-customers-api-openapi.yml
- filename: mercado-pago-merchant-orders-api-openapi.yml
  format: yaml
  label: Mercado Pago Merchant Orders API
  slug: mercado-pago-merchant-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-merchant-orders-api-openapi.yml
- filename: mercado-pago-orders-api-openapi.yml
  format: yaml
  label: Mercado Pago Orders API
  slug: mercado-pago-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-orders-api-openapi.yml
- filename: mercado-pago-payment-methods-api-openapi.yml
  format: yaml
  label: Mercado Pago Payment Methods API
  slug: mercado-pago-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-payment-methods-api-openapi.yml
- filename: mercado-pago-payments-api-openapi.yml
  format: yaml
  label: Mercado Pago Payments API
  slug: mercado-pago-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-payments-api-openapi.yml
- filename: mercado-pago-plans-api-openapi.yml
  format: yaml
  label: Mercado Pago Plans API
  slug: mercado-pago-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-plans-api-openapi.yml
- filename: mercado-pago-point-api-openapi.yml
  format: yaml
  label: Mercado Pago Point API
  slug: mercado-pago-point-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-point-api-openapi.yml
- filename: mercado-pago-preferences-api-openapi.yml
  format: yaml
  label: Mercado Pago Preferences API
  slug: mercado-pago-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-preferences-api-openapi.yml
- filename: mercado-pago-qr-api-openapi.yml
  format: yaml
  label: Mercado Pago QR API
  slug: mercado-pago-qr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-qr-api-openapi.yml
- filename: mercado-pago-refunds-api-openapi.yml
  format: yaml
  label: Mercado Pago Refunds API
  slug: mercado-pago-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-refunds-api-openapi.yml
- filename: mercado-pago-reports-api-openapi.yml
  format: yaml
  label: Mercado Pago Reports API
  slug: mercado-pago-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-reports-api-openapi.yml
- filename: mercado-pago-subscriptions-api-openapi.yml
  format: yaml
  label: Mercado Pago Subscriptions API
  slug: mercado-pago-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "visa.com"
  - 0 iodef "mailto:domains@mercadolibre.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mercadopago.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:domains@mercadolibre.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mercadopago.com.br
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.mercadopago.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: www.mercadopago.com.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: api.mercadopago.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercado Pago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercado Pago, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mercado Pago
provider_slug: mercado-pago
slug: mercado-pago-domain-security
source_filename: mercado-pago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mercadopago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.mercadopago.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mercadopago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mercadopago.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"visa.com\"\n  - 0 iodef \"mailto:domains@mercadolibre.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mercadopago.com.br\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:domains@mercadolibre.com\"\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/security/mercado-pago-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Checkout
- Subscriptions
- POS
- QR
- PIX
- SDKs
- Wallet
- Acquiring
- Lending
- Issuing
- Latin America
- Brazil
- Argentina
- Mexico
- Chile
- Colombia
- Peru
- Uruguay
- Fintech
---
