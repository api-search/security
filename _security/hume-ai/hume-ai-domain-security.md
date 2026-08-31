---
api_specs:
- filename: hume-ai-default-api-openapi.yml
  format: yaml
  label: Hume AI Ai Default API
  slug: hume-ai-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-default-api-openapi.yml
- filename: hume-ai-subpackage-batch-api-openapi.yml
  format: yaml
  label: Hume AI subpackage_batch API
  slug: hume-ai-subpackage-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-subpackage-batch-api-openapi.yml
- filename: hume-ai-subpackage-chatgroups-api-openapi.yml
  format: yaml
  label: Hume AI subpackage_chatGroups API
  slug: hume-ai-subpackage-chatgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-subpackage-chatgroups-api-openapi.yml
- filename: hume-ai-subpackage-chats-api-openapi.yml
  format: yaml
  label: Hume AI subpackage_chats API
  slug: hume-ai-subpackage-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-subpackage-chats-api-openapi.yml
- filename: hume-ai-subpackage-configs-api-openapi.yml
  format: yaml
  label: Hume AI subpackage_configs API
  slug: hume-ai-subpackage-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-subpackage-configs-api-openapi.yml
- filename: hume-ai-subpackage-controlplane-api-openapi.yml
  format: yaml
  label: Hume AI subpackage_controlPlane API
  slug: hume-ai-subpackage-controlplane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-subpackage-controlplane-api-openapi.yml
- filename: hume-ai-subpackage-prompts-api-openapi.yml
  format: yaml
  label: Hume AI subpackage_prompts API
  slug: hume-ai-subpackage-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-subpackage-prompts-api-openapi.yml
- filename: hume-ai-subpackage-tools-api-openapi.yml
  format: yaml
  label: Hume AI subpackage_tools API
  slug: hume-ai-subpackage-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-subpackage-tools-api-openapi.yml
- filename: hume-ai-subpackage-voices-api-openapi.yml
  format: yaml
  label: Hume AI subpackage_voices API
  slug: hume-ai-subpackage-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-subpackage-voices-api-openapi.yml
- filename: hume-ai-speech-to-speech-evi-api-openapi.yml
  format: yaml
  label: Hume AI Speech To Speech (EVI) API
  slug: hume-ai-speech-to-speech-evi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-speech-to-speech-evi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hume.ai
  spf: true
hosts:
- cert_expires: Aug  9 15:41:55 2026 GMT
  host: www.hume.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 22:36:52 2026 GMT
  host: dev.hume.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 18:43:43 2026 GMT
  host: api.hume.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hume Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hume AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hume AI
provider_slug: hume-ai
slug: hume-ai-domain-security
source_filename: hume-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hume.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 15:41:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dev.hume.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:36:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hume.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:43:43 2026 GMT\n  hsts: null\ndomains:\n- domain: hume.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/security/hume-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Voice
- Empathic
- Emotion
- Multi-Modal
---
