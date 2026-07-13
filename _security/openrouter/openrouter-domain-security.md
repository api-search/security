---
api_specs:
- filename: openapi.json
  format: json
  label: OpenRouter
  slug: openrouter
  spec_type: OpenAPI
  url: https://openrouter.ai/openapi.json
- filename: openapi.json
  format: json
  label: OpenRouter Chat Completions API
  slug: chat-completions-api
  spec_type: OpenAPI
  url: https://openrouter.ai/openapi.json
- filename: openapi.json
  format: json
  label: OpenRouter Models API
  slug: models-api
  spec_type: OpenAPI
  url: https://openrouter.ai/openapi.json
- filename: openapi.json
  format: json
  label: OpenRouter Generation API
  slug: generation-api
  spec_type: OpenAPI
  url: https://openrouter.ai/openapi.json
- filename: openapi.json
  format: json
  label: OpenRouter Keys Management API
  slug: keys-api
  spec_type: OpenAPI
  url: https://openrouter.ai/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openrouter.ai
  spf: true
hosts:
- cert_expires: Oct  4 19:49:33 2026 GMT
  host: openrouter.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openrouter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenRouter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenRouter
provider_slug: openrouter
slug: openrouter-domain-security
source_filename: openrouter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openrouter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:49:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openrouter.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrouter/refs/heads/main/security/openrouter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Gateway
- Large Language Models
- Router
---
