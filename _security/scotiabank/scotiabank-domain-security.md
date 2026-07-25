---
api_specs:
- filename: scotiabank-account-validation-api-openapi.yml
  format: yaml
  label: Scotiabank Account Validation API
  slug: scotiabank-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-account-validation-api-openapi.yml
- filename: scotiabank-accounts-api-openapi.yml
  format: yaml
  label: Scotiabank Accounts API
  slug: scotiabank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-accounts-api-openapi.yml
- filename: scotiabank-eft-payments-api-openapi.yml
  format: yaml
  label: Scotiabank EFT Payments API
  slug: scotiabank-eft-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-eft-payments-api-openapi.yml
- filename: scotiabank-payment-tracking-api-openapi.yml
  format: yaml
  label: Scotiabank Payment Tracking API
  slug: scotiabank-payment-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-payment-tracking-api-openapi.yml
- filename: scotiabank-real-time-payments-api-openapi.yml
  format: yaml
  label: Scotiabank Real-Time Payments API
  slug: scotiabank-real-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-real-time-payments-api-openapi.yml
- filename: scotiabank-request-for-payment-api-openapi.yml
  format: yaml
  label: Scotiabank Request for Payment API
  slug: scotiabank-request-for-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-request-for-payment-api-openapi.yml
- filename: scotiabank-wire-payments-api-openapi.yml
  format: yaml
  label: Scotiabank Wire Payments API
  slug: scotiabank-wire-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/openapi/scotiabank-wire-payments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scotiabank.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: developer.scotiabank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: developer.api.scotiabank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scotiabank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scotiabank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scotiabank
provider_slug: scotiabank
slug: scotiabank-domain-security
source_filename: scotiabank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.scotiabank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.api.scotiabank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scotiabank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scotiabank/refs/heads/main/security/scotiabank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Finance
- Payments
- Canada
- Open Banking
---
