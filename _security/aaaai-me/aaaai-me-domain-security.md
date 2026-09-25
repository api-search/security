---
api_specs:
- filename: aaaai-me-openapi.json
  format: json
  label: AAAAI Platform API
  slug: aaaai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/openapi/aaaai-me-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aaaai.me
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: aaaai.me
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: web.aaaai.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aaaai Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AAA AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AAA AI
provider_slug: aaaai-me
slug: aaaai-me-domain-security
source_filename: aaaai-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aaaai.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\n- host: web.aaaai.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aaaai.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaaai-me/refs/heads/main/security/aaaai-me-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Agents
- Multi-Agent
- LLM Orchestration
- Meetings
- Voice
- Video
- Workflows
- MCP
- Agentic Commerce
- OpenAI-Compatible
- Self-Hosted
- Agent-Native
- Montenegro
---
