---
api_specs:
- filename: ollama-blobs-api-openapi.yml
  format: yaml
  label: Ollama Blobs API
  slug: ollama-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-blobs-api-openapi.yml
- filename: ollama-chat-api-openapi.yml
  format: yaml
  label: Ollama Chat API
  slug: ollama-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-chat-api-openapi.yml
- filename: ollama-chat-completions-api-openapi.yml
  format: yaml
  label: Ollama Chat Completions API
  slug: ollama-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-chat-completions-api-openapi.yml
- filename: ollama-completions-api-openapi.yml
  format: yaml
  label: Ollama Completions API
  slug: ollama-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-completions-api-openapi.yml
- filename: ollama-embeddings-api-openapi.yml
  format: yaml
  label: Ollama Embeddings API
  slug: ollama-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-embeddings-api-openapi.yml
- filename: ollama-generate-api-openapi.yml
  format: yaml
  label: Ollama Generate API
  slug: ollama-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-generate-api-openapi.yml
- filename: ollama-images-api-openapi.yml
  format: yaml
  label: Ollama Images API
  slug: ollama-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-images-api-openapi.yml
- filename: ollama-models-api-openapi.yml
  format: yaml
  label: Ollama Models API
  slug: ollama-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-models-api-openapi.yml
- filename: ollama-responses-api-openapi.yml
  format: yaml
  label: Ollama Responses API
  slug: ollama-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-responses-api-openapi.yml
- filename: ollama-running-models-api-openapi.yml
  format: yaml
  label: Ollama Running Models API
  slug: ollama-running-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-running-models-api-openapi.yml
- filename: ollama-version-api-openapi.yml
  format: yaml
  label: Ollama Version API
  slug: ollama-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ollama.com
  spf: true
hosts:
- cert_expires: Sep 18 23:37:57 2026 GMT
  host: ollama.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:58:29 2026 GMT
  host: docs.ollama.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ollama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ollama, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ollama
provider_slug: ollama
slug: ollama-domain-security
source_filename: ollama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ollama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:37:57 2026 GMT\n  hsts: false\n- host: docs.ollama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:58:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ollama.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/security/ollama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Large Language Models
- Models
---
