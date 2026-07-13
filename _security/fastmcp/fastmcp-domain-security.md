---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gofastmcp.com
  spf: false
hosts:
- cert_expires: Sep 20 08:39:15 2026 GMT
  host: gofastmcp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fastmcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FastMCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: FastMCP
provider_slug: fastmcp
slug: fastmcp-domain-security
source_filename: fastmcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gofastmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:39:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gofastmcp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastmcp/refs/heads/main/security/fastmcp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- MCP
- Model Context Protocol
- Python
- Framework
- Open Source
- AI Agents
- Tools
- Resources
- Prompts
- LLMs
- Anthropic
---
