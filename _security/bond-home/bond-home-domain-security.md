---
api_specs:
- filename: bond-home-openapi-generated.yml
  format: yaml
  label: Bond (fan / shade bridge) API
  slug: bond-home-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bond-home/openapi/_ae-authored/bond-home-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bondhome.io
  spf: true
hosts:
- cert_expires: Dec  9 06:33:58 2026 GMT
  host: bondhome.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bond Home Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bond (fan / shade bridge), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bond (fan / shade bridge)
provider_slug: bond-home
slug: bond-home-domain-security
source_filename: bond-home-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bondhome.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 06:33:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bondhome.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bond-home/security/bond-home-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SmartHome
- IoT
- HomeAutomation
- Connectivity
---
