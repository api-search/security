---
api_specs:
- filename: mindlogic-audio-api-openapi.yml
  format: yaml
  label: Mindlogic Audio API
  slug: mindlogic-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/openapi/mindlogic-audio-api-openapi.yml
- filename: mindlogic-chat-api-openapi.yml
  format: yaml
  label: Mindlogic Chat API
  slug: mindlogic-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/openapi/mindlogic-chat-api-openapi.yml
- filename: mindlogic-credits-api-openapi.yml
  format: yaml
  label: Mindlogic Credits API
  slug: mindlogic-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/openapi/mindlogic-credits-api-openapi.yml
- filename: mindlogic-gateway-api-openapi.yml
  format: yaml
  label: Mindlogic gateway API
  slug: mindlogic-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/openapi/mindlogic-gateway-api-openapi.yml
- filename: mindlogic-images-api-openapi.yml
  format: yaml
  label: Mindlogic Images API
  slug: mindlogic-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/openapi/mindlogic-images-api-openapi.yml
- filename: mindlogic-models-api-openapi.yml
  format: yaml
  label: Mindlogic Models API
  slug: mindlogic-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/openapi/mindlogic-models-api-openapi.yml
- filename: mindlogic-video-api-openapi.yml
  format: yaml
  label: Mindlogic Video API
  slug: mindlogic-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/openapi/mindlogic-video-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mindlogic.ai
  spf: true
hosts:
- cert_expires: Aug 29 02:41:05 2026 GMT
  host: mindlogic.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 17:55:05 2026 GMT
  host: docs.mindlogic.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 11:45:25 2026 GMT
  host: factchat-cloud.mindlogic.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mindlogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mindlogic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mindlogic
provider_slug: mindlogic
slug: mindlogic-domain-security
source_filename: mindlogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindlogic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 02:41:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.mindlogic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:55:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: factchat-cloud.mindlogic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:45:25 2026 GMT\n  hsts: null\ndomains:\n- domain: mindlogic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindlogic/refs/heads/main/security/mindlogic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI/ML
- Generative AI
- Conversational AI
- LLM Gateway
- Chatbots
- API Gateway
- Korea
---
