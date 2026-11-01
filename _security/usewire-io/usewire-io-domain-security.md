---
api_specs:
- filename: usewire-io-openapi-generated.yml
  format: yaml
  label: usewire-io API
  slug: usewire-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewire-io/openapi/_ae-authored/usewire-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usewire.io
  spf: true
hosts:
- cert_expires: Jan 23 02:04:22 2027 GMT
  host: usewire.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usewire Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for usewire-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: usewire-io
provider_slug: usewire-io
slug: usewire-io-domain-security
source_filename: usewire-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usewire.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 02:04:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usewire.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/usewire-io/security/usewire-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- MCP
- Collaboration
- Context
- Platform
---
