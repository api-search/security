---
api_specs:
- filename: galileo-ai-openapi.yml
  format: yaml
  label: Galileo Public API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/openapi/galileo-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: galileo.ai
  spf: true
hosts:
- cert_expires: Sep 25 15:02:15 2026 GMT
  host: galileo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 12:52:22 2026 GMT
  host: docs.galileo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 11:42:58 2026 GMT
  host: api.galileo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Galileo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galileo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Galileo
provider_slug: galileo-ai
slug: galileo-ai-domain-security
source_filename: galileo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: galileo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:02:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.galileo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:52:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.galileo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:42:58 2026 GMT\n  hsts: null\ndomains:\n- domain: galileo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/security/galileo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Evaluation
- AI Observability
- GenAI
- Guardrails
- Agentic AI
- LLM
- Tracing
- Experiments
- Prompts
- Datasets
---
