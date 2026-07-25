---
api_specs:
- filename: bitpay-bills-api-openapi.yml
  format: yaml
  label: BitPay Bills API
  slug: bitpay-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-bills-api-openapi.yml
- filename: bitpay-payouts-api-openapi.yml
  format: yaml
  label: BitPay Payouts API
  slug: bitpay-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-payouts-api-openapi.yml
- filename: bitpay-refunds-api-openapi.yml
  format: yaml
  label: BitPay Refunds API
  slug: bitpay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-refunds-api-openapi.yml
- filename: bitpay-settlements-api-openapi.yml
  format: yaml
  label: BitPay Settlements API
  slug: bitpay-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-settlements-api-openapi.yml
- filename: bitpay-rates-api-openapi.yml
  format: yaml
  label: BitPay Rates API
  slug: bitpay-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-rates-api-openapi.yml
- filename: bitpay-ledgers-api-openapi.yml
  format: yaml
  label: BitPay Ledgers API
  slug: bitpay-ledgers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-ledgers-api-openapi.yml
- filename: bitpay-bills-api-openapi.yml
  format: yaml
  label: BitPay Bills API
  slug: bitpay-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-bills-api-openapi.yml
- filename: bitpay-invoices-api-openapi.yml
  format: yaml
  label: BitPay Invoices API
  slug: bitpay-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-invoices-api-openapi.yml
- filename: bitpay-ledgers-api-openapi.yml
  format: yaml
  label: BitPay Ledgers API
  slug: bitpay-ledgers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-ledgers-api-openapi.yml
- filename: bitpay-payouts-api-openapi.yml
  format: yaml
  label: BitPay Payouts API
  slug: bitpay-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-payouts-api-openapi.yml
- filename: bitpay-rates-api-openapi.yml
  format: yaml
  label: BitPay Rates API
  slug: bitpay-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-rates-api-openapi.yml
- filename: bitpay-refunds-api-openapi.yml
  format: yaml
  label: BitPay Refunds API
  slug: bitpay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-refunds-api-openapi.yml
- filename: bitpay-settlements-api-openapi.yml
  format: yaml
  label: BitPay Settlements API
  slug: bitpay-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/openapi/bitpay-settlements-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bitpay.com
  spf: true
hosts:
- cert_expires: Sep 20 10:14:07 2026 GMT
  host: developer.bitpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 21:13:07 2026 GMT
  host: bitpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 21:13:07 2026 GMT
  host: test.bitpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitPay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BitPay
provider_slug: bitpay
slug: bitpay-domain-security
source_filename: bitpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.bitpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 10:14:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bitpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:13:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: test.bitpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:13:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bitpay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitpay/refs/heads/main/security/bitpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Payments
- Bitcoin
- Blockchain
- Invoices
- Payouts
- Settlement
---
