---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: armature.tech
  spf: true
hosts:
- cert_expires: Oct  1 01:13:52 2026 GMT
  host: docs.armature.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 16:52:30 2026 GMT
  host: mcp.armature.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Armature Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armature, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Armature
provider_slug: armature
slug: armature-domain-security
source_filename: armature-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.armature.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:13:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp.armature.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:52:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: armature.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armature/refs/heads/main/security/armature-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agent Experience
- Model Context Protocol
- MCP
- Analytics
- Observability
- AI Agents
- Product Analytics
- Developer Tools
---
