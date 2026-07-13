---
api_specs:
- filename: abacatepay-openapi.yml
  format: yaml
  label: AbacatePay Billing and Charges API
  slug: abacatepay-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-openapi.yml
- filename: abacatepay-openapi.yml
  format: yaml
  label: AbacatePay Pix QR Code API
  slug: abacatepay-pix-qrcode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-openapi.yml
- filename: abacatepay-openapi.yml
  format: yaml
  label: AbacatePay Customers API
  slug: abacatepay-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-openapi.yml
- filename: abacatepay-openapi.yml
  format: yaml
  label: AbacatePay Coupons API
  slug: abacatepay-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-openapi.yml
- filename: abacatepay-openapi.yml
  format: yaml
  label: AbacatePay Withdraw API
  slug: abacatepay-withdraw-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/openapi/abacatepay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abacatepay.com
  spf: false
hosts:
- cert_expires: Aug 19 15:00:51 2026 GMT
  host: www.abacatepay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 17:00:27 2026 GMT
  host: docs.abacatepay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 12:16:02 2026 GMT
  host: api.abacatepay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abacatepay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AbacatePay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AbacatePay
provider_slug: abacatepay
slug: abacatepay-domain-security
source_filename: abacatepay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abacatepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:00:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.abacatepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 17:00:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.abacatepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 12:16:02 2026 GMT\n  hsts: false\ndomains:\n- domain: abacatepay.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abacatepay/refs/heads/main/security/abacatepay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Pix
- Brazil
- FinTech
- Developers
---
