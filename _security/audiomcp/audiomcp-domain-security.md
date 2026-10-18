---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audiomcp.ai
  spf: true
hosts:
- cert_expires: Jan 10 10:26:20 2027 GMT
  host: audiomcp.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audiomcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for op.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: op.ai
provider_slug: audiomcp
slug: audiomcp-domain-security
source_filename: audiomcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audiomcp.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 10:26:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: audiomcp.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audiomcp/refs/heads/main/security/audiomcp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Voice
- Conversational AI
- Platform
- MCP
---
