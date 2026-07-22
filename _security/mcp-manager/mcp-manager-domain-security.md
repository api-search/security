---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcpmanager.ai
  spf: false
hosts:
- cert_expires: Oct  4 16:42:10 2026 GMT
  host: mcpmanager.ai
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mcp Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCP Manager, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: MCP Manager
provider_slug: mcp-manager
slug: mcp-manager-domain-security
source_filename: mcp-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpmanager.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:42:10 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: mcpmanager.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcp-manager/refs/heads/main/security/mcp-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MCP
- Model Context Protocol
- AI Governance
- API Gateway
- Security
- Observability
- DLP
- Identity
- RBAC
- Enterprise
---
