---
api_specs:
- filename: printful-catalog-api-openapi.yml
  format: yaml
  label: Printful Catalog API
  slug: printful-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-catalog-api-openapi.yml
- filename: printful-files-api-openapi.yml
  format: yaml
  label: Printful Files API
  slug: printful-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-files-api-openapi.yml
- filename: printful-mockup-generator-api-openapi.yml
  format: yaml
  label: Printful Mockup Generator API
  slug: printful-mockup-generator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-mockup-generator-api-openapi.yml
- filename: printful-orders-api-openapi.yml
  format: yaml
  label: Printful Orders API
  slug: printful-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-orders-api-openapi.yml
- filename: printful-shipping-rates-api-openapi.yml
  format: yaml
  label: Printful Shipping Rates API
  slug: printful-shipping-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-shipping-rates-api-openapi.yml
- filename: printful-store-products-api-openapi.yml
  format: yaml
  label: Printful Store Products API
  slug: printful-store-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-store-products-api-openapi.yml
- filename: printful-warehouse-api-openapi.yml
  format: yaml
  label: Printful Warehouse API
  slug: printful-warehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-warehouse-api-openapi.yml
- filename: printful-webhooks-api-openapi.yml
  format: yaml
  label: Printful Webhooks API
  slug: printful-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/openapi/printful-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: printful.com
  spf: true
hosts:
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: www.printful.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: developers.printful.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: api.printful.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Printful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Printful, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Printful
provider_slug: printful
slug: printful-domain-security
source_filename: printful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.printful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.printful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.printful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: printful.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printful/refs/heads/main/security/printful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Print on Demand
- Fulfillment
- E-Commerce
- Dropshipping
- Merchandise
---
