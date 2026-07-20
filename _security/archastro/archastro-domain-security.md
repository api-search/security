---
api_specs:
- filename: archastro-platform-openapi.json
  format: json
  label: ArchAstro Platform API
  slug: archastro-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-platform-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: archastro.ai
  spf: false
hosts:
- cert_expires: Aug 27 07:50:12 2026 GMT
  host: archastro.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Archastro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archastro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Archastro
provider_slug: archastro
slug: archastro-domain-security
source_filename: archastro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: archastro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 07:50:12 2026 GMT\n  hsts: false\ndomains:\n- domain: archastro.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/security/archastro-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI Agents
- Agentic
- Developer Platform
- Automation
- Integration
- MCP
- Workflows
---
