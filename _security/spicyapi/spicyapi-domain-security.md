---
api_specs:
- filename: spicyapi-account-api-openapi.yml
  format: yaml
  label: SpicyAPI Account API
  slug: spicyapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/openapi/spicyapi-account-api-openapi.yml
- filename: spicyapi-media-api-openapi.yml
  format: yaml
  label: SpicyAPI Media API
  slug: spicyapi-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/openapi/spicyapi-media-api-openapi.yml
- filename: spicyapi-models-api-openapi.yml
  format: yaml
  label: SpicyAPI Models API
  slug: spicyapi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/openapi/spicyapi-models-api-openapi.yml
- filename: spicyapi-openai-compatible-api-openapi.yml
  format: yaml
  label: SpicyAPI OpenAI Compatible API
  slug: spicyapi-openai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/openapi/spicyapi-openai-compatible-api-openapi.yml
- filename: spicyapi-tasks-api-openapi.yml
  format: yaml
  label: SpicyAPI Tasks API
  slug: spicyapi-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/openapi/spicyapi-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spicyapi.ai
  spf: true
hosts:
- cert_expires: Nov 28 14:41:23 2026 GMT
  host: spicyapi.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 10:55:57 2026 GMT
  host: docs.spicyapi.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 14:41:23 2026 GMT
  host: api.spicyapi.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Spicyapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpicyAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SpicyAPI
provider_slug: spicyapi
slug: spicyapi-domain-security
source_filename: spicyapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spicyapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 14:41:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.spicyapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:55:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spicyapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 14:41:23 2026 GMT\n  hsts: null\ndomains:\n- domain: spicyapi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spicyapi/refs/heads/main/security/spicyapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Generative Media
- LLM
- Video Generation
- Image Generation
- Model Aggregator
---
