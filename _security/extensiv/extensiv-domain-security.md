---
api_specs:
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Orders API
  slug: extensiv-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Inventory API
  slug: extensiv-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Items API
  slug: extensiv-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Customers API
  slug: extensiv-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Receivers (ASN) API
  slug: extensiv-receivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Warehouses API
  slug: extensiv-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
- filename: extensiv-openapi.yml
  format: yaml
  label: Extensiv Auth Token API
  slug: extensiv-auth-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/openapi/extensiv-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: extensiv.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: secure-wms.com
  spf: true
hosts:
- cert_expires: Sep 28 13:32:32 2026 GMT
  host: www.extensiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: developer.extensiv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: secure-wms.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Extensiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extensiv, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Extensiv
provider_slug: extensiv
slug: extensiv-domain-security
source_filename: extensiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.extensiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:32:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.extensiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: false\n- host: secure-wms.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: extensiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: secure-wms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/security/extensiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- 3PL
- Warehouse Management
- WMS
- Order Management
- Inventory Management
- Fulfillment
- Logistics
- Supply Chain
---
