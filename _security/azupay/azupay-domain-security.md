---
api_specs:
- filename: azupay-api-keys-api-openapi.yml
  format: yaml
  label: Azupay API Keys API
  slug: azupay-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-api-keys-api-openapi.yml
- filename: azupay-billing-and-transaction-reports-api-openapi.yml
  format: yaml
  label: Azupay Billing and Transaction Reports API
  slug: azupay-billing-and-transaction-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-billing-and-transaction-reports-api-openapi.yml
- filename: azupay-check-accounts-api-openapi.yml
  format: yaml
  label: Azupay Check Accounts API
  slug: azupay-check-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-check-accounts-api-openapi.yml
- filename: azupay-clients-api-openapi.yml
  format: yaml
  label: Azupay Clients API
  slug: azupay-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-clients-api-openapi.yml
- filename: azupay-current-balances-api-openapi.yml
  format: yaml
  label: Azupay Current Balances API
  slug: azupay-current-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-current-balances-api-openapi.yml
- filename: azupay-payment-agreement-api-openapi.yml
  format: yaml
  label: Azupay Payment Agreement API
  slug: azupay-payment-agreement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-agreement-api-openapi.yml
- filename: azupay-payment-agreement-request-api-openapi.yml
  format: yaml
  label: Azupay Payment Agreement Request API
  slug: azupay-payment-agreement-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-agreement-request-api-openapi.yml
- filename: azupay-payment-api-openapi.yml
  format: yaml
  label: Azupay Payment API
  slug: azupay-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-api-openapi.yml
- filename: azupay-payment-initiation-api-openapi.yml
  format: yaml
  label: Azupay Payment Initiation API
  slug: azupay-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-initiation-api-openapi.yml
- filename: azupay-payment-request-api-openapi.yml
  format: yaml
  label: Azupay Payment Request API
  slug: azupay-payment-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-request-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azupay.com.au
  spf: true
hosts:
- cert_expires: Sep 13 22:30:29 2026 GMT
  host: azupay.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 00:38:05 2026 GMT
  host: developer.azupay.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api.azupay.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Azupay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azupay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azupay
provider_slug: azupay
slug: azupay-domain-security
source_filename: azupay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azupay.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:30:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.azupay.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:38:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.azupay.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: azupay.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/security/azupay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Real-Time Payments
- Account-to-Account
- New Payments Platform
- PayID
- PayTo
- Money Transfer
- Confirmation of Payee
- Open Banking
---
