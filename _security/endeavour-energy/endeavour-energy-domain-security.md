---
api_specs:
- filename: endeavour-energy-open-data-explore-api-v2-1-openapi.json
  format: json
  label: Endeavour Energy Open Data Explore API
  slug: endeavour-energy-open-data-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavour-energy/refs/heads/main/openapi/endeavour-energy-open-data-explore-api-v2-1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: endeavourenergy.com.au
  spf: true
hosts:
- cert_expires: Sep  4 11:51:30 2026 GMT
  host: www.endeavourenergy.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 06:13:44 2026 GMT
  host: data.endeavourenergy.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Endeavour Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endeavour Energy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Endeavour Energy
provider_slug: endeavour-energy
slug: endeavour-energy-domain-security
source_filename: endeavour-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.endeavourenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 11:51:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: data.endeavourenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:13:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: endeavourenergy.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endeavour-energy/refs/heads/main/security/endeavour-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Open Data
- Energy Networks
- Distribution
- Outages
- Consumer Data Right
- Smart Metering
- DER
- Solar
- Renewables
---
