---
api_specs:
- filename: hanchu-ess-openapi-generated.yml
  format: yaml
  label: Hanchu ESS API
  slug: hanchu-ess-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hanchu-ess/openapi/_ae-authored/hanchu-ess-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hanchuess.com
  spf: true
hosts:
- cert_expires: Dec 20 15:11:51 2026 GMT
  host: hanchuess.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hanchu ESS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hanchu ESS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hanchu ESS
provider_slug: hanchu-ess
slug: hanchu-ess-domain-security
source_filename: hanchu-ess-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hanchuess.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 15:11:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hanchuess.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hanchu-ess/security/hanchu-ess-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Energy
- Storage
- Battery
- Renewables
- Smart Grid
---
