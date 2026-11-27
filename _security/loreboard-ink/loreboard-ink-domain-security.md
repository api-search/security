---
api_specs:
- filename: loreboard-ink-data-api-openapi.yml
  format: yaml
  label: Loreboard Data API
  slug: loreboard-ink-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loreboard-ink/openapi/loreboard-ink-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: loreboard.ink
  spf: true
hosts:
- cert_expires: Jan 28 16:27:54 2027 GMT
  host: loreboard.ink
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Loreboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loreboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Loreboard
provider_slug: loreboard-ink
slug: loreboard-ink-domain-security
source_filename: loreboard-ink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loreboard.ink\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 16:27:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: loreboard.ink\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/loreboard-ink/security/loreboard-ink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Community
- Gaming
- Directory
- Lorcana
- Resources
---
