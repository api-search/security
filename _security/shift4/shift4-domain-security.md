---
api_specs:
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 Transactions API
  slug: shift4-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 Tokens API
  slug: shift4-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 Gift Cards API
  slug: shift4-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 Devices API
  slug: shift4-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 ACH API
  slug: shift4-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 Alternative & QR Payments API
  slug: shift4-alternative-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 3D Secure & Risk API
  slug: shift4-3d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 Payment Links API
  slug: shift4-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 Checkout Sessions API
  slug: shift4-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 OCT Payouts API
  slug: shift4-oct-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
- filename: shift4-payment-api.yml
  format: yaml
  label: Shift4 Reports & Merchants API
  slug: shift4-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/openapi/shift4-payment-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shift4.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: shift4api.net
  spf: false
hosts:
- cert_expires: Sep 23 06:56:58 2026 GMT
  host: www.shift4.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 19:50:59 2026 GMT
  host: docs.shift4.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: api.shift4api.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Shift4 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shift4, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shift4
provider_slug: shift4
slug: shift4-domain-security
source_filename: shift4-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shift4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:56:58 2026 GMT\n  hsts: null\n- host: docs.shift4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:50:59 2026 GMT\n  hsts: false\n- host: api.shift4api.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: shift4.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: shift4api.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shift4/refs/heads/main/security/shift4-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- United States
- Payment Processing
- Payment Gateway
- Acquiring
- Payment Terminal
- Tokenization
- ACH
- 3D Secure
- Gift Cards
- Payment Links
- Card Present
---
