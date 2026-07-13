---
api_specs:
- filename: fal-model-apis-openapi.yml
  format: yaml
  label: fal Model APIs
  slug: fal-model-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-model-apis-openapi.yml
- filename: fal-ai-asyncapi.yml
  format: yaml
  label: fal Realtime API
  slug: fal-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/asyncapi/fal-ai-asyncapi.yml
- filename: fal-ai-asyncapi.yml
  format: yaml
  label: fal Streaming API
  slug: fal-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/asyncapi/fal-ai-asyncapi.yml
- filename: fal-storage-api-openapi.yml
  format: yaml
  label: fal Storage API
  slug: fal-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-storage-api-openapi.yml
- filename: fal-serverless-platform-api-openapi.yml
  format: yaml
  label: fal Serverless Platform API
  slug: fal-serverless-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-serverless-platform-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fal.ai
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: fal.run
  spf: false
hosts:
- cert_expires: Sep 18 20:46:02 2026 GMT
  host: fal.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 01:11:22 2026 GMT
  host: queue.fal.run
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: realtime.fal.run
  https: false
kind: domain-security
layout: security
method: probed
name: Fal Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fal, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: fal
provider_slug: fal-ai
slug: fal-ai-domain-security
source_filename: fal-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:46:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: queue.fal.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 01:11:22 2026 GMT\n  hsts: null\n- host: realtime.fal.run\n  https: false\ndomains:\n- domain: fal.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fal.run\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/security/fal-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Artificial Intelligence
- Generative AI
- Generative Media
- Image Generation
- Video Generation
- Audio Generation
- Inference
- Serverless
- GPU
- MCP
---
