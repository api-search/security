---
api_specs:
- filename: housedata-uk-scoring-api-openapi.yml
  format: yaml
  label: HouseData.uk Scoring API
  slug: housedata-uk-scoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/housedata-uk/openapi/housedata-uk-scoring-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: housedata.uk
  spf: true
hosts:
- cert_expires: Jan  3 15:44:45 2027 GMT
  host: housedata.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HouseData.uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HouseData.uk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HouseData.uk
provider_slug: housedata-uk
slug: housedata-uk-domain-security
source_filename: housedata-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: housedata.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 15:44:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: housedata.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/housedata-uk/security/housedata-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Property
- Data
- United Kingdom
- Free
---
