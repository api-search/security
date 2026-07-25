---
api_specs:
- filename: ecwid-categories-api-openapi.yml
  format: yaml
  label: Ecwid by Lightspeed Categories API
  slug: ecwid-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecwid/refs/heads/main/openapi/ecwid-categories-api-openapi.yml
- filename: ecwid-customers-api-openapi.yml
  format: yaml
  label: Ecwid by Lightspeed Customers API
  slug: ecwid-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecwid/refs/heads/main/openapi/ecwid-customers-api-openapi.yml
- filename: ecwid-discount-coupons-api-openapi.yml
  format: yaml
  label: Ecwid by Lightspeed Discount Coupons API
  slug: ecwid-discount-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecwid/refs/heads/main/openapi/ecwid-discount-coupons-api-openapi.yml
- filename: ecwid-orders-api-openapi.yml
  format: yaml
  label: Ecwid by Lightspeed Orders API
  slug: ecwid-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecwid/refs/heads/main/openapi/ecwid-orders-api-openapi.yml
- filename: ecwid-products-api-openapi.yml
  format: yaml
  label: Ecwid by Lightspeed Products API
  slug: ecwid-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecwid/refs/heads/main/openapi/ecwid-products-api-openapi.yml
- filename: ecwid-profile-api-openapi.yml
  format: yaml
  label: Ecwid by Lightspeed Profile API
  slug: ecwid-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecwid/refs/heads/main/openapi/ecwid-profile-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ecwid.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: www.ecwid.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api-docs.ecwid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: app.ecwid.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ecwid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ecwid by Lightspeed, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ecwid by Lightspeed
provider_slug: ecwid
slug: ecwid-domain-security
source_filename: ecwid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecwid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\n- host: api-docs.ecwid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.ecwid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ecwid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecwid/refs/heads/main/security/ecwid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Online Store
- Storefront
- Retail
- Point of Sale
- Multi-Channel Commerce
---
