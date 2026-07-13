---
api_specs:
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer SKUs, Prices & Stock API
  slug: skus-prices-stock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Orders & Line Items API
  slug: orders-line-items
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Customers & Addresses API
  slug: customers-addresses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Shipments API
  slug: shipments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Markets API
  slug: markets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Promotions API
  slug: promotions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
- filename: commercelayer-openapi.yml
  format: yaml
  label: Commerce Layer Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercelayer/refs/heads/main/openapi/commercelayer-openapi.yml
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
