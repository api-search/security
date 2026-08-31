---
api_specs:
- filename: autogpt-external-api-openapi.json
  format: json
  label: AutoGPT External API
  slug: autogpt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autogpt/refs/heads/main/openapi/autogpt-external-api-openapi.json
- filename: autogpt-agent-server-openapi.json
  format: json
  label: AutoGPT Agent Server API
  slug: autogpt-agent-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autogpt/refs/heads/main/openapi/autogpt-agent-server-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: agpt.co
  spf: true
hosts:
- cert_expires: Oct 31 10:05:22 2026 GMT
  host: agpt.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 16:28:19 2026 GMT
  host: backend.agpt.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autogpt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoGPT, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: AutoGPT
provider_slug: autogpt
slug: autogpt-domain-security
source_filename: autogpt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agpt.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 10:05:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: backend.agpt.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 16:28:19 2026 GMT\n  hsts: null\ndomains:\n- domain: agpt.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autogpt/refs/heads/main/security/autogpt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- AI Automation
- Agent Platform
- Workflow-Automation
- MCP
- Open-Source
- No-Code
- LLM Orchestration
- Agent Marketplace
---
