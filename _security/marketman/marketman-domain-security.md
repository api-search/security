---
api_specs:
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Inventory & Items API
  slug: inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Vendors API
  slug: vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Purchase Orders API
  slug: purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Invoices & Docs API
  slug: invoices-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Deliveries API
  slug: deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Recipes & Menu Profitability API
  slug: recipes-menu-profitability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
- filename: marketman-openapi.yml
  format: yaml
  label: MarketMan Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/openapi/marketman-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marketman.com
  spf: true
hosts:
- cert_expires: Aug 12 09:42:19 2026 GMT
  host: www.marketman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 12:02:21 2026 GMT
  host: api-doc.marketman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 12:02:21 2026 GMT
  host: api.marketman.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marketman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarketMan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MarketMan
provider_slug: marketman
slug: marketman-domain-security
source_filename: marketman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marketman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 09:42:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-doc.marketman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:02:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.marketman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:02:21 2026 GMT\n  hsts: false\ndomains:\n- domain: marketman.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketman/refs/heads/main/security/marketman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Inventory
- Purchasing
- Supply Chain
- Food Service
---
