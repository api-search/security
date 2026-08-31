---
api_specs:
- filename: finditparts-addresses-api-openapi.yml
  format: yaml
  label: FinditParts Addresses API
  slug: finditparts-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-addresses-api-openapi.yml
- filename: finditparts-carts-api-openapi.yml
  format: yaml
  label: FinditParts Carts API
  slug: finditparts-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-carts-api-openapi.yml
- filename: finditparts-orders-api-openapi.yml
  format: yaml
  label: FinditParts Orders API
  slug: finditparts-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-orders-api-openapi.yml
- filename: finditparts-partners-api-openapi.yml
  format: yaml
  label: FinditParts Partners API
  slug: finditparts-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-partners-api-openapi.yml
- filename: finditparts-products-api-openapi.yml
  format: yaml
  label: FinditParts Products API
  slug: finditparts-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-products-api-openapi.yml
- filename: finditparts-reseller-customer-sessions-api-openapi.yml
  format: yaml
  label: FinditParts Reseller Customer Sessions API
  slug: finditparts-reseller-customer-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-reseller-customer-sessions-api-openapi.yml
- filename: finditparts-reseller-customers-api-openapi.yml
  format: yaml
  label: FinditParts Reseller Customers API
  slug: finditparts-reseller-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-reseller-customers-api-openapi.yml
- filename: finditparts-sessions-api-openapi.yml
  format: yaml
  label: FinditParts Sessions API
  slug: finditparts-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-sessions-api-openapi.yml
- filename: finditparts-shipping-api-openapi.yml
  format: yaml
  label: FinditParts Shipping API
  slug: finditparts-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-shipping-api-openapi.yml
- filename: finditparts-users-api-openapi.yml
  format: yaml
  label: FinditParts Users API
  slug: finditparts-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-users-api-openapi.yml
- filename: finditparts-variants-api-openapi.yml
  format: yaml
  label: FinditParts Variants API
  slug: finditparts-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/openapi/finditparts-variants-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: finditparts.com
  spf: true
hosts:
- cert_expires: Sep 16 00:00:14 2026 GMT
  host: www.finditparts.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: finditparts.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finditparts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FinditParts, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FinditParts
provider_slug: finditparts
slug: finditparts-domain-security
source_filename: finditparts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finditparts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:00:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: finditparts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: finditparts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finditparts/refs/heads/main/security/finditparts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Marketplace
- Automotive
- Parts
- Heavy Duty Trucking
- Fleet
- Logistics
- Commerce
- Catalog
- Order
- Shipping
---
