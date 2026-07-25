---
api_specs:
- filename: prodsmart-authorization-api-openapi.yml
  format: yaml
  label: Prodsmart Authorization API
  slug: prodsmart-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-authorization-api-openapi.yml
- filename: prodsmart-changes-feed-api-openapi.yml
  format: yaml
  label: Prodsmart Changes Feed API
  slug: prodsmart-changes-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-changes-feed-api-openapi.yml
- filename: prodsmart-clients-api-openapi.yml
  format: yaml
  label: Prodsmart Clients API
  slug: prodsmart-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-clients-api-openapi.yml
- filename: prodsmart-downtime-api-openapi.yml
  format: yaml
  label: Prodsmart Downtime API
  slug: prodsmart-downtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-downtime-api-openapi.yml
- filename: prodsmart-inventory-api-openapi.yml
  format: yaml
  label: Prodsmart Inventory API
  slug: prodsmart-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-inventory-api-openapi.yml
- filename: prodsmart-machines-api-openapi.yml
  format: yaml
  label: Prodsmart Machines API
  slug: prodsmart-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-machines-api-openapi.yml
- filename: prodsmart-product-families-api-openapi.yml
  format: yaml
  label: Prodsmart Product Families API
  slug: prodsmart-product-families-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-product-families-api-openapi.yml
- filename: prodsmart-production-orders-api-openapi.yml
  format: yaml
  label: Prodsmart Production Orders API
  slug: prodsmart-production-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-production-orders-api-openapi.yml
- filename: prodsmart-productions-api-openapi.yml
  format: yaml
  label: Prodsmart Productions API
  slug: prodsmart-productions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-productions-api-openapi.yml
- filename: prodsmart-products-api-openapi.yml
  format: yaml
  label: Prodsmart Products API
  slug: prodsmart-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-products-api-openapi.yml
- filename: prodsmart-punch-clock-api-openapi.yml
  format: yaml
  label: Prodsmart Punch Clock API
  slug: prodsmart-punch-clock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-punch-clock-api-openapi.yml
- filename: prodsmart-purchase-orders-api-openapi.yml
  format: yaml
  label: Prodsmart Purchase Orders API
  slug: prodsmart-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-purchase-orders-api-openapi.yml
- filename: prodsmart-reports-api-openapi.yml
  format: yaml
  label: Prodsmart Reports API
  slug: prodsmart-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-reports-api-openapi.yml
- filename: prodsmart-sales-orders-api-openapi.yml
  format: yaml
  label: Prodsmart Sales Orders API
  slug: prodsmart-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-sales-orders-api-openapi.yml
- filename: prodsmart-suppliers-api-openapi.yml
  format: yaml
  label: Prodsmart Suppliers API
  slug: prodsmart-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-suppliers-api-openapi.yml
- filename: prodsmart-task-durations-api-openapi.yml
  format: yaml
  label: Prodsmart Task Durations API
  slug: prodsmart-task-durations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/openapi/prodsmart-task-durations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prodsmart.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: prodsmart.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Prodsmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prodsmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prodsmart
provider_slug: prodsmart
slug: prodsmart-domain-security
source_filename: prodsmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prodsmart.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: prodsmart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prodsmart/refs/heads/main/security/prodsmart-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Manufacturing
- Manufacturing Execution System
- Production Management
- Inventory
- Shop Floor
- Autodesk
- Industry 4.0
---
