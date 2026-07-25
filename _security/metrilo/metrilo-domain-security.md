---
api_specs:
- filename: metrilo-categories-api-openapi.yml
  format: yaml
  label: Metrilo Categories API
  slug: metrilo-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-categories-api-openapi.yml
- filename: metrilo-customers-api-openapi.yml
  format: yaml
  label: Metrilo Customers API
  slug: metrilo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-customers-api-openapi.yml
- filename: metrilo-orders-api-openapi.yml
  format: yaml
  label: Metrilo Orders API
  slug: metrilo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-orders-api-openapi.yml
- filename: metrilo-products-api-openapi.yml
  format: yaml
  label: Metrilo Products API
  slug: metrilo-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mtrl.me
  spf: true
hosts:
- cert_expires: Sep  8 22:55:37 2026 GMT
  host: trk.mtrl.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metrilo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metrilo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Metrilo
provider_slug: metrilo
slug: metrilo-domain-security
source_filename: metrilo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trk.mtrl.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:55:37 2026 GMT\n  hsts: null\ndomains:\n- domain: mtrl.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/security/metrilo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ecommerce
- Analytics
- CRM
- Email Marketing
- Customer Retention
- Tracking
- Marketing
---
