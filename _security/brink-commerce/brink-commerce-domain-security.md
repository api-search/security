---
api_specs:
- filename: brink-commerce-custom-api-openapi.yml
  format: yaml
  label: Brink Commerce Custom API
  slug: brink-commerce-custom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/brink-commerce-custom-api-openapi.yml
- filename: brink-commerce-deliveries-api-openapi.yml
  format: yaml
  label: Brink Commerce Deliveries API
  slug: brink-commerce-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/brink-commerce-deliveries-api-openapi.yml
- filename: brink-commerce-orders-api-openapi.yml
  format: yaml
  label: Brink Commerce Orders API
  slug: brink-commerce-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/brink-commerce-orders-api-openapi.yml
- filename: brink-commerce-products-api-openapi.yml
  format: yaml
  label: Brink Commerce Products API
  slug: brink-commerce-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/brink-commerce-products-api-openapi.yml
- filename: brink-commerce-technical-api-openapi.yml
  format: yaml
  label: Brink Commerce Technical API
  slug: brink-commerce-technical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/brink-commerce-technical-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brinkcommerce.com
  spf: true
hosts:
- cert_expires: Jan  5 05:24:30 2027 GMT
  host: brinkcommerce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brink Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brink Commerce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brink Commerce
provider_slug: brink-commerce
slug: brink-commerce-domain-security
source_filename: brink-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brinkcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 05:24:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brinkcommerce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/security/brink-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Platform
- Enterprise
- Composable
---
