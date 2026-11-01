---
api_specs:
- filename: birdieapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: birdieapi-com Basic lookup API
  slug: birdieapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-basic-lookup-api-openapi.yml
- filename: birdieapi-com-static-reference-api-openapi.yml
  format: yaml
  label: birdieapi-com Static reference API
  slug: birdieapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-static-reference-api-openapi.yml
- filename: birdieapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: birdieapi-com Stats + aggregation API
  slug: birdieapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-stats-aggregation-api-openapi.yml
- filename: birdieapi-com-time-series-api-openapi.yml
  format: yaml
  label: birdieapi-com Time Series API
  slug: birdieapi-com-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-time-series-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: birdieapi.com
  spf: true
hosts:
- cert_expires: Jan  6 13:33:48 2027 GMT
  host: birdieapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Birdieapi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for birdieapi-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: birdieapi-com
provider_slug: birdieapi-com
slug: birdieapi-com-domain-security
source_filename: birdieapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: birdieapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 13:33:48 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: birdieapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/birdieapi-com/security/birdieapi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Bird Tracking
- Migration Analytics
- Open Data
- Conservation
---
