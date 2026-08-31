---
api_specs:
- filename: secton-api-chat-api-openapi.yml
  format: yaml
  label: Secton API Chat API
  slug: secton-api-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secton-api/refs/heads/main/openapi/secton-api-chat-api-openapi.yml
- filename: secton-api-models-api-openapi.yml
  format: yaml
  label: Secton API Models API
  slug: secton-api-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secton-api/refs/heads/main/openapi/secton-api-models-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: secton.org
  spf: true
hosts:
- cert_expires: Oct 30 19:15:56 2026 GMT
  host: console.secton.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 19:15:56 2026 GMT
  host: api.secton.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Secton Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Secton API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Secton API
provider_slug: secton-api
slug: secton-api-domain-security
source_filename: secton-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.secton.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 19:15:56 2026 GMT\n  hsts: false\n- host: api.secton.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 19:15:56 2026 GMT\n  hsts: false\ndomains:\n- domain: secton.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secton-api/refs/heads/main/security/secton-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Inference
- llm
- chat-completions
- generative-ai
- Developer Tools
- openai-compatible
- streaming
- machine-learning
---
