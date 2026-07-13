---
api_specs:
- filename: printify-openapi.yml
  format: yaml
  label: Printify Shops API
  slug: printify-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Catalog API
  slug: printify-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Products API
  slug: printify-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Orders API
  slug: printify-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Uploads API
  slug: printify-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
- filename: printify-openapi.yml
  format: yaml
  label: Printify Webhooks API
  slug: printify-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/openapi/printify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: printify.com
  spf: true
hosts:
- cert_expires: Sep 29 13:30:14 2026 GMT
  host: printify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 13:30:14 2026 GMT
  host: developers.printify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 13:30:14 2026 GMT
  host: api.printify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Printify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Printify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Printify
provider_slug: printify
slug: printify-domain-security
source_filename: printify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: printify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:30:14 2026 GMT\n  hsts: false\n- host: developers.printify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:30:14 2026 GMT\n  hsts: false\n- host: api.printify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:30:14 2026 GMT\n  hsts: null\ndomains:\n- domain: printify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printify/refs/heads/main/security/printify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Print on Demand
- Ecommerce
- Marketplace
- Fulfillment
- Merchandise
---
