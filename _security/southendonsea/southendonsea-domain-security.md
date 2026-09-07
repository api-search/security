---
api_specs:
- filename: southendonsea-southend-now-api-openapi.yml
  format: yaml
  label: SouthendOnSea.city Southend Now API
  slug: southendonsea-southend-now-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/southendonsea/refs/heads/main/openapi/southendonsea-southend-now-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: southendonsea.city
  spf: true
hosts:
- cert_expires: Nov  2 20:55:18 2026 GMT
  host: southendonsea.city
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Southendonsea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SouthendOnSea.city, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SouthendOnSea.city
provider_slug: southendonsea
slug: southendonsea-domain-security
source_filename: southendonsea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: southendonsea.city\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 20:55:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: southendonsea.city\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/southendonsea/refs/heads/main/security/southendonsea-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- Southend-on-Sea
- Weather
- Environment
- local data
---
