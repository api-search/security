---
api_specs:
- filename: scansource-product-openapi.yml
  format: yaml
  label: ScanSource Product API
  slug: scansource-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-product-openapi.yml
- filename: scansource-sales-order-openapi.yml
  format: yaml
  label: ScanSource Sales Order API
  slug: scansource-sales-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-sales-order-openapi.yml
- filename: scansource-invoice-openapi.yml
  format: yaml
  label: ScanSource Invoice API
  slug: scansource-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/openapi/scansource-invoice-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scansource.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.scansource.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: services.scansource.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scansource Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScanSource, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ScanSource
provider_slug: scansource
slug: scansource-domain-security
source_filename: scansource-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scansource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.scansource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scansource.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scansource/refs/heads/main/security/scansource-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ScanSource
- Distribution
- Barcode
- Point Of Sale
- AIDC
- Inventory
- Order Management
- E-Commerce
- Fortune 1000
---
