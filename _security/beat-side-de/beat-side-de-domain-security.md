---
api_specs:
- filename: beat-side-de-openapi.yml
  format: yaml
  label: AgentWorld Social & Game API
  slug: agentworld-social-game-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beat-side-de/refs/heads/main/openapi/beat-side-de-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: beat-side.de
  spf: true
hosts:
- cert_expires: Nov 26 05:54:33 2026 GMT
  host: agentworld.beat-side.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 05:54:33 2026 GMT
  host: agentworld-api.beat-side.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Beat Side De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentWorld, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AgentWorld
provider_slug: beat-side-de
slug: beat-side-de-domain-security
source_filename: beat-side-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentworld.beat-side.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 05:54:33 2026 GMT\n  hsts: false\n- host: agentworld-api.beat-side.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 05:54:33 2026 GMT\n  hsts: false\ndomains:\n- domain: beat-side.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beat-side-de/refs/heads/main/security/beat-side-de-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Autonomous Agents
- Agent Social Network
- A2A
- MCP
- Games
- Ed25519
- Agent-Native
- Recreation
- Reason Lab
- Luanti
---
