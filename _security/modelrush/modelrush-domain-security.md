---
api_specs:
- filename: modelrush-audio-api-openapi.yml
  format: yaml
  label: ModelRush Audio API
  slug: modelrush-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/openapi/modelrush-audio-api-openapi.yml
- filename: modelrush-chat-api-openapi.yml
  format: yaml
  label: ModelRush Chat API
  slug: modelrush-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/openapi/modelrush-chat-api-openapi.yml
- filename: modelrush-discovery-api-openapi.yml
  format: yaml
  label: ModelRush Discovery API
  slug: modelrush-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/openapi/modelrush-discovery-api-openapi.yml
- filename: modelrush-images-api-openapi.yml
  format: yaml
  label: ModelRush Images API
  slug: modelrush-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/openapi/modelrush-images-api-openapi.yml
- filename: modelrush-predictions-api-openapi.yml
  format: yaml
  label: ModelRush Predictions API
  slug: modelrush-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/openapi/modelrush-predictions-api-openapi.yml
- filename: modelrush-uploads-api-openapi.yml
  format: yaml
  label: ModelRush Uploads API
  slug: modelrush-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/openapi/modelrush-uploads-api-openapi.yml
- filename: modelrush-video-api-openapi.yml
  format: yaml
  label: ModelRush Video API
  slug: modelrush-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/openapi/modelrush-video-api-openapi.yml
- filename: modelrush-webhooks-api-openapi.yml
  format: yaml
  label: ModelRush Webhooks API
  slug: modelrush-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/openapi/modelrush-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  - 0 issue "pki.goog"
  - 0 issue "amazontrust.com"
  dmarc: false
  dnssec: false
  domain: modelrush.ai
  spf: true
hosts:
- cert_expires: Nov  6 23:58:00 2026 GMT
  host: modelrush.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:58:00 2026 GMT
  host: api.modelrush.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Modelrush Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ModelRush, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ModelRush
provider_slug: modelrush
slug: modelrush-domain-security
source_filename: modelrush-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modelrush.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:58:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.modelrush.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:58:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: modelrush.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/security/modelrush-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- LLM
- Inference
- Multi-Modal
- Model Hosting
- Speech
- Image Generation
---
