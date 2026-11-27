---
api_specs:
- filename: layerz-cc-openapi-generated.yml
  format: yaml
  label: Layerz API
  slug: layerz-cc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layerz-cc/openapi/_ae-authored/layerz-cc-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: layerz.cc
  spf: true
hosts:
- cert_expires: Feb  1 19:30:04 2027 GMT
  host: layerz.cc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Layerz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Layerz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Layerz
provider_slug: layerz-cc
slug: layerz-cc-domain-security
source_filename: layerz-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: layerz.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 19:30:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: layerz.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/layerz-cc/security/layerz-cc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Spreadsheets
- Artificial Intelligence
- CFO
- FP&A
---
