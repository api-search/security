---
api_specs:
- filename: rowguard-csv-validation-api-openapi.yml
  format: yaml
  label: RowGuard API Catalog CSV validation API
  slug: rowguard-csv-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rowguard/refs/heads/main/openapi/rowguard-csv-validation-api-openapi.yml
- filename: rowguard-example-api-openapi.yml
  format: yaml
  label: RowGuard API Catalog Example API
  slug: rowguard-example-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rowguard/refs/heads/main/openapi/rowguard-example-api-openapi.yml
- filename: rowguard-healthz-api-openapi.yml
  format: yaml
  label: RowGuard API Catalog Healthz API
  slug: rowguard-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rowguard/refs/heads/main/openapi/rowguard-healthz-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Dec  8 02:36:23 2026 GMT
  host: rowguard-api.rowguard-api.workers.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rowguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RowGuard API Catalog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RowGuard API Catalog
provider_slug: rowguard
slug: rowguard-domain-security
source_filename: rowguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rowguard-api.rowguard-api.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 02:36:23 2026 GMT\n  hsts: null\ndomains:\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rowguard/refs/heads/main/security/rowguard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CSV
- Validation
- Data Quality
- Import
- Automation
---
