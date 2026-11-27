---
api_specs:
- filename: bim-house-openapi-generated.yml
  format: yaml
  label: BIM.HOUSE API
  slug: bim-house-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bim-house/openapi/_ae-authored/bim-house-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bim.house
  spf: true
hosts:
- cert_expires: Dec  3 19:08:10 2026 GMT
  host: bim.house
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BIM.HOUSE Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BIM.HOUSE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BIM.HOUSE
provider_slug: bim-house
slug: bim-house-domain-security
source_filename: bim-house-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bim.house\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 19:08:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bim.house\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bim-house/security/bim-house-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- BIM
- Architecture
- Construction
- Artificial Intelligence
---
