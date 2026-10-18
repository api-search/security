---
api_specs:
- filename: llmrouter-openapi-generated.yml
  format: yaml
  label: LLMrouter.eu API
  slug: llmrouter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmrouter/refs/heads/main/openapi/_ae-authored/llmrouter-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: llmrouter.eu
  spf: false
hosts:
- cert_expires: Jan 10 08:42:25 2027 GMT
  host: llmrouter.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llmrouter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LLMrouter.eu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: LLMrouter.eu
provider_slug: llmrouter
slug: llmrouter-domain-security
source_filename: llmrouter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmrouter.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 08:42:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: llmrouter.eu\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llmrouter/refs/heads/main/security/llmrouter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- SaaS
- Security
- EU
---
