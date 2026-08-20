---
api_specs:
- filename: koin-access-api-openapi.yml
  format: yaml
  label: Koin Access API
  slug: koin-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-access-api-openapi.yml
- filename: koin-account-take-over-services-api-openapi.yml
  format: yaml
  label: Koin Account Take Over Services API
  slug: koin-account-take-over-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-account-take-over-services-api-openapi.yml
- filename: koin-availability-services-api-openapi.yml
  format: yaml
  label: Koin Availability Services API
  slug: koin-availability-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-availability-services-api-openapi.yml
- filename: koin-communication-services-api-openapi.yml
  format: yaml
  label: Koin Communication Services API
  slug: koin-communication-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-communication-services-api-openapi.yml
- filename: koin-ecommerce-api-openapi.yml
  format: yaml
  label: Koin Ecommerce API
  slug: koin-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-ecommerce-api-openapi.yml
- filename: koin-notification-services-sales-api-openapi.yml
  format: yaml
  label: Koin Notification Services Sales API
  slug: koin-notification-services-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-notification-services-sales-api-openapi.yml
- filename: koin-onboarding-services-api-openapi.yml
  format: yaml
  label: Koin Onboarding Services API
  slug: koin-onboarding-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-onboarding-services-api-openapi.yml
- filename: koin-payment-service-provider-api-openapi.yml
  format: yaml
  label: Koin Payment Service Provider API
  slug: koin-payment-service-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-payment-service-provider-api-openapi.yml
- filename: koin-payment-services-api-openapi.yml
  format: yaml
  label: Koin Payment Services API
  slug: koin-payment-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-payment-services-api-openapi.yml
- filename: koin-paymentrequest-api-openapi.yml
  format: yaml
  label: Koin PaymentRequest API
  slug: koin-paymentrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-paymentrequest-api-openapi.yml
- filename: koin-payout-services-api-openapi.yml
  format: yaml
  label: Koin Payout Services API
  slug: koin-payout-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-payout-services-api-openapi.yml
- filename: koin-recipient-services-account-api-openapi.yml
  format: yaml
  label: Koin Recipient Services Account API
  slug: koin-recipient-services-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-recipient-services-account-api-openapi.yml
- filename: koin-refund-services-api-openapi.yml
  format: yaml
  label: Koin Refund Services API
  slug: koin-refund-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-refund-services-api-openapi.yml
- filename: koin-support-services-api-openapi.yml
  format: yaml
  label: Koin Support Services API
  slug: koin-support-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-support-services-api-openapi.yml
- filename: koin-tokenize-services-api-openapi.yml
  format: yaml
  label: Koin Tokenize Services API
  slug: koin-tokenize-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-tokenize-services-api-openapi.yml
- filename: koin-wiretransfer-api-openapi.yml
  format: yaml
  label: Koin WireTransfer API
  slug: koin-wiretransfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/openapi/koin-wiretransfer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: koin.com.br
  spf: true
hosts:
- cert_expires: Aug 30 03:15:24 2026 GMT
  host: www.koin.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 07:19:04 2026 GMT
  host: api-docs.koin.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api-sandbox.koin.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Koin
provider_slug: koin
slug: koin-domain-security
source_filename: koin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.koin.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:15:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.koin.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:19:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-sandbox.koin.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: koin.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koin/refs/heads/main/security/koin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fraud Prevention
- Buy Now Pay Later
- Pix
- E-Commerce
- Financial-Services
- Brazil
- Latin America
- Anti-Fraud
- Checkout
- Company
---
