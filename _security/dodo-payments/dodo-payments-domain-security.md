---
api_specs:
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Products API
  slug: dodo-payments-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Payments API
  slug: dodo-payments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Subscriptions API
  slug: dodo-payments-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Customers API
  slug: dodo-payments-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Checkout Sessions API
  slug: dodo-payments-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Discounts API
  slug: dodo-payments-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Licenses API
  slug: dodo-payments-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Payouts API
  slug: dodo-payments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
- filename: dodo-payments-openapi.yml
  format: yaml
  label: Dodo Payments Webhooks API
  slug: dodo-payments-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/openapi/dodo-payments-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dodopayments.com
  spf: true
hosts:
- cert_expires: Oct  2 17:29:55 2026 GMT
  host: dodopayments.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 19:30:52 2026 GMT
  host: docs.dodopayments.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 14:44:12 2026 GMT
  host: live.dodopayments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dodo Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dodo Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dodo Payments
provider_slug: dodo-payments
slug: dodo-payments-domain-security
source_filename: dodo-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dodopayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:29:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.dodopayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:30:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: live.dodopayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 14:44:12 2026 GMT\n  hsts: null\ndomains:\n- domain: dodopayments.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dodo-payments/refs/heads/main/security/dodo-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Merchant of Record
- Subscriptions
- Billing
- Global Commerce
---
