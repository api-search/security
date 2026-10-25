---
api_specs:
- filename: australian-bureau-of-statistics-get-data-api-openapi.yml
  format: yaml
  label: Australian Bureau of Statistics Get Data API
  slug: australian-bureau-of-statistics-get-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-bureau-of-statistics/refs/heads/main/openapi/australian-bureau-of-statistics-get-data-api-openapi.yml
- filename: australian-bureau-of-statistics-get-metadata-api-openapi.yml
  format: yaml
  label: Australian Bureau of Statistics Get Metadata API
  slug: australian-bureau-of-statistics-get-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-bureau-of-statistics/refs/heads/main/openapi/australian-bureau-of-statistics-get-metadata-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abs.gov.au
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: www.abs.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Australian Bureau Of Statistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Bureau of Statistics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Australian Bureau of Statistics
provider_slug: australian-bureau-of-statistics
slug: australian-bureau-of-statistics-domain-security
source_filename: australian-bureau-of-statistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abs.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abs.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-bureau-of-statistics/refs/heads/main/security/australian-bureau-of-statistics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- Statistics
- Open Data
- SDMX
- Census
- Economic Indicators
- Australia
---
