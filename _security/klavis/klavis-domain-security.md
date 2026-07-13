---
api_specs:
- filename: klavis-openapi.yml
  format: yaml
  label: Klavis MCP Platform API
  slug: mcp-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klavis/refs/heads/main/openapi/klavis-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: klavis.ai
  spf: true
hosts:
- cert_expires: Sep  3 19:05:06 2026 GMT
  host: www.klavis.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 18:45:50 2026 GMT
  host: api.klavis.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klavis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klavis AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Klavis AI
provider_slug: klavis
slug: klavis-domain-security
source_filename: klavis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klavis.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:05:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.klavis.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:45:50 2026 GMT\n  hsts: null\ndomains:\n- domain: klavis.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klavis/refs/heads/main/security/klavis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- MCP
- Model Context Protocol
- MCP Servers
- MCP Hosting
- Connectors
- OAuth
- Sandboxes
- Agent Training
- Reinforcement Learning
- White Label
- Open Source
- Strata
---
