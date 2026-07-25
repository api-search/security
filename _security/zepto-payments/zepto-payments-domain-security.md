---
api_specs:
- filename: zepto-payments-zepto.yml
  format: yaml
  label: Zepto API
  slug: zepto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-zepto.yml
- filename: zepto-payments-pay-to.yml
  format: yaml
  label: Zepto PayTo API
  slug: payto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-pay-to.yml
- filename: zepto-payments-validate-cop.yml
  format: yaml
  label: Zepto Validate API (Confirmation of Payee)
  slug: validate-cop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-validate-cop.yml
- filename: zepto-payments-investigations.yml
  format: yaml
  label: Zepto Investigations API
  slug: investigations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-investigations.yml
- filename: zepto-payments-clients.yml
  format: yaml
  label: Zepto Clients API
  slug: clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-clients.yml
- filename: zepto-payments-merchant-reports.yml
  format: yaml
  label: Zepto Merchant Reports API
  slug: merchant-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-merchant-reports.yml
- filename: zepto-payments-notifications.yml
  format: yaml
  label: Zepto Notifications API (Webhooks)
  slug: notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-notifications.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zepto.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zeptopayments.com
  spf: true
hosts:
- cert_expires: Oct  2 03:14:43 2026 GMT
  host: zepto.com.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 22:17:52 2026 GMT
  host: docs.zeptopayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 10:06:51 2026 GMT
  host: api.zeptopayments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zepto Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zepto, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zepto
provider_slug: zepto-payments
slug: zepto-payments-domain-security
source_filename: zepto-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zepto.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:14:43 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.zeptopayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:17:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.zeptopayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 10:06:51 2026 GMT\n  hsts: null\ndomains:\n- domain: zepto.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zeptopayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/security/zepto-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Real-Time Payments
- Account-to-Account
- New Payments Platform
- PayTo
- PayID
- Direct Entry
- Open Banking
- Money Movement
---
