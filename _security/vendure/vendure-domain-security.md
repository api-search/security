---
api_specs:
- filename: vendure-shop-api-openapi.yml
  format: yaml
  label: Vendure Shop GraphQL API
  slug: shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendure/refs/heads/main/openapi/vendure-shop-api-openapi.yml
- filename: vendure-admin-api-openapi.yml
  format: yaml
  label: Vendure Admin GraphQL API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendure/refs/heads/main/openapi/vendure-admin-api-openapi.yml
- filename: vendure-asset-server-openapi.yml
  format: yaml
  label: Vendure Asset Server REST API
  slug: asset-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendure/refs/heads/main/openapi/vendure-asset-server-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vendure.io
  spf: true
hosts:
- cert_expires: Sep 24 21:53:03 2026 GMT
  host: vendure.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 09:01:43 2026 GMT
  host: docs.vendure.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vendure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vendure, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vendure
provider_slug: vendure
slug: vendure-domain-security
source_filename: vendure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vendure.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:53:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.vendure.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:01:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vendure.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendure/refs/heads/main/security/vendure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Headless Commerce
- eCommerce
- GraphQL
- Open Source
- TypeScript
- NestJS
- B2B
- B2C
- Storefront
- Plugins
---
