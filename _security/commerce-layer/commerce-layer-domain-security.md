---
api_specs:
- filename: openapi.json
  format: json
  label: Commerce Layer Core API
  slug: commerce-layer-core-api
  spec_type: OpenAPI
  url: https://data.commercelayer.app/schemas/openapi.json
- filename: openapi.json
  format: json
  label: Commerce Layer Provisioning API
  slug: commerce-layer-provisioning-api
  spec_type: OpenAPI
  url: https://data.commercelayer.app/schemas/provisioning/openapi.json
- filename: openapi.json
  format: json
  label: Commerce Layer Metrics API
  slug: commerce-layer-metrics-api
  spec_type: OpenAPI
  url: https://data.commercelayer.app/schemas/metrics/openapi.json
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
  host: provisioning.commercelayer.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commerce Layer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commerce Layer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Commerce Layer
provider_slug: commerce-layer
slug: commerce-layer-domain-security
source_filename: commerce-layer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commercelayer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:43:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.commercelayer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:34:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: provisioning.commercelayer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 00:54:24 2026 GMT\n  hsts: null\ndomains:\n- domain: commercelayer.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commerce-layer/refs/heads/main/security/commerce-layer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Headless Commerce
- Composable Commerce
- API-First
- Ecommerce
- JSON:API
- OAuth 2.0
- Multi-Market
- Multi-Currency
- B2C
- B2B
- Subscriptions
- Promotions
- Inventory
- Order Management
- Checkout
---
