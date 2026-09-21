---
api_specs:
- filename: afmr-ai-discovery-api-openapi.yml
  format: yaml
  label: AFMR Discovery API
  slug: afmr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-discovery-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: afmr.ai
  spf: true
hosts:
- cert_expires: Oct 28 17:13:34 2026 GMT
  host: afmr.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Afmr Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Failure Mode Registry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agent Failure Mode Registry
provider_slug: afmr-ai
slug: afmr-ai-domain-security
source_filename: afmr-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: afmr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 17:13:34 2026 GMT\n  hsts: false\ndomains:\n- domain: afmr.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/security/afmr-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI Agents
- Agent Governance
- Standards
- Reputation
- Failure Modes
- Discovery
- MCP
- A2A
- Machine-Readable Standards
---
