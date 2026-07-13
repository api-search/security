---
api_specs:
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Subscriptions API
  slug: ordergroove-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Customers API
  slug: ordergroove-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Orders API
  slug: ordergroove-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Items API
  slug: ordergroove-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Products API
  slug: ordergroove-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Offers and Incentives API
  slug: ordergroove-offers-incentives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
- filename: ordergroove-openapi.yml
  format: yaml
  label: Ordergroove Webhooks API
  slug: ordergroove-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/openapi/ordergroove-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ordergroove.com
  spf: true
hosts:
- cert_expires: Sep 22 13:08:16 2026 GMT
  host: www.ordergroove.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 19:03:04 2026 GMT
  host: developer.ordergroove.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 13:22:17 2027 GMT
  host: restapi.ordergroove.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ordergroove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ordergroove, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ordergroove
provider_slug: ordergroove
slug: ordergroove-domain-security
source_filename: ordergroove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ordergroove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:08:16 2026 GMT\n  hsts: false\n- host: developer.ordergroove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:03:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: restapi.ordergroove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 13:22:17 2027 GMT\n  hsts: null\ndomains:\n- domain: ordergroove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordergroove/refs/heads/main/security/ordergroove-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Subscriptions
- Recurring Commerce
- Relationship Commerce
- eCommerce
- Autoship
- DTC
- Retail
- Subscription Management
---
