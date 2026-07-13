---
api_specs:
- filename: wayfair-supplier-api.yml
  format: yaml
  label: Wayfair Supplier API
  slug: wayfair-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wayfair/refs/heads/main/openapi/wayfair-supplier-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wayfair.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wayfair.io
  spf: false
hosts:
- cert_expires: Oct  9 05:31:29 2026 GMT
  host: developer.wayfair.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 17:17:54 2026 GMT
  host: developer.wayfair.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 09:10:37 2026 GMT
  host: www.wayfair.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wayfair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wayfair, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wayfair
provider_slug: wayfair
slug: wayfair-domain-security
source_filename: wayfair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.wayfair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:31:29 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.wayfair.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:17:54 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.wayfair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:10:37 2026 GMT\n  hsts: null\ndomains:\n- domain: wayfair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wayfair.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wayfair/refs/heads/main/security/wayfair-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Furniture
- Home Goods
- Retail
- Suppliers
- GraphQL
---
