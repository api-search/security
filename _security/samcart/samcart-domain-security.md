---
api_specs:
- filename: samcart-openapi.yml
  format: yaml
  label: SamCart Orders API
  slug: samcart-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samcart/refs/heads/main/openapi/samcart-openapi.yml
- filename: samcart-openapi.yml
  format: yaml
  label: SamCart Products API
  slug: samcart-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samcart/refs/heads/main/openapi/samcart-openapi.yml
- filename: samcart-openapi.yml
  format: yaml
  label: SamCart Customers API
  slug: samcart-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samcart/refs/heads/main/openapi/samcart-openapi.yml
- filename: samcart-openapi.yml
  format: yaml
  label: SamCart Subscriptions API
  slug: samcart-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samcart/refs/heads/main/openapi/samcart-openapi.yml
- filename: samcart-openapi.yml
  format: yaml
  label: SamCart Charges and Refunds API
  slug: samcart-charges-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samcart/refs/heads/main/openapi/samcart-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: samcart.com
  spf: true
hosts:
- cert_expires: Oct  7 10:47:23 2026 GMT
  host: www.samcart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: developer.samcart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.samcart.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Samcart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SamCart, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SamCart
provider_slug: samcart
slug: samcart-domain-security
source_filename: samcart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.samcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:47:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.samcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.samcart.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: samcart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samcart/refs/heads/main/security/samcart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-commerce
- Checkout
- Payments
- Subscriptions
- Digital Products
- Courses
---
