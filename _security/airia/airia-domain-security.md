---
api_specs:
- filename: airia-openapi.yml
  format: yaml
  label: Airia Web APIs
  slug: airia-web-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airia/refs/heads/main/openapi/airia-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airia.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airia.ai
  spf: true
hosts:
- cert_expires: Dec  7 02:44:47 2026 GMT
  host: airia.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 20:01:03 2026 GMT
  host: api.airia.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 18:43:57 2026 GMT
  host: airia.ai
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Airia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Airia
provider_slug: airia
slug: airia-domain-security
source_filename: airia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 02:44:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: api.airia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 20:01:03 2026 GMT\n  hsts: null\n- host: airia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 18:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: airia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: airia.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airia/refs/heads/main/security/airia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise AI
- AI Agents
- AI Governance
- AI Security
- MCP
- MCP Gateway
- Agent Orchestration
- LLM Gateway
- AI Discovery
- Red Teaming
- Guardrails
- Knowledge Retrieval
- RAG
- agent-native
---
