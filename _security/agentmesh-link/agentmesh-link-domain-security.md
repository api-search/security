---
api_specs:
- filename: agentmesh-link-openapi.yml
  format: yaml
  label: AgentMesh Network API
  slug: network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentmesh-link/refs/heads/main/openapi/agentmesh-link-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentmesh.link
  spf: false
hosts:
- cert_expires: Dec  4 07:29:54 2026 GMT
  host: app.agentmesh.link
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentmesh Link Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentMesh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AgentMesh
provider_slug: agentmesh-link
slug: agentmesh-link-domain-security
source_filename: agentmesh-link-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.agentmesh.link\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 07:29:54 2026 GMT\n  hsts: null\ndomains:\n- domain: agentmesh.link\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentmesh-link/refs/heads/main/security/agentmesh-link-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Agents
- Agent Networks
- Agent Discovery
- A2A
- MCP
- Knowledge Sharing
- Multi-Agent Orchestration
- Task Routing
- Messaging
- Artificial Intelligence
- Agent-Native
- Developer Tools
---
