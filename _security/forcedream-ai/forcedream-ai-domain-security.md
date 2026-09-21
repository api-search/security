---
api_specs:
- filename: forcedream-ai-openapi.yml
  format: yaml
  label: ForceDream API
  slug: forcedream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forcedream-ai/refs/heads/main/openapi/forcedream-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: forcedream.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forcedream.com
  spf: true
hosts:
- cert_expires: Dec 10 15:18:48 2026 GMT
  host: forcedream.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 22:52:11 2026 GMT
  host: www.forcedream.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 21:44:20 2026 GMT
  host: api.forcedream.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Forcedream Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ForceDream, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ForceDream
provider_slug: forcedream-ai
slug: forcedream-ai-domain-security
source_filename: forcedream-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forcedream.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 15:18:48 2026 GMT\n  hsts: false\n- host: www.forcedream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 22:52:11 2026 GMT\n  hsts: false\n- host: api.forcedream.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 21:44:20 2026 GMT\n  hsts: false\ndomains:\n- domain: forcedream.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: forcedream.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forcedream-ai/refs/heads/main/security/forcedream-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Agents
- Agent Marketplace
- MCP
- A2A
- Cryptographic Proofs
- AI Inference Routing
- Agent Payments
- Agentic Commerce
- agent-native
- United Kingdom
---
