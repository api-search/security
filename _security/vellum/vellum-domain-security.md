---
api_specs:
- filename: vellum-openapi.json
  format: json
  label: Vellum LLM Platform API
  slug: llm-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vellum.ai
  spf: true
hosts:
- cert_expires: Aug 31 10:36:09 2026 GMT
  host: www.vellum.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 20:42:04 2026 GMT
  host: docs.vellum.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 20:34:23 2026 GMT
  host: api.vellum.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vellum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vellum AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vellum AI
provider_slug: vellum
slug: vellum-domain-security
source_filename: vellum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vellum.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:36:09 2026 GMT\n  hsts: false\n- host: docs.vellum.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:42:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vellum.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:34:23 2026 GMT\n  hsts: null\ndomains:\n- domain: vellum.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/security/vellum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LLM Platform
- Prompt Engineering
- Workflows
- Evaluations
- LLM Ops
- RAG
- Observability
- Datasets
- Deployments
- Multi-Provider
- Agent Builder
- Self-Hosted
---
