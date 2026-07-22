---
api_specs:
- filename: sageox-openapi-original.json
  format: json
  label: SageOx API
  slug: sageox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sageox/refs/heads/main/openapi/sageox-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sageox.ai
  spf: false
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: sageox.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: test.sageox.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sageox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SageOx, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: SageOx
provider_slug: sageox
slug: sageox-domain-security
source_filename: sageox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sageox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: test.sageox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sageox.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sageox/refs/heads/main/security/sageox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Developer Tools
- Knowledge Management
- Agent Memory
- Model Context Protocol
- MCP
- CLI
- Team Collaboration
- Agentic Engineering
---
