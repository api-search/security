---
api_specs:
- filename: arthur-scope-openapi.json
  format: json
  label: Arthur Scope
  slug: arthur-scope
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthurai/refs/heads/main/openapi/arthur-scope-openapi.json
- filename: arthur-engine-openapi.json
  format: json
  label: Arthur GenAI Engine
  slug: arthur-genai-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthurai/refs/heads/main/openapi/arthur-engine-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arthur.ai
  spf: true
hosts:
- cert_expires: Oct 15 19:50:45 2026 GMT
  host: arthur.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arthurai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ArthurAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ArthurAI
provider_slug: arthurai
slug: arthurai-domain-security
source_filename: arthurai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arthur.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:50:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arthur.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arthurai/refs/heads/main/security/arthurai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- AI Governance
- AI Observability
- LLM Evaluation
- Model Monitoring
- Guardrails
- MLOps
---
