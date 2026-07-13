---
api_specs:
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Customers API
  slug: hyperline-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Products & Plans API
  slug: hyperline-products-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Subscriptions API
  slug: hyperline-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Usage & Events API
  slug: hyperline-usage-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Invoices API
  slug: hyperline-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Payments API
  slug: hyperline-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
- filename: hyperline-openapi.yml
  format: yaml
  label: Hyperline Webhooks API
  slug: hyperline-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/openapi/hyperline-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hyperline.co
  spf: true
hosts:
- cert_expires: Oct  3 10:25:58 2026 GMT
  host: www.hyperline.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 16:05:18 2026 GMT
  host: docs.hyperline.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 09:48:28 2026 GMT
  host: api.hyperline.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperline, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hyperline
provider_slug: hyperline
slug: hyperline-domain-security
source_filename: hyperline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyperline.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:25:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.hyperline.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:05:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hyperline.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:48:28 2026 GMT\n  hsts: null\ndomains:\n- domain: hyperline.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperline/refs/heads/main/security/hyperline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Subscriptions
- Usage-Based
- Metering
- Payments
- Invoicing
- FinOps
---
