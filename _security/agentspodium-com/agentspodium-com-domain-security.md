---
api_specs:
- filename: agentspodium-com-openapi.yml
  format: yaml
  label: AgentsPodium Account API
  slug: account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentspodium-com/refs/heads/main/openapi/agentspodium-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentspodium.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: defispace.com
  spf: false
hosts:
- cert_expires: Nov 25 21:48:21 2026 GMT
  host: agentspodium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 10:03:53 2026 GMT
  host: hosting.defispace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 21:48:21 2026 GMT
  host: mcp.agentspodium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agentspodium Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentsPodium, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AgentsPodium
provider_slug: agentspodium-com
slug: agentspodium-com-domain-security
source_filename: agentspodium-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentspodium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 21:48:21 2026 GMT\n  hsts: false\n- host: hosting.defispace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 10:03:53 2026 GMT\n  hsts: false\n- host: mcp.agentspodium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 21:48:21 2026 GMT\n  hsts: false\ndomains:\n- domain: agentspodium.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: defispace.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentspodium-com/refs/heads/main/security/agentspodium-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Agents
- Agent Hosting
- MCP
- A2A
- Agent-Native
- Hosting
- Webhook
- Personal Assistants
- Company
---
