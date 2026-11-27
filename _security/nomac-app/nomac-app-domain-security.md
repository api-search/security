---
api_specs:
- filename: nomac-app-openapi-generated.yml
  format: yaml
  label: NoMac API
  slug: nomac-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomac-app/openapi/_ae-authored/nomac-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nomac.app
  spf: true
hosts:
- cert_expires: Feb 11 01:37:37 2027 GMT
  host: nomac.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NoMac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NoMac, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NoMac
provider_slug: nomac-app
slug: nomac-app-domain-security
source_filename: nomac-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nomac.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 01:37:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nomac.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nomac-app/security/nomac-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- macOS
- Artificial Intelligence
- CI
- On-Demand
---
