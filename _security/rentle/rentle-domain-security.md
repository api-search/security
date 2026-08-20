---
api_specs:
- filename: rentle-api-keys-api-openapi.yml
  format: yaml
  label: Rentle API Keys API
  slug: rentle-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-api-keys-api-openapi.yml
- filename: rentle-categories-api-openapi.yml
  format: yaml
  label: Rentle Categories API
  slug: rentle-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-categories-api-openapi.yml
- filename: rentle-customers-api-openapi.yml
  format: yaml
  label: Rentle Customers API
  slug: rentle-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-customers-api-openapi.yml
- filename: rentle-discount-codes-api-openapi.yml
  format: yaml
  label: Rentle Discount Codes API
  slug: rentle-discount-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-discount-codes-api-openapi.yml
- filename: rentle-inventory-articles-api-openapi.yml
  format: yaml
  label: Rentle Inventory Articles API
  slug: rentle-inventory-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-inventory-articles-api-openapi.yml
- filename: rentle-inventory-skus-api-openapi.yml
  format: yaml
  label: Rentle Inventory SKUs API
  slug: rentle-inventory-skus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-inventory-skus-api-openapi.yml
- filename: rentle-merchant-api-openapi.yml
  format: yaml
  label: Rentle Merchant API
  slug: rentle-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-merchant-api-openapi.yml
- filename: rentle-orders-api-openapi.yml
  format: yaml
  label: Rentle Orders API
  slug: rentle-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-orders-api-openapi.yml
- filename: rentle-products-api-openapi.yml
  format: yaml
  label: Rentle Products API
  slug: rentle-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-products-api-openapi.yml
- filename: rentle-stores-api-openapi.yml
  format: yaml
  label: Rentle Stores API
  slug: rentle-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-stores-api-openapi.yml
- filename: rentle-webhooks-api-openapi.yml
  format: yaml
  label: Rentle Webhooks API
  slug: rentle-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: twicecommerce.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rentle.io
  spf: true
hosts:
- cert_expires: Aug 21 14:10:42 2026 GMT
  host: www.twicecommerce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 21:10:39 2026 GMT
  host: api.rentle.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 09:55:00 2026 GMT
  host: api.twicecommerce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rentle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rentle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rentle
provider_slug: rentle
slug: rentle-domain-security
source_filename: rentle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.twicecommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 14:10:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rentle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:10:39 2026 GMT\n  hsts: null\n- host: api.twicecommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:55:00 2026 GMT\n  hsts: null\ndomains:\n- domain: twicecommerce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rentle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/security/rentle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Rentals
- Commerce
- E-Commerce
- Circular Economy
- Resale
- Subscription
- Bookings
- Webhook
- Software-as-a-Service
---
