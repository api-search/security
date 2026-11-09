---
api_specs:
- filename: buyrecord-app-keys-api-openapi.yml
  format: yaml
  label: BuyRecord Keys API
  slug: buyrecord-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-keys-api-openapi.yml
- filename: buyrecord-app-merchants-api-openapi.yml
  format: yaml
  label: BuyRecord Merchants API
  slug: buyrecord-app-merchants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-merchants-api-openapi.yml
- filename: buyrecord-app-outcomes-api-openapi.yml
  format: yaml
  label: BuyRecord Outcomes API
  slug: buyrecord-app-outcomes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-outcomes-api-openapi.yml
- filename: buyrecord-app-products-api-openapi.yml
  format: yaml
  label: BuyRecord Products API
  slug: buyrecord-app-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-products-api-openapi.yml
- filename: buyrecord-app-stays-api-openapi.yml
  format: yaml
  label: BuyRecord Stays API
  slug: buyrecord-app-stays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyrecord-app/openapi/buyrecord-app-stays-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buyrecord.app
  spf: true
hosts:
- cert_expires: Jan  3 16:28:20 2027 GMT
  host: buyrecord.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buyrecord App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuyRecord, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BuyRecord
provider_slug: buyrecord-app
slug: buyrecord-app-domain-security
source_filename: buyrecord-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buyrecord.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 16:28:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buyrecord.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buyrecord-app/security/buyrecord-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- E-Commerce
- Data
- Shopping
- Analytics
---
