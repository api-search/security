---
api_specs:
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Sales Orders API
  slug: fulfil-io-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Products & Variants API
  slug: fulfil-io-products-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Inventory & Stock API
  slug: fulfil-io-inventory-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Customers API
  slug: fulfil-io-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Shipments API
  slug: fulfil-io-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Purchases API
  slug: fulfil-io-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Manufacturing API
  slug: fulfil-io-manufacturing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Webhooks API
  slug: fulfil-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Model Interface API
  slug: fulfil-io-model-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fulfil.io
  spf: true
hosts:
- cert_expires: Sep  6 22:47:38 2026 GMT
  host: www.fulfil.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 22:47:38 2026 GMT
  host: developers.fulfil.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 19:39:20 2026 GMT
  host: docs.fulfil.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fulfil Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fulfil, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fulfil
provider_slug: fulfil-io
slug: fulfil-io-domain-security
source_filename: fulfil-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fulfil.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:47:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.fulfil.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:47:38 2026 GMT\n  hsts: false\n- host: docs.fulfil.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 19:39:20 2026 GMT\n  hsts: false\ndomains:\n- domain: fulfil.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/security/fulfil-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ERP
- E-commerce
- Order Management
- Inventory
- Warehouse Management
- Manufacturing
- Operations
---
