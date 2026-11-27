---
api_specs:
- filename: ironledger-app-tools-api-openapi.yml
  format: yaml
  label: IronLedger Tools API
  slug: ironledger-app-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ironledger-app/openapi/ironledger-app-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ironledger.app
  spf: false
hosts:
- cert_expires: Dec 27 16:01:00 2026 GMT
  host: ironledger.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IronLedger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IronLedger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: IronLedger
provider_slug: ironledger-app
slug: ironledger-app-domain-security
source_filename: ironledger-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ironledger.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 16:01:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ironledger.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ironledger-app/security/ironledger-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fitness
- Health
- Workouts
- Strength Training
- FreeApp
- Company
---
