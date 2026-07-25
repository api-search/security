---
api_specs:
- filename: mile-aramex-api-openapi.yml
  format: yaml
  label: Mile Aramex API
  slug: mile-aramex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-aramex-api-openapi.yml
- filename: mile-customers-api-openapi.yml
  format: yaml
  label: Mile Customers API
  slug: mile-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-customers-api-openapi.yml
- filename: mile-debug-api-openapi.yml
  format: yaml
  label: Mile Debug API
  slug: mile-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-debug-api-openapi.yml
- filename: mile-drivers-api-openapi.yml
  format: yaml
  label: Mile Drivers API
  slug: mile-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-drivers-api-openapi.yml
- filename: mile-export-api-openapi.yml
  format: yaml
  label: Mile Export API
  slug: mile-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-export-api-openapi.yml
- filename: mile-login-api-openapi.yml
  format: yaml
  label: Mile Login API
  slug: mile-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-login-api-openapi.yml
- filename: mile-order-api-openapi.yml
  format: yaml
  label: Mile Order API
  slug: mile-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-order-api-openapi.yml
- filename: mile-order-optimization-api-openapi.yml
  format: yaml
  label: Mile Order Optimization API
  slug: mile-order-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-order-optimization-api-openapi.yml
- filename: mile-order-webhook-api-openapi.yml
  format: yaml
  label: Mile Order Webhook API
  slug: mile-order-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-order-webhook-api-openapi.yml
- filename: mile-order-with-dynamic-merchant-api-openapi.yml
  format: yaml
  label: Mile Order With Dynamic Merchant API
  slug: mile-order-with-dynamic-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-order-with-dynamic-merchant-api-openapi.yml
- filename: mile-payment-terms-api-openapi.yml
  format: yaml
  label: Mile Payment Terms API
  slug: mile-payment-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-payment-terms-api-openapi.yml
- filename: mile-products-api-openapi.yml
  format: yaml
  label: Mile Products API
  slug: mile-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-products-api-openapi.yml
- filename: mile-promotion-bundle-api-openapi.yml
  format: yaml
  label: Mile Promotion Bundle API
  slug: mile-promotion-bundle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-promotion-bundle-api-openapi.yml
- filename: mile-routes-api-openapi.yml
  format: yaml
  label: Mile Routes API
  slug: mile-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-routes-api-openapi.yml
- filename: mile-settlement-webhook-api-openapi.yml
  format: yaml
  label: Mile Settlement Webhook API
  slug: mile-settlement-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-settlement-webhook-api-openapi.yml
- filename: mile-vehicles-api-openapi.yml
  format: yaml
  label: Mile Vehicles API
  slug: mile-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-vehicles-api-openapi.yml
- filename: mile-warehouse-inbound-orders-api-openapi.yml
  format: yaml
  label: Mile Warehouse Inbound Orders API
  slug: mile-warehouse-inbound-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-warehouse-inbound-orders-api-openapi.yml
- filename: mile-webhooks-api-openapi.yml
  format: yaml
  label: Mile Webhooks API
  slug: mile-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/openapi/mile-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: milenow.com
  spf: true
hosts:
- cert_expires: Sep 18 01:15:55 2026 GMT
  host: milenow.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 01:15:55 2026 GMT
  host: lastmile.milenow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mile, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Mile
provider_slug: mile
slug: mile-domain-security
source_filename: mile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: milenow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:15:55 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: lastmile.milenow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:15:55 2026 GMT\n  hsts: false\ndomains:\n- domain: milenow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mile/refs/heads/main/security/mile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Supply Chain
- Last Mile Delivery
- Order Management
- Warehouse Management
- Transportation Management
- Fulfillment
- Shipping
- Webhooks
- Route Optimization
---
