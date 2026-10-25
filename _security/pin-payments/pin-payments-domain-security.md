---
api_specs:
- filename: pin-payments-cards-api-openapi.yml
  format: yaml
  label: Pin Payments Cards API
  slug: pin-payments-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/openapi/pin-payments-cards-api-openapi.yml
- filename: pin-payments-charges-api-openapi.yml
  format: yaml
  label: Pin Payments Charges API
  slug: pin-payments-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/openapi/pin-payments-charges-api-openapi.yml
- filename: pin-payments-customers-api-openapi.yml
  format: yaml
  label: Pin Payments Customers API
  slug: pin-payments-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/openapi/pin-payments-customers-api-openapi.yml
- filename: pin-payments-refunds-api-openapi.yml
  format: yaml
  label: Pin Payments Refunds API
  slug: pin-payments-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/openapi/pin-payments-refunds-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pinpayments.com
  spf: true
hosts:
- cert_expires: Dec 12 15:17:49 2026 GMT
  host: pinpayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: api.pinpayments.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: test-api.pinpayments.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Pin Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pin Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pin Payments
provider_slug: pin-payments
slug: pin-payments-domain-security
source_filename: pin-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pinpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:17:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pinpayments.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: null\n- host: test-api.pinpayments.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pinpayments.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pin-payments/refs/heads/main/security/pin-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Cards
- Subscription
- Refunds
- Payment Gateway
- Recurring Payments
- Ecommerce
- Australia
---
