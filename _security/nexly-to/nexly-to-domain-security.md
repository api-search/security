---
api_specs:
- filename: nexly-to-openapi-generated.yml
  format: yaml
  label: Nexly Analytics API
  slug: nexly-to-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexly-to/openapi/_ae-authored/nexly-to-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nexly.to
  spf: true
hosts:
- cert_expires: Jan 16 01:04:29 2027 GMT
  host: nexly.to
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nexly Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexly Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nexly Analytics
provider_slug: nexly-to
slug: nexly-to-domain-security
source_filename: nexly-to-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexly.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 01:04:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nexly.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nexly-to/security/nexly-to-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Artificial Intelligence
- Traffic
- Product
- Insights
---
