---
api_specs:
- filename: fastrouter-audio-api-openapi.yml
  format: yaml
  label: Fastrouter Audio API
  slug: fastrouter-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-audio-api-openapi.yml
- filename: fastrouter-batches-api-openapi.yml
  format: yaml
  label: Fastrouter Batches API
  slug: fastrouter-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-batches-api-openapi.yml
- filename: fastrouter-embeddings-api-openapi.yml
  format: yaml
  label: Fastrouter Embeddings API
  slug: fastrouter-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-embeddings-api-openapi.yml
- filename: fastrouter-files-api-openapi.yml
  format: yaml
  label: Fastrouter Files API
  slug: fastrouter-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-files-api-openapi.yml
- filename: fastrouter-generation-api-openapi.yml
  format: yaml
  label: Fastrouter Generation API
  slug: fastrouter-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-generation-api-openapi.yml
- filename: fastrouter-getasyncresponse-api-openapi.yml
  format: yaml
  label: Fastrouter Get Async Response API
  slug: fastrouter-getasyncresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-getasyncresponse-api-openapi.yml
- filename: fastrouter-getprompttoaudioresponse-api-openapi.yml
  format: yaml
  label: Fastrouter Get Prompt To Audio Response API
  slug: fastrouter-getprompttoaudioresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-getprompttoaudioresponse-api-openapi.yml
- filename: fastrouter-images-api-openapi.yml
  format: yaml
  label: Fastrouter Images API
  slug: fastrouter-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-images-api-openapi.yml
- filename: fastrouter-model-api-openapi.yml
  format: yaml
  label: Fastrouter Model API
  slug: fastrouter-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-model-api-openapi.yml
- filename: fastrouter-models-api-openapi.yml
  format: yaml
  label: Fastrouter Models API
  slug: fastrouter-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-models-api-openapi.yml
- filename: fastrouter-moderations-api-openapi.yml
  format: yaml
  label: Fastrouter Moderations API
  slug: fastrouter-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-moderations-api-openapi.yml
- filename: fastrouter-responses-api-openapi.yml
  format: yaml
  label: Fastrouter Responses API
  slug: fastrouter-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-responses-api-openapi.yml
- filename: fastrouter-videos-api-openapi.yml
  format: yaml
  label: Fastrouter Videos API
  slug: fastrouter-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-videos-api-openapi.yml
- filename: fastrouter-chat-completions-api-openapi.yml
  format: yaml
  label: Fastrouter Chat Completions API
  slug: fastrouter-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-chat-completions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fastrouter.ai
  spf: true
hosts:
- cert_expires: Dec 25 00:51:29 2026 GMT
  host: fastrouter.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fastrouter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fastrouter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fastrouter
provider_slug: fastrouter
slug: fastrouter-domain-security
source_filename: fastrouter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fastrouter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 00:51:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fastrouter.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/security/fastrouter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- API Gateway
- LLM
- Enterprise
---
