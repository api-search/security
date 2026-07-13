---
api_specs:
- filename: orderdesk-openapi.yml
  format: yaml
  label: Order Desk Orders API
  slug: orderdesk-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/openapi/orderdesk-openapi.yml
- filename: orderdesk-openapi.yml
  format: yaml
  label: Order Desk Order Items API
  slug: orderdesk-order-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/openapi/orderdesk-openapi.yml
- filename: orderdesk-openapi.yml
  format: yaml
  label: Order Desk Shipments API
  slug: orderdesk-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/openapi/orderdesk-openapi.yml
- filename: orderdesk-openapi.yml
  format: yaml
  label: Order Desk Inventory Items API
  slug: orderdesk-inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/openapi/orderdesk-openapi.yml
- filename: orderdesk-openapi.yml
  format: yaml
  label: Order Desk Store API
  slug: orderdesk-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/openapi/orderdesk-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orderdesk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orderdesk.me
  spf: true
hosts:
- cert_expires: Sep 28 04:16:56 2026 GMT
  host: www.orderdesk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 04:16:44 2026 GMT
  host: apidocs.orderdesk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: app.orderdesk.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orderdesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Order Desk, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Order Desk
provider_slug: orderdesk
slug: orderdesk-domain-security
source_filename: orderdesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orderdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:16:56 2026 GMT\n  hsts: false\n- host: apidocs.orderdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:16:44 2026 GMT\n  hsts: false\n- host: app.orderdesk.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: orderdesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: orderdesk.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderdesk/refs/heads/main/security/orderdesk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Ecommerce
- Order Management
- Fulfillment
- Dropshipping
- Inventory
- Shipping
---
