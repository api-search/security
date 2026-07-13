---
api_specs:
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Products API
  slug: paddle-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Prices API
  slug: paddle-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Customers API
  slug: paddle-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Subscriptions API
  slug: paddle-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Transactions API
  slug: paddle-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Adjustments API
  slug: paddle-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Discounts API
  slug: paddle-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
- filename: paddle-openapi.yml
  format: yaml
  label: Paddle Notifications API
  slug: paddle-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/openapi/paddle-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paddle.com
  spf: true
hosts:
- cert_expires: Sep 11 12:23:57 2026 GMT
  host: www.paddle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 04:23:43 2026 GMT
  host: developer.paddle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 16:26:49 2026 GMT
  host: api.paddle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paddle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paddle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paddle
provider_slug: paddle
slug: paddle-domain-security
source_filename: paddle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paddle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:23:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.paddle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:23:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.paddle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 16:26:49 2026 GMT\n  hsts: null\ndomains:\n- domain: paddle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paddle/refs/heads/main/security/paddle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Payments
- Subscriptions
- Merchant of Record
- SaaS
---
