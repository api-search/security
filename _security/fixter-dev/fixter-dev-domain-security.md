---
api_specs:
- filename: fixter-dev-openapi-generated.yml
  format: yaml
  label: Fixter API
  slug: fixter-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixter-dev/openapi/_ae-authored/fixter-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fixter.dev
  spf: true
hosts:
- cert_expires: Jan 25 03:33:47 2027 GMT
  host: fixter.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fixter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fixter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fixter
provider_slug: fixter-dev
slug: fixter-dev-domain-security
source_filename: fixter-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixter.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 03:33:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fixter.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fixter-dev/security/fixter-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Artificial Intelligence
- APM
- Error Tracking
- MCP
---
