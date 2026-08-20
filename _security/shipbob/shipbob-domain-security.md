---
api_specs:
- filename: shipbob-subpackage-billing-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_billing API
  slug: shipbob-subpackage-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-billing-api-openapi.yml
- filename: shipbob-subpackage-channels-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_channels API
  slug: shipbob-subpackage-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-channels-api-openapi.yml
- filename: shipbob-subpackage-inventory-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_inventory API
  slug: shipbob-subpackage-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-inventory-api-openapi.yml
- filename: shipbob-subpackage-locations-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_locations API
  slug: shipbob-subpackage-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-locations-api-openapi.yml
- filename: shipbob-subpackage-orders-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_orders API
  slug: shipbob-subpackage-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-orders-api-openapi.yml
- filename: shipbob-subpackage-products-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_products API
  slug: shipbob-subpackage-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-products-api-openapi.yml
- filename: shipbob-subpackage-receiving-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_receiving API
  slug: shipbob-subpackage-receiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-receiving-api-openapi.yml
- filename: shipbob-subpackage-returns-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_returns API
  slug: shipbob-subpackage-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-returns-api-openapi.yml
- filename: shipbob-subpackage-simulations-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_simulations API
  slug: shipbob-subpackage-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-simulations-api-openapi.yml
- filename: shipbob-subpackage-webhooks-api-openapi.yml
  format: yaml
  label: ShipBob subpackage_webhooks API
  slug: shipbob-subpackage-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/openapi/shipbob-subpackage-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shipbob.com
  spf: true
hosts:
- cert_expires: Sep 23 15:51:24 2026 GMT
  host: www.shipbob.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:30:22 2026 GMT
  host: developer.shipbob.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 15:51:24 2026 GMT
  host: api.shipbob.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shipbob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShipBob, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ShipBob
provider_slug: shipbob
slug: shipbob-domain-security
source_filename: shipbob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipbob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:51:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.shipbob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:30:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.shipbob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:51:24 2026 GMT\n  hsts: null\ndomains:\n- domain: shipbob.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/security/shipbob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Fulfillment
- 3PL
- E-Commerce
- Inventory
- Warehousing
- Shipping
- Direct to Consumer
---
