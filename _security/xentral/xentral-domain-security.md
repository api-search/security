---
api_specs:
- filename: xentral-api-openapi-original.json
  format: json
  label: Xentral API
  slug: xentral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xentral/refs/heads/main/openapi/xentral-api-openapi-original.json
- filename: xentral-documents-api-openapi-original.json
  format: json
  label: Xentral Business Documents API v3
  slug: xentral-business-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xentral/refs/heads/main/openapi/xentral-documents-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xentral.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: xentral.biz
  spf: false
hosts:
- cert_expires: Sep  9 04:40:48 2026 GMT
  host: developer.xentral.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: xentral.xentral.biz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xentral Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xentral, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xentral
provider_slug: xentral
slug: xentral-domain-security
source_filename: xentral-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.xentral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 04:40:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: xentral.xentral.biz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: xentral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: xentral.biz\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xentral/refs/heads/main/security/xentral-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- ERP
- eCommerce
- Fulfillment
- Warehousing
- Invoicing
- Accounting
- Orders
- Products
- Germany
---
