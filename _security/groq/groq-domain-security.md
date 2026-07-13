---
api_specs:
- filename: groq-openapi.yml
  format: yaml
  label: Groq Chat Completions API
  slug: groq-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Reasoning API
  slug: groq-reasoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Vision API
  slug: groq-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Speech-to-Text API
  slug: groq-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Text-to-Speech API
  slug: groq-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Content Moderation API
  slug: groq-content-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Batch API
  slug: groq-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Flex Processing API
  slug: groq-flex-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Files API
  slug: groq-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Models API
  slug: groq-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Tools API
  slug: groq-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq LoRA Inference API
  slug: groq-lora-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
- filename: groq-openapi.yml
  format: yaml
  label: Groq Prompt Caching
  slug: groq-prompt-caching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/openapi/groq-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: groq.com
  spf: true
hosts:
- cert_expires: Oct  3 16:33:55 2026 GMT
  host: groq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 18:00:40 2026 GMT
  host: console.groq.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 15:31:53 2026 GMT
  host: api.groq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groq, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Groq
provider_slug: groq
slug: groq-domain-security
source_filename: groq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:33:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: console.groq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:00:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.groq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:31:53 2026 GMT\n  hsts: null\ndomains:\n- domain: groq.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groq/refs/heads/main/security/groq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- LPU
- Low Latency
---
