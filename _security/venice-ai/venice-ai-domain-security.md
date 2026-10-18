---
api_specs:
- filename: venice-ai-api-keys-api-openapi.yml
  format: yaml
  label: Venice.ai API Keys API
  slug: venice-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-api-keys-api-openapi.yml
- filename: venice-ai-audio-api-openapi.yml
  format: yaml
  label: Venice.ai Audio API
  slug: venice-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-audio-api-openapi.yml
- filename: venice-ai-augment-api-openapi.yml
  format: yaml
  label: Venice.ai Augment API
  slug: venice-ai-augment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-augment-api-openapi.yml
- filename: venice-ai-billing-api-openapi.yml
  format: yaml
  label: Venice.ai Billing API
  slug: venice-ai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-billing-api-openapi.yml
- filename: venice-ai-characters-api-openapi.yml
  format: yaml
  label: Venice.ai Characters API
  slug: venice-ai-characters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-characters-api-openapi.yml
- filename: venice-ai-crypto-rpc-api-openapi.yml
  format: yaml
  label: Venice.ai Crypto RPC API
  slug: venice-ai-crypto-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-crypto-rpc-api-openapi.yml
- filename: venice-ai-decisions-api-openapi.yml
  format: yaml
  label: Venice.ai Decisions API
  slug: venice-ai-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-decisions-api-openapi.yml
- filename: venice-ai-embeddings-api-openapi.yml
  format: yaml
  label: Venice.ai Embeddings API
  slug: venice-ai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-embeddings-api-openapi.yml
- filename: venice-ai-image-api-openapi.yml
  format: yaml
  label: Venice.ai Image API
  slug: venice-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-image-api-openapi.yml
- filename: venice-ai-models-api-openapi.yml
  format: yaml
  label: Venice.ai Models API
  slug: venice-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-models-api-openapi.yml
- filename: venice-ai-preview-api-openapi.yml
  format: yaml
  label: Venice.ai Preview API
  slug: venice-ai-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-preview-api-openapi.yml
- filename: venice-ai-responses-api-openapi.yml
  format: yaml
  label: Venice.ai Responses API
  slug: venice-ai-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-responses-api-openapi.yml
- filename: venice-ai-speech-api-openapi.yml
  format: yaml
  label: Venice.ai Speech API
  slug: venice-ai-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-speech-api-openapi.yml
- filename: venice-ai-transcriptions-api-openapi.yml
  format: yaml
  label: Venice.ai Transcriptions API
  slug: venice-ai-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-transcriptions-api-openapi.yml
- filename: venice-ai-video-api-openapi.yml
  format: yaml
  label: Venice.ai Video API
  slug: venice-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-video-api-openapi.yml
- filename: venice-ai-voices-api-openapi.yml
  format: yaml
  label: Venice.ai Voices API
  slug: venice-ai-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-voices-api-openapi.yml
- filename: venice-ai-x402-api-openapi.yml
  format: yaml
  label: Venice.ai X402 API
  slug: venice-ai-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-x402-api-openapi.yml
- filename: venice-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Venice.ai Chat Completions API
  slug: venice-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/openapi/venice-ai-chat-completions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: venice.ai
  spf: true
hosts:
- cert_expires: Jan  1 23:45:54 2027 GMT
  host: venice.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Venice Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Venice.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Venice.ai
provider_slug: venice-ai
slug: venice-ai-domain-security
source_filename: venice-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: venice.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:45:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: venice.ai\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venice-ai/refs/heads/main/security/venice-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- LLM
- Image Generation
- Video Generation
- Text-to-Speech
- Embeddings
- Privacy
- OpenAI-Compatible
- x402
---
