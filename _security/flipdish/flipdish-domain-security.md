---
api_specs:
- filename: flipdish-apps-openapi.json
  format: json
  label: Flipdish Apps & Channels API
  slug: apps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-apps-openapi.json
- filename: flipdish-catalog-openapi.json
  format: json
  label: Flipdish Catalog API
  slug: catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-catalog-openapi.json
- filename: flipdish-customers-openapi.json
  format: json
  label: Flipdish Customers & Accounts API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-customers-openapi.json
- filename: flipdish-devices-openapi.json
  format: json
  label: Flipdish Devices API
  slug: devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-devices-openapi.json
- filename: flipdish-marketing-openapi.json
  format: json
  label: Flipdish Marketing API
  slug: marketing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-marketing-openapi.json
- filename: flipdish-menus-openapi.json
  format: json
  label: Flipdish Menus API
  slug: menus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-menus-openapi.json
- filename: flipdish-orders-openapi.json
  format: json
  label: Flipdish Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-orders-openapi.json
- filename: flipdish-payments-openapi.json
  format: json
  label: Flipdish Payments & Payouts API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-payments-openapi.json
- filename: flipdish-platform-openapi.json
  format: json
  label: Flipdish Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-platform-openapi.json
- filename: flipdish-stores-openapi.json
  format: json
  label: Flipdish Stores API
  slug: stores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/openapi/flipdish-stores-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flipdish.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: flipdish.co
  spf: true
hosts:
- cert_expires: Sep 11 00:07:51 2026 GMT
  host: www.flipdish.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:42:22 2026 GMT
  host: developers.flipdish.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 11:55:14 2026 GMT
  host: api.flipdish.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flipdish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flipdish, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flipdish
provider_slug: flipdish
slug: flipdish-domain-security
source_filename: flipdish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flipdish.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 00:07:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.flipdish.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:42:22 2026 GMT\n  hsts: null\n- host: api.flipdish.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 11:55:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flipdish.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: flipdish.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipdish/refs/heads/main/security/flipdish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Online Ordering
- Mobile Apps
- Point of Sale
- Orders
- Menu
- Payments
- Webhooks
---
