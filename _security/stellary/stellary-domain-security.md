---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: stellary.co
  spf: true
hosts:
- cert_expires: Nov  8 07:41:48 2026 GMT
  host: stellary.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 11:36:58 2026 GMT
  host: api.stellary.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stellary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stellary, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Stellary
provider_slug: stellary
slug: stellary-domain-security
source_filename: stellary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stellary.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 07:41:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stellary.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:36:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stellary.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellary/refs/heads/main/security/stellary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- project-management
- productivity
- AI-agents
- agent-orchestration
- MCP
- remote-mcp
- developer-tools
- SaaS
- collaboration
---
