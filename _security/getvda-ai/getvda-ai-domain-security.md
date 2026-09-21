---
api_specs:
- filename: getvda-ai-witness-openapi.json
  format: json
  label: VDA Witness API
  slug: vda-witness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-witness-openapi.json
- filename: getvda-ai-hitl-openapi.json
  format: json
  label: VDA HITL API
  slug: vda-hitl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-hitl-openapi.json
- filename: getvda-ai-acp-openapi.json
  format: json
  label: VDA ACP API
  slug: vda-acp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-acp-openapi.json
- filename: getvda-ai-c2md-edge-openapi.json
  format: json
  label: C2MD Compliance Agent
  slug: c2md-compliance-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-c2md-edge-openapi.json
- filename: getvda-ai-gosce-router-openapi.json
  format: json
  label: GOSCE Agent Portfolio and Router
  slug: gosce-agent-portfolio-and-router
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-gosce-router-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getvda.ai
  spf: true
hosts:
- cert_expires: Dec 10 10:28:08 2026 GMT
  host: getvda.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 20:40:00 2026 GMT
  host: witness.getvda.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 16:21:55 2026 GMT
  host: hitl.getvda.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Getvda Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verified Digital Agents (VDA), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Verified Digital Agents (VDA)
provider_slug: getvda-ai
slug: getvda-ai-domain-security
source_filename: getvda-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getvda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 10:28:08 2026 GMT\n  hsts: false\n- host: witness.getvda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 20:40:00 2026 GMT\n  hsts: false\n- host: hitl.getvda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 16:21:55 2026 GMT\n  hsts: null\ndomains:\n- domain: getvda.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/security/getvda-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Agents
- AI Governance
- Compliance
- Audit Trail
- Agent Identity
- A2A
- MCP
- x402
- EU AI Act
- Human-in-the-Loop
---
