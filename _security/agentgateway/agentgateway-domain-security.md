---
api_specs:
- filename: agentgateway-openapi.yml
  format: yaml
  label: AgentGateway
  slug: agentgateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/openapi/agentgateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentgateway.dev
  spf: false
hosts:
- cert_expires: Sep  9 19:32:36 2026 GMT
  host: agentgateway.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Agentgateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentGateway, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AgentGateway
provider_slug: agentgateway
slug: agentgateway-domain-security
source_filename: agentgateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentgateway.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 19:32:36 2026 GMT\n  hsts: false\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: agentgateway.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/security/agentgateway-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Gateway
- API Gateway
- MCP
- LLM
- Agent-to-Agent
- Open Source
- CNCF
- Observability
- Security
---
