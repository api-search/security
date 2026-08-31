---
api_specs:
- filename: nutrientsdb-foods-api-openapi.yml
  format: yaml
  label: NutrientsDB Foods API
  slug: nutrientsdb-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutrientsdb/refs/heads/main/openapi/nutrientsdb-foods-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nutrientsdb.com
  spf: false
hosts:
- cert_expires: Nov  5 00:28:08 2026 GMT
  host: www.nutrientsdb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nutrientsdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NutrientsDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: NutrientsDB
provider_slug: nutrientsdb
slug: nutrientsdb-domain-security
source_filename: nutrientsdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nutrientsdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 00:28:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nutrientsdb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutrientsdb/refs/heads/main/security/nutrientsdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- nutrition
- food
- nutrients
- food-composition
- Data
- Search
- sample-data
- Dataset
- ai-builders
- reference-data
- Open Data
- keyless-api
---
