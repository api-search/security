---
api_specs:
- filename: depict-storefront-openapi-original.json
  format: json
  label: Depict Storefront API
  slug: depict-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depict/refs/heads/main/openapi/depict-storefront-openapi-original.json
- filename: depict-portal-openapi-original.json
  format: json
  label: Depict Portal API
  slug: depict-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depict/refs/heads/main/openapi/depict-portal-openapi-original.json
- filename: depict-lite-openapi-original.json
  format: json
  label: Depict Lite API
  slug: depict-lite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depict/refs/heads/main/openapi/depict-lite-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: depict.ai
  spf: true
hosts:
- cert_expires: Oct 15 18:51:24 2026 GMT
  host: depict.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 14:50:38 2026 GMT
  host: docs.depict.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 10:54:38 2026 GMT
  host: api.depict.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Depict Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Depict, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Depict
provider_slug: depict
slug: depict-domain-security
source_filename: depict-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: depict.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:51:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.depict.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:50:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.depict.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:54:38 2026 GMT\n  hsts: null\ndomains:\n- domain: depict.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depict/refs/heads/main/security/depict-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Merchandising
- Product Recommendations
- Search
- Personalization
- Artificial Intelligence
- Retail
- Fashion
- Shopify
---
