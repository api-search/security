---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mcpjunction.ai
  spf: true
hosts:
- cert_expires: Jan  9 14:33:19 2027 GMT
  host: mcpjunction.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCP Junction Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCP Junction, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MCP Junction
provider_slug: mcpjunction-ai
slug: mcpjunction-ai-domain-security
source_filename: mcpjunction-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpjunction.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 14:33:19 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mcpjunction.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mcpjunction-ai/security/mcpjunction-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Directory
- MCP
- Servers
- Datasets
---
