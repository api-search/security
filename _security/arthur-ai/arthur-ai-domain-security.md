---
api_specs:
- filename: arthur-ai-platform-openapi.json
  format: json
  label: Arthur Platform API
  slug: arthur-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-ai/refs/heads/main/openapi/arthur-ai-platform-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arthur.ai
  spf: true
hosts:
- cert_expires: Oct 15 19:54:24 2026 GMT
  host: www.arthur.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arthur Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arthur AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arthur AI
provider_slug: arthur-ai
slug: arthur-ai-domain-security
source_filename: arthur-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arthur.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:54:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arthur.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arthur-ai/refs/heads/main/security/arthur-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- AI Governance
- AI Observability
- Machine Learning
- LLM Evaluation
- Model Monitoring
- MLOps
- Guardrails
- Agents
---
