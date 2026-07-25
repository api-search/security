---
api_specs:
- filename: commercelayer-addresses-api-openapi.yml
  format: yaml
  label: Commerce Layer Addresses API
  slug: commercelayer-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-addresses-api-openapi.yml
- filename: commercelayer-customers-api-openapi.yml
  format: yaml
  label: Commerce Layer Customers API
  slug: commercelayer-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-customers-api-openapi.yml
- filename: commercelayer-line-items-api-openapi.yml
  format: yaml
  label: Commerce Layer Line Items API
  slug: commercelayer-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-line-items-api-openapi.yml
- filename: commercelayer-markets-api-openapi.yml
  format: yaml
  label: Commerce Layer Markets API
  slug: commercelayer-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-markets-api-openapi.yml
- filename: commercelayer-orders-api-openapi.yml
  format: yaml
  label: Commerce Layer Orders API
  slug: commercelayer-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-orders-api-openapi.yml
- filename: commercelayer-payment-methods-api-openapi.yml
  format: yaml
  label: Commerce Layer Payment Methods API
  slug: commercelayer-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-payment-methods-api-openapi.yml
- filename: commercelayer-prices-api-openapi.yml
  format: yaml
  label: Commerce Layer Prices API
  slug: commercelayer-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-prices-api-openapi.yml
- filename: commercelayer-promotions-api-openapi.yml
  format: yaml
  label: Commerce Layer Promotions API
  slug: commercelayer-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-promotions-api-openapi.yml
- filename: commercelayer-shipments-api-openapi.yml
  format: yaml
  label: Commerce Layer Shipments API
  slug: commercelayer-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-shipments-api-openapi.yml
- filename: commercelayer-skus-api-openapi.yml
  format: yaml
  label: Commerce Layer SKUs API
  slug: commercelayer-skus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-skus-api-openapi.yml
- filename: commercelayer-stock-items-api-openapi.yml
  format: yaml
  label: Commerce Layer Stock Items API
  slug: commercelayer-stock-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-stock-items-api-openapi.yml
- filename: commercelayer-webhooks-api-openapi.yml
  format: yaml
  label: Commerce Layer Webhooks API
  slug: commercelayer-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: commercelayer.io
  spf: true
hosts:
- cert_expires: Aug 22 08:43:15 2026 GMT
  host: commercelayer.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 21:34:06 2026 GMT
  host: docs.commercelayer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 00:54:24 2026 GMT
  host: yourdomain.commercelayer.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commercelayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commerce Layer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Commerce Layer
provider_slug: commercelayer
slug: commercelayer-domain-security
source_filename: commercelayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commercelayer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:43:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.commercelayer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:34:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yourdomain.commercelayer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 00:54:24 2026 GMT\n  hsts: null\ndomains:\n- domain: commercelayer.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/security/commercelayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Commerce
- Headless
- Composable
- eCommerce
- JSON:API
- Orders
---
