---
api_specs:
- filename: hvacbuilder-app-openapi-generated.yml
  format: yaml
  label: HVAC Builder API
  slug: hvacbuilder-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hvacbuilder-app/openapi/_ae-authored/hvacbuilder-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hvacbuilder.app
  spf: true
hosts:
- cert_expires: Jan  9 08:46:46 2027 GMT
  host: hvacbuilder.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HVAC Builder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HVAC Builder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HVAC Builder
provider_slug: hvacbuilder-app
slug: hvacbuilder-app-domain-security
source_filename: hvacbuilder-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hvacbuilder.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 08:46:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hvacbuilder.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hvacbuilder-app/security/hvacbuilder-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HVAC
- Engineering
- Simulation
- Web App
- Free Tier
---
