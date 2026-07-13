---
api_specs:
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Orders API
  slug: 3plcentral-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Items API
  slug: 3plcentral-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Inventory API
  slug: 3plcentral-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Stock Summaries API
  slug: 3plcentral-stock-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Receivers (ASN) API
  slug: 3plcentral-receivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Customers API
  slug: 3plcentral-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Warehouses API
  slug: 3plcentral-warehouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
- filename: 3plcentral-openapi.yml
  format: yaml
  label: 3PL Warehouse Manager Packages API
  slug: 3plcentral-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/openapi/3plcentral-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: extensiv.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 3plcentral.com
  spf: true
hosts:
- cert_expires: Sep 28 13:32:32 2026 GMT
  host: www.extensiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 00:05:59 2026 GMT
  host: developer.3plcentral.com
  hsts: true
  hsts_max_age: 31536000
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
name: 3Plcentral Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3PL Warehouse Manager, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 3PL Warehouse Manager
provider_slug: 3plcentral
slug: 3plcentral-domain-security
source_filename: 3plcentral-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.extensiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:32:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.3plcentral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:05:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: secure-wms.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: extensiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: 3plcentral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3plcentral/refs/heads/main/security/3plcentral-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Warehouse Management
- WMS
- 3PL
- Logistics
- Fulfillment
- Inventory
- Orders
- SecureWMS
- Extensiv
---
