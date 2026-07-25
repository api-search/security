---
api_specs:
- filename: moonshot-ai-batch-api-openapi.yml
  format: yaml
  label: Moonshot AI Batch API
  slug: moonshot-ai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonshot-ai/refs/heads/main/openapi/moonshot-ai-batch-api-openapi.yml
- filename: moonshot-ai-billing-api-openapi.yml
  format: yaml
  label: Moonshot AI Billing API
  slug: moonshot-ai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonshot-ai/refs/heads/main/openapi/moonshot-ai-billing-api-openapi.yml
- filename: moonshot-ai-chat-api-openapi.yml
  format: yaml
  label: Moonshot AI Chat API
  slug: moonshot-ai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonshot-ai/refs/heads/main/openapi/moonshot-ai-chat-api-openapi.yml
- filename: moonshot-ai-files-api-openapi.yml
  format: yaml
  label: Moonshot AI Files API
  slug: moonshot-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonshot-ai/refs/heads/main/openapi/moonshot-ai-files-api-openapi.yml
- filename: moonshot-ai-models-api-openapi.yml
  format: yaml
  label: Moonshot AI Models API
  slug: moonshot-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonshot-ai/refs/heads/main/openapi/moonshot-ai-models-api-openapi.yml
- filename: moonshot-ai-utilities-api-openapi.yml
  format: yaml
  label: Moonshot AI Utilities API
  slug: moonshot-ai-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonshot-ai/refs/heads/main/openapi/moonshot-ai-utilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moonshot.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: kimi.ai
  spf: true
hosts:
- cert_expires: Nov 26 11:15:02 2026 GMT
  host: www.moonshot.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 06:45:18 2026 GMT
  host: platform.kimi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 11:15:02 2026 GMT
  host: api.moonshot.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moonshot Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moonshot AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Moonshot AI
provider_slug: moonshot-ai
slug: moonshot-ai-domain-security
source_filename: moonshot-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moonshot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 11:15:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.kimi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 06:45:18 2026 GMT\n  hsts: false\n- host: api.moonshot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 11:15:02 2026 GMT\n  hsts: null\ndomains:\n- domain: moonshot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kimi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonshot-ai/refs/heads/main/security/moonshot-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- Long Context
- Kimi
---
