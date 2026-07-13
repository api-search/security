---
api_specs:
- filename: mem0-openapi.json
  format: json
  label: Mem0 Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/openapi/mem0-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mem0.ai
  spf: true
hosts:
- cert_expires: Oct  3 23:12:28 2026 GMT
  host: mem0.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:16:38 2026 GMT
  host: docs.mem0.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.mem0.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mem0 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mem0, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mem0
provider_slug: mem0
slug: mem0-domain-security
source_filename: mem0-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mem0.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:12:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mem0.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:16:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mem0.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mem0.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mem0/refs/heads/main/security/mem0-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Memory
- AI Agents
- Agent Memory
- Context
- LLMs
- Retrieval
- Vector
- LangChain
- CrewAI
- AutoGen
- LlamaIndex
- Open Source
- Infrastructure
---
