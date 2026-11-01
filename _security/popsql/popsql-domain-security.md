---
api_specs:
- filename: popsql-data-catalog-api-openapi.yml
  format: yaml
  label: PopSQL Data Catalog API
  slug: popsql-data-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/popsql/openapi/popsql-data-catalog-api-openapi.yml
- filename: popsql-query-runs-api-openapi.yml
  format: yaml
  label: PopSQL Query Runs API
  slug: popsql-query-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/popsql/openapi/popsql-query-runs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: popsql.com
  spf: true
hosts:
- cert_expires: Nov 26 19:02:20 2026 GMT
  host: popsql.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Popsql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PopSQL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PopSQL
provider_slug: popsql
slug: popsql-domain-security
source_filename: popsql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: popsql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 19:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: popsql.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/popsql/security/popsql-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SQL
- Collaboration
- Data-Analytics
- Cloud
---
