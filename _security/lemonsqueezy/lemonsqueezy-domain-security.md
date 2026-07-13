---
api_specs:
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Stores API
  slug: stores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Products & Variants API
  slug: products-variants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Subscriptions API
  slug: subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy License Keys API
  slug: license-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Checkouts API
  slug: checkouts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Discounts API
  slug: discounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
- filename: lemonsqueezy-openapi.yml
  format: yaml
  label: Lemon Squeezy Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/openapi/lemonsqueezy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lemonsqueezy.com
  spf: true
hosts:
- cert_expires: Oct  6 09:03:07 2026 GMT
  host: www.lemonsqueezy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 09:03:07 2026 GMT
  host: docs.lemonsqueezy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 09:03:07 2026 GMT
  host: api.lemonsqueezy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemonsqueezy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemon Squeezy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lemon Squeezy
provider_slug: lemonsqueezy
slug: lemonsqueezy-domain-security
source_filename: lemonsqueezy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lemonsqueezy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lemonsqueezy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lemonsqueezy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:03:07 2026 GMT\n  hsts: null\ndomains:\n- domain: lemonsqueezy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonsqueezy/refs/heads/main/security/lemonsqueezy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Merchant of Record
- Subscriptions
- Digital Products
- SaaS
- Sales Tax
---
