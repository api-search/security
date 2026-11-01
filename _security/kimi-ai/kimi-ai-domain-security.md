---
api_specs:
- filename: kimi-ai-batch-api-openapi.yml
  format: yaml
  label: Moonshot AI Batch API
  slug: kimi-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-batch-api-openapi.yml
- filename: kimi-ai-billing-api-openapi.yml
  format: yaml
  label: Moonshot AI Billing API
  slug: kimi-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-billing-api-openapi.yml
- filename: kimi-ai-files-api-openapi.yml
  format: yaml
  label: Moonshot AI Files API
  slug: kimi-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-files-api-openapi.yml
- filename: kimi-ai-models-api-openapi.yml
  format: yaml
  label: Moonshot AI Models API
  slug: kimi-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-models-api-openapi.yml
- filename: kimi-ai-utilities-api-openapi.yml
  format: yaml
  label: Moonshot AI Utilities API
  slug: kimi-ai-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-utilities-api-openapi.yml
- filename: kimi-ai-responses-api-openapi.yml
  format: yaml
  label: Moonshot AI Responses API
  slug: kimi-ai-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-responses-api-openapi.yml
- filename: kimi-ai-tools-api-openapi.yml
  format: yaml
  label: Moonshot AI Tools API
  slug: kimi-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-tools-api-openapi.yml
- filename: kimi-ai-messages-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Messages API
  slug: kimi-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-messages-api-openapi.yml
- filename: kimi-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Chat Completions API
  slug: kimi-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-chat-completions-api-openapi.yml
description: ''
domains:
- caa:
  - moonshot.ai.cdn.cloudflare.net.
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
- cert_expires: Dec  9 09:17:36 2026 GMT
  host: platform.kimi.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 11:15:02 2026 GMT
  host: api.moonshot.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Kimi Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kimi (Moonshot AI), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kimi (Moonshot AI)
provider_slug: kimi-ai
slug: kimi-ai-domain-security
source_filename: kimi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moonshot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 11:15:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.kimi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 09:17:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moonshot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 11:15:02 2026 GMT\n  hsts: null\ndomains:\n- domain: moonshot.ai\n  dnssec: false\n  caa:\n  - moonshot.ai.cdn.cloudflare.net.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kimi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kimi-ai/security/kimi-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LLM
- Inference
- Long Context
- Kimi
- Foundation Models
---
