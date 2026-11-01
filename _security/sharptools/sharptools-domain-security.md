---
api_specs:
- filename: sharptools-openapi-generated.yml
  format: yaml
  label: SharpTools API
  slug: sharptools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharptools/openapi/_ae-authored/sharptools-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sharptools.io
  spf: true
hosts:
- cert_expires: Dec  2 13:05:03 2026 GMT
  host: sharptools.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sharptools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SharpTools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SharpTools
provider_slug: sharptools
slug: sharptools-domain-security
source_filename: sharptools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sharptools.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 13:05:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: sharptools.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sharptools/security/sharptools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Smart Home
- Dashboards
- Automation
- Rule Engine
- Hub Integration
- Device Monitoring
- Custom Tiles
---
