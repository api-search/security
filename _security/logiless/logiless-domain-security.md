---
api_specs:
- filename: logiless-articles-api-openapi.yml
  format: yaml
  label: Logiless Articles API
  slug: logiless-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-articles-api-openapi.yml
- filename: logiless-inbound-deliveries-api-openapi.yml
  format: yaml
  label: Logiless Inbound Deliveries API
  slug: logiless-inbound-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-inbound-deliveries-api-openapi.yml
- filename: logiless-inter-warehouse-transfers-api-openapi.yml
  format: yaml
  label: Logiless Inter-Warehouse Transfers API
  slug: logiless-inter-warehouse-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-inter-warehouse-transfers-api-openapi.yml
- filename: logiless-inventory-api-openapi.yml
  format: yaml
  label: Logiless Inventory API
  slug: logiless-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-inventory-api-openapi.yml
- filename: logiless-locations-api-openapi.yml
  format: yaml
  label: Logiless Locations API
  slug: logiless-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-locations-api-openapi.yml
- filename: logiless-outbound-deliveries-api-openapi.yml
  format: yaml
  label: Logiless Outbound Deliveries API
  slug: logiless-outbound-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-outbound-deliveries-api-openapi.yml
- filename: logiless-sales-orders-api-openapi.yml
  format: yaml
  label: Logiless Sales Orders API
  slug: logiless-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-sales-orders-api-openapi.yml
- filename: logiless-sales-returns-api-openapi.yml
  format: yaml
  label: Logiless Sales Returns API
  slug: logiless-sales-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-sales-returns-api-openapi.yml
- filename: logiless-suppliers-api-openapi.yml
  format: yaml
  label: Logiless Suppliers API
  slug: logiless-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-suppliers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: logiless.co.jp
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: logiless.com
  spf: true
hosts:
- host: logiless.co.jp
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: app2.logiless.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Logiless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logiless, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Logiless
provider_slug: logiless
slug: logiless-domain-security
source_filename: logiless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logiless.co.jp\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: app2.logiless.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: logiless.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: logiless.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/security/logiless-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Logistics
- E-commerce
- Order Management
- Warehouse Management
- Inventory
- Fulfillment
- Shipping
- OMS
- WMS
- Japan
---
