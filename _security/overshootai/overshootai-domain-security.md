---
api_specs:
- filename: overshootai-billing-api-openapi.yml
  format: yaml
  label: overshoot.ai Billing API
  slug: overshootai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-billing-api-openapi.yml
- filename: overshootai-chat-api-openapi.yml
  format: yaml
  label: overshoot.ai Chat API
  slug: overshootai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-chat-api-openapi.yml
- filename: overshootai-healthz-api-openapi.yml
  format: yaml
  label: overshoot.ai Healthz API
  slug: overshootai-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-healthz-api-openapi.yml
- filename: overshootai-metrics-api-openapi.yml
  format: yaml
  label: overshoot.ai Metrics API
  slug: overshootai-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-metrics-api-openapi.yml
- filename: overshootai-models-api-openapi.yml
  format: yaml
  label: overshoot.ai Models API
  slug: overshootai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-models-api-openapi.yml
- filename: overshootai-readyz-api-openapi.yml
  format: yaml
  label: overshoot.ai Readyz API
  slug: overshootai-readyz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-readyz-api-openapi.yml
- filename: overshootai-streams-api-openapi.yml
  format: yaml
  label: overshoot.ai Streams API
  slug: overshootai-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-streams-api-openapi.yml
- filename: overshootai-v1beta-api-openapi.yml
  format: yaml
  label: overshoot.ai V1beta API
  slug: overshootai-v1beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/openapi/overshootai-v1beta-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: overshoot.ai
  spf: true
hosts:
- cert_expires: Sep 27 16:16:51 2026 GMT
  host: docs.overshoot.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 06:47:31 2026 GMT
  host: api.overshoot.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Overshootai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for overshoot.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: overshoot.ai
provider_slug: overshootai
slug: overshootai-domain-security
source_filename: overshootai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.overshoot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:16:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.overshoot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:47:31 2026 GMT\n  hsts: null\ndomains:\n- domain: overshoot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overshootai/refs/heads/main/security/overshootai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Computer-Vision
- Video
- Real-Time
- Streaming
- Machine-Learning
- Vision Language Models
- Inference
- Developer Tools
---
