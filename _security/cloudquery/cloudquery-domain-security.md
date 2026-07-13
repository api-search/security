---
api_specs:
- filename: cloudquery-openapi.json
  format: json
  label: CloudQuery Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudquery/refs/heads/main/openapi/cloudquery-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cloudquery.io
  spf: true
hosts:
- cert_expires: Oct  7 17:22:38 2026 GMT
  host: www.cloudquery.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 03:18:23 2026 GMT
  host: platform-multi-tenant-api-docs.cloudquery.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 17:22:38 2026 GMT
  host: api.cloudquery.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudquery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudQuery, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CloudQuery
provider_slug: cloudquery
slug: cloudquery-domain-security
source_filename: cloudquery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudquery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:22:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform-multi-tenant-api-docs.cloudquery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 03:18:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cloudquery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:22:38 2026 GMT\n  hsts: null\ndomains:\n- domain: cloudquery.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudquery/refs/heads/main/security/cloudquery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Infrastructure
- Cloud Asset Inventory
- CSPM
- Cloud Governance
- FinOps
- Data Integration
- Platform Engineering
---
