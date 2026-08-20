---
api_specs:
- filename: shipstation-accounts-api-openapi.yml
  format: yaml
  label: ShipStation Accounts API
  slug: shipstation-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-accounts-api-openapi.yml
- filename: shipstation-carriers-api-openapi.yml
  format: yaml
  label: ShipStation Carriers API
  slug: shipstation-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-carriers-api-openapi.yml
- filename: shipstation-customers-api-openapi.yml
  format: yaml
  label: ShipStation Customers API
  slug: shipstation-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-customers-api-openapi.yml
- filename: shipstation-fulfillments-api-openapi.yml
  format: yaml
  label: ShipStation Fulfillments API
  slug: shipstation-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-fulfillments-api-openapi.yml
- filename: shipstation-orders-api-openapi.yml
  format: yaml
  label: ShipStation Orders API
  slug: shipstation-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-orders-api-openapi.yml
- filename: shipstation-products-api-openapi.yml
  format: yaml
  label: ShipStation Products API
  slug: shipstation-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-products-api-openapi.yml
- filename: shipstation-shipments-api-openapi.yml
  format: yaml
  label: ShipStation Shipments API
  slug: shipstation-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-shipments-api-openapi.yml
- filename: shipstation-stores-api-openapi.yml
  format: yaml
  label: ShipStation Stores API
  slug: shipstation-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-stores-api-openapi.yml
- filename: shipstation-warehouses-api-openapi.yml
  format: yaml
  label: ShipStation Warehouses API
  slug: shipstation-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-warehouses-api-openapi.yml
- filename: shipstation-webhooks-api-openapi.yml
  format: yaml
  label: ShipStation Webhooks API
  slug: shipstation-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/openapi/shipstation-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shipstation.com
  spf: true
hosts:
- cert_expires: Sep 17 10:55:15 2026 GMT
  host: www.shipstation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 10:58:25 2026 GMT
  host: docs.shipstation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: ssapi.shipstation.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Shipstation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShipStation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ShipStation
provider_slug: shipstation
slug: shipstation-domain-security
source_filename: shipstation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipstation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 10:55:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.shipstation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 10:58:25 2026 GMT\n  hsts: false\n- host: ssapi.shipstation.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: shipstation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipstation/refs/heads/main/security/shipstation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Labels
- Logistics
- Order Management
- Shipping
- Warehousing
---
