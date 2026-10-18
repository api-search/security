---
api_specs:
- filename: airouter-ai-router-api-api-openapi.yml
  format: yaml
  label: AI Router AI Router API
  slug: airouter-ai-router-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airouter/refs/heads/main/openapi/airouter-ai-router-api-api-openapi.yml
- filename: airouter-chat-completions-api-openapi.yml
  format: yaml
  label: AI Router Chat Completions API
  slug: airouter-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airouter/refs/heads/main/openapi/airouter-chat-completions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: airouter.io
  spf: true
hosts:
- cert_expires: Nov 26 02:49:15 2026 GMT
  host: airouter.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airouter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Router, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AI Router
provider_slug: airouter
slug: airouter-domain-security
source_filename: airouter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airouter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 02:49:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: airouter.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airouter/refs/heads/main/security/airouter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LLM Cost Optimization
- Model Routing
- Enterprise AI
- Privacy
---
