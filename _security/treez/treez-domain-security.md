---
api_specs:
- filename: treez-dispensary-openapi.json
  format: json
  label: Treez Dispensary API v3
  slug: treez-dispensary-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-dispensary-openapi.json
- filename: treez-catalog-openapi.json
  format: json
  label: Treez Catalog Service API
  slug: treez-catalog-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-catalog-openapi.json
- filename: treez-discount-openapi.json
  format: json
  label: Treez Discount Service API
  slug: treez-discount-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-discount-openapi.json
- filename: treez-collections-openapi.json
  format: json
  label: Treez Collection Service API
  slug: treez-collection-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-collections-openapi.json
- filename: treez-tag-openapi.json
  format: json
  label: Treez Tag Service API
  slug: treez-tag-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-tag-openapi.json
- filename: treez-jwt-check-openapi.json
  format: json
  label: Treez JWT Validation Service
  slug: treez-jwt-validation-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-jwt-check-openapi.json
- filename: treez-product-api-openapi.json
  format: json
  label: Treez Legacy SellTreez v2.0 Product API
  slug: treez-legacy-selltreez-v20-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/openapi/treez-product-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: treez.io
  spf: true
hosts:
- cert_expires: Nov  1 06:50:48 2026 GMT
  host: www.treez.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 05:01:54 2026 GMT
  host: code.treez.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: api-prod.treez.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Treez Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Treez, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Treez
provider_slug: treez
slug: treez-domain-security
source_filename: treez-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.treez.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 06:50:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: code.treez.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:01:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-prod.treez.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: treez.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treez/refs/heads/main/security/treez-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- cannabis
- point-of-sale
- Retail
- dispensary
- inventory-management
- E-Commerce
- Payments
- Compliance
- Track and Trace
- metrc
- product-catalog
- customer-data
---
