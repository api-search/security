---
api_specs:
- filename: framethrower-openapi.yml
  format: yaml
  label: FrameThrower API
  slug: framethrower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/openapi/framethrower-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: framethrower.ai
  spf: true
hosts:
- cert_expires: Dec  8 01:48:19 2026 GMT
  host: framethrower.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Framethrower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FrameThrower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FrameThrower
provider_slug: framethrower
slug: framethrower-domain-security
source_filename: framethrower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: framethrower.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 01:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: framethrower.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/security/framethrower-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Film
- Cinematography
- Visual Reference
- Image Search
- Media
- Creative Tools
- MCP
- Agent-Native
---
