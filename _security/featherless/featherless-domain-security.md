---
api_specs:
- filename: featherless-openapi.yml
  format: yaml
  label: Featherless Chat Completions API
  slug: featherless-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featherless/refs/heads/main/openapi/featherless-openapi.yml
- filename: featherless-openapi.yml
  format: yaml
  label: Featherless Completions API
  slug: featherless-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featherless/refs/heads/main/openapi/featherless-openapi.yml
- filename: featherless-openapi.yml
  format: yaml
  label: Featherless Models API
  slug: featherless-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featherless/refs/heads/main/openapi/featherless-openapi.yml
- filename: featherless-openapi.yml
  format: yaml
  label: Featherless Embeddings API
  slug: featherless-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/featherless/refs/heads/main/openapi/featherless-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: featherless.ai
  spf: true
hosts:
- cert_expires: Sep 24 19:34:15 2026 GMT
  host: featherless.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:26:51 2026 GMT
  host: api.featherless.ai
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Featherless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Featherless AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Featherless AI
provider_slug: featherless
slug: featherless-domain-security
source_filename: featherless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: featherless.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 19:34:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.featherless.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:26:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: featherless.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/featherless/refs/heads/main/security/featherless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- Serverless
- Open Models
---
