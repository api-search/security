---
api_specs:
- filename: fudo-customers-api-openapi.yml
  format: yaml
  label: Fudo Customers API
  slug: fudo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-customers-api-openapi.yml
- filename: fudo-discounts-api-openapi.yml
  format: yaml
  label: Fudo Discounts API
  slug: fudo-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-discounts-api-openapi.yml
- filename: fudo-expense-categories-api-openapi.yml
  format: yaml
  label: Fudo Expense Categories API
  slug: fudo-expense-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-expense-categories-api-openapi.yml
- filename: fudo-expenses-api-openapi.yml
  format: yaml
  label: Fudo Expenses API
  slug: fudo-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-expenses-api-openapi.yml
- filename: fudo-ingredients-api-openapi.yml
  format: yaml
  label: Fudo Ingredients API
  slug: fudo-ingredients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-ingredients-api-openapi.yml
- filename: fudo-items-api-openapi.yml
  format: yaml
  label: Fudo Items API
  slug: fudo-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-items-api-openapi.yml
- filename: fudo-kitchens-api-openapi.yml
  format: yaml
  label: Fudo Kitchens API
  slug: fudo-kitchens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-kitchens-api-openapi.yml
- filename: fudo-payment-methods-api-openapi.yml
  format: yaml
  label: Fudo Payment Methods API
  slug: fudo-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-payment-methods-api-openapi.yml
- filename: fudo-payments-api-openapi.yml
  format: yaml
  label: Fudo Payments API
  slug: fudo-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-payments-api-openapi.yml
- filename: fudo-product-categories-api-openapi.yml
  format: yaml
  label: Fudo Product Categories API
  slug: fudo-product-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-product-categories-api-openapi.yml
- filename: fudo-product-modifiers-api-openapi.yml
  format: yaml
  label: Fudo Product Modifiers API
  slug: fudo-product-modifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-product-modifiers-api-openapi.yml
- filename: fudo-products-api-openapi.yml
  format: yaml
  label: Fudo Products API
  slug: fudo-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-products-api-openapi.yml
- filename: fudo-providers-api-openapi.yml
  format: yaml
  label: Fudo Providers API
  slug: fudo-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-providers-api-openapi.yml
- filename: fudo-roles-api-openapi.yml
  format: yaml
  label: Fudo Roles API
  slug: fudo-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-roles-api-openapi.yml
- filename: fudo-rooms-api-openapi.yml
  format: yaml
  label: Fudo Rooms API
  slug: fudo-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-rooms-api-openapi.yml
- filename: fudo-sales-api-openapi.yml
  format: yaml
  label: Fudo Sales API
  slug: fudo-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-sales-api-openapi.yml
- filename: fudo-subitems-api-openapi.yml
  format: yaml
  label: Fudo Subitems API
  slug: fudo-subitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-subitems-api-openapi.yml
- filename: fudo-tables-api-openapi.yml
  format: yaml
  label: Fudo Tables API
  slug: fudo-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-tables-api-openapi.yml
- filename: fudo-users-api-openapi.yml
  format: yaml
  label: Fudo Users API
  slug: fudo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fu.do
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: fu.do
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: dev.fu.do
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.fu.do
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fudo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fudo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fudo
provider_slug: fudo
slug: fudo-domain-security
source_filename: fudo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fu.do\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: dev.fu.do\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: api.fu.do\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fu.do\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/security/fudo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurant
- Point-of-Sale
- Hospitality
- Food and Beverage
- Payments
- Inventory
- Latin America
- Software-as-a-Service
---
