---
api_specs:
- filename: fastspring-accounts-api-openapi.yml
  format: yaml
  label: FastSpring Accounts API
  slug: fastspring-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-accounts-api-openapi.yml
- filename: fastspring-coupons-api-openapi.yml
  format: yaml
  label: FastSpring Coupons API
  slug: fastspring-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-coupons-api-openapi.yml
- filename: fastspring-data-api-openapi.yml
  format: yaml
  label: FastSpring Data API
  slug: fastspring-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-data-api-openapi.yml
- filename: fastspring-events-api-openapi.yml
  format: yaml
  label: FastSpring Events API
  slug: fastspring-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-events-api-openapi.yml
- filename: fastspring-invoices-api-openapi.yml
  format: yaml
  label: FastSpring Invoices API
  slug: fastspring-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-invoices-api-openapi.yml
- filename: fastspring-orders-api-openapi.yml
  format: yaml
  label: FastSpring Orders API
  slug: fastspring-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-orders-api-openapi.yml
- filename: fastspring-products-api-openapi.yml
  format: yaml
  label: FastSpring Products API
  slug: fastspring-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-products-api-openapi.yml
- filename: fastspring-quotes-api-openapi.yml
  format: yaml
  label: FastSpring Quotes API
  slug: fastspring-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-quotes-api-openapi.yml
- filename: fastspring-returns-api-openapi.yml
  format: yaml
  label: FastSpring Returns API
  slug: fastspring-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-returns-api-openapi.yml
- filename: fastspring-sessions-api-openapi.yml
  format: yaml
  label: FastSpring Sessions API
  slug: fastspring-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-sessions-api-openapi.yml
- filename: fastspring-subscriptions-api-openapi.yml
  format: yaml
  label: FastSpring Subscriptions API
  slug: fastspring-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-subscriptions-api-openapi.yml
- filename: fastspring-webhooks-api-openapi.yml
  format: yaml
  label: FastSpring Webhooks API
  slug: fastspring-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/openapi/fastspring-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fastspring.com
  spf: true
hosts:
- cert_expires: Aug 20 19:19:33 2026 GMT
  host: fastspring.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 22:54:30 2026 GMT
  host: developer.fastspring.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.fastspring.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fastspring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FastSpring, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FastSpring
provider_slug: fastspring
slug: fastspring-domain-security
source_filename: fastspring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fastspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:19:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.fastspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 22:54:30 2026 GMT\n  hsts: null\n- host: api.fastspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fastspring.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastspring/refs/heads/main/security/fastspring-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ecommerce
- Merchant of Record
- Subscription Billing
- Payments
- SaaS Billing
- Checkout
- Tax Compliance
---
