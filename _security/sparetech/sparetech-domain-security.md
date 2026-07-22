---
api_specs:
- filename: sparetech-sync-v1-openapi.json
  format: json
  label: Sparetech Sync API v1
  slug: sparetech-sync-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparetech/refs/heads/main/openapi/sparetech-sync-v1-openapi.json
- filename: sparetech-sync-v2-openapi.json
  format: json
  label: Sparetech Sync API v2 (SAP)
  slug: sparetech-sync-api-v2-sap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparetech/refs/heads/main/openapi/sparetech-sync-v2-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sparetech.io
  spf: true
hosts:
- cert_expires: Oct 11 22:29:57 2026 GMT
  host: www.sparetech.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: sync.sparetech.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: sync.sandbox.sparetech.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sparetech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sparetech, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sparetech
provider_slug: sparetech
slug: sparetech-domain-security
source_filename: sparetech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sparetech.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 22:29:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sync.sparetech.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\n- host: sync.sandbox.sparetech.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sparetech.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparetech/refs/heads/main/security/sparetech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- Spare Parts
- MRO
- Maintenance
- Procurement
- Inventory Optimization
- ERP Integration
- SAP
- Master Data Management
---
