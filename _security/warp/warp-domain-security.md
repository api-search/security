---
api_specs:
- filename: warp-oz-agent-api-openapi.yml
  format: yaml
  label: Warp Oz Agent API
  slug: oz-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warp/refs/heads/main/openapi/warp-oz-agent-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: warp.dev
  spf: true
hosts:
- cert_expires: Sep  9 07:36:59 2026 GMT
  host: www.warp.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:32:26 2026 GMT
  host: docs.warp.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 15:29:25 2026 GMT
  host: app.warp.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Warp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Warp
provider_slug: warp
slug: warp-domain-security
source_filename: warp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.warp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:36:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.warp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:32:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.warp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 15:29:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: warp.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warp/refs/heads/main/security/warp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Terminal
- AI Agents
- Cloud Agents
- Agentic Development
---
