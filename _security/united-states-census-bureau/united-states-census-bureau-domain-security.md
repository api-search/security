---
api_specs:
- filename: census-data-api-openapi.yml
  format: yaml
  label: Census Data API
  slug: census-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-census-bureau/refs/heads/main/openapi/census-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: census.gov
  spf: true
hosts:
- cert_expires: Oct  2 23:56:12 2026 GMT
  host: www.census.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: api.census.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: tigerweb.geo.census.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: United States Census Bureau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United States Census Bureau, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: United States Census Bureau
provider_slug: united-states-census-bureau
slug: united-states-census-bureau-domain-security
source_filename: united-states-census-bureau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.census.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:56:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.census.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tigerweb.geo.census.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: census.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-census-bureau/refs/heads/main/security/united-states-census-bureau-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Demographics
- Federal Government
- Open Data
- Statistics
- Economics
- Population
---
