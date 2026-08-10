---
api_specs:
- filename: also-cart-api-openapi.yml
  format: yaml
  label: Also Cart API
  slug: also-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/openapi/also-cart-api-openapi.yml
- filename: also-collections-api-openapi.yml
  format: yaml
  label: Also Collections API
  slug: also-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/openapi/also-collections-api-openapi.yml
- filename: also-products-api-openapi.yml
  format: yaml
  label: Also Products API
  slug: also-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/openapi/also-products-api-openapi.yml
- filename: also-search-api-openapi.yml
  format: yaml
  label: Also Search API
  slug: also-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/openapi/also-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ridealso.com
  spf: true
hosts:
- cert_expires: Oct 12 05:30:31 2026 GMT
  host: ridealso.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Also Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Also, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Also
provider_slug: also
slug: also-domain-security
source_filename: also-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ridealso.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:30:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: ridealso.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/also/refs/heads/main/security/also-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Micromobility
- Electric Vehicles
- Transportation
- E-Commerce
- Consumer Hardware
- Agentic Commerce
- Logistics
- Delivery
---
