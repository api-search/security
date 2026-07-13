---
api_specs:
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Subscriptions API
  slug: bold-commerce-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Checkout API
  slug: bold-commerce-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Price Rules API
  slug: bold-commerce-price-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Products API
  slug: bold-commerce-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Customers API
  slug: bold-commerce-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
- filename: bold-commerce-openapi.yml
  format: yaml
  label: Bold Shops API
  slug: bold-commerce-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/openapi/bold-commerce-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: boldcommerce.com
  spf: true
hosts:
- cert_expires: Sep 20 03:20:30 2026 GMT
  host: boldcommerce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:07:15 2026 GMT
  host: developer.boldcommerce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 18:00:41 2026 GMT
  host: api.boldcommerce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bold Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bold Commerce, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bold Commerce
provider_slug: bold-commerce
slug: bold-commerce-domain-security
source_filename: bold-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boldcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:20:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.boldcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:07:15 2026 GMT\n  hsts: false\n- host: api.boldcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:00:41 2026 GMT\n  hsts: false\ndomains:\n- domain: boldcommerce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bold-commerce/refs/heads/main/security/bold-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- E-Commerce
- Subscriptions
- Checkout
- Pricing
- Headless Commerce
- Shopify
---
