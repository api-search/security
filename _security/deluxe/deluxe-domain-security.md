---
api_specs:
- filename: deluxe-american-api-openapi.yml
  format: yaml
  label: Deluxe Corporation American API
  slug: deluxe-american-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-american-api-openapi.yml
- filename: deluxe-batches-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Batches API
  slug: deluxe-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-batches-api-openapi.yml
- filename: deluxe-customers-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Customers API
  slug: deluxe-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-customers-api-openapi.yml
- filename: deluxe-emv-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Emv API
  slug: deluxe-emv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-emv-api-openapi.yml
- filename: deluxe-events-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Events API
  slug: deluxe-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-events-api-openapi.yml
- filename: deluxe-invoices-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Invoices API
  slug: deluxe-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-invoices-api-openapi.yml
- filename: deluxe-paymentlinks-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Paymentlinks API
  slug: deluxe-paymentlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-paymentlinks-api-openapi.yml
- filename: deluxe-paymentmethods-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Paymentmethods API
  slug: deluxe-paymentmethods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-paymentmethods-api-openapi.yml
- filename: deluxe-payments-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Payments API
  slug: deluxe-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-payments-api-openapi.yml
- filename: deluxe-refunds-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Refunds API
  slug: deluxe-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-refunds-api-openapi.yml
- filename: deluxe-reports-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Reports API
  slug: deluxe-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-reports-api-openapi.yml
- filename: deluxe-secservices-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Secservices API
  slug: deluxe-secservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-secservices-api-openapi.yml
- filename: deluxe-subscriptions-api-openapi.yml
  format: yaml
  label: Deluxe Corporation Subscriptions API
  slug: deluxe-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/openapi/deluxe-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deluxe.com
  spf: false
hosts:
- cert_expires: Oct 26 04:41:06 2026 GMT
  host: www.deluxe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 16:31:34 2026 GMT
  host: developer.deluxe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 18:46:19 2026 GMT
  host: api.deluxe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deluxe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deluxe Corporation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Deluxe Corporation
provider_slug: deluxe
slug: deluxe-domain-security
source_filename: deluxe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deluxe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 04:41:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.deluxe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 16:31:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.deluxe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:46:19 2026 GMT\n  hsts: null\ndomains:\n- domain: deluxe.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deluxe/refs/heads/main/security/deluxe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Merchant Services
- Card Processing
- ACH
- Invoicing
- Subscription
- Tokenization
- Webhook
- Reporting
- Data Analytics
- Marketing
- Small Business
---
