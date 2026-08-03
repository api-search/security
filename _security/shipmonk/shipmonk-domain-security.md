---
api_specs:
- filename: shipmonk-orders-openapi.yml
  format: yaml
  label: ShipMonk Orders API
  slug: shipmonk-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-orders-openapi.yml
- filename: shipmonk-products-openapi.yml
  format: yaml
  label: ShipMonk Products API
  slug: shipmonk-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-products-openapi.yml
- filename: shipmonk-receivings-openapi.yml
  format: yaml
  label: ShipMonk Receivings API
  slug: shipmonk-receivings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-receivings-openapi.yml
- filename: shipmonk-returns-openapi.yml
  format: yaml
  label: ShipMonk Returns API
  slug: shipmonk-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-returns-openapi.yml
- filename: shipmonk-warehouses-openapi.yml
  format: yaml
  label: ShipMonk Warehouses API
  slug: shipmonk-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/openapi/shipmonk-warehouses-openapi.yml
- filename: shipmonk-webhooks-asyncapi.yml
  format: yaml
  label: ShipMonk Webhooks
  slug: shipmonk-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/asyncapi/shipmonk-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shipmonk.com
  spf: true
hosts:
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 22:12:32 2026 GMT
  host: api.shipmonk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 02:58:47 2026 GMT
  host: sandbox.shipmonk.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shipmonk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShipMonk, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ShipMonk
provider_slug: shipmonk
slug: shipmonk-domain-security
source_filename: shipmonk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n- host: api.shipmonk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 22:12:32 2026 GMT\n  hsts: null\n- host: sandbox.shipmonk.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 02:58:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: shipmonk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipmonk/refs/heads/main/security/shipmonk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Fulfillment
- 3PL
- Ecommerce
- Warehousing
- Inventory
- Shipping
- Returns
- Supply Chain
- Direct-to-Consumer
- Order Management
---
