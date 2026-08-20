---
api_specs:
- filename: convai-com-characters-api-openapi.yml
  format: yaml
  label: Convai Characters API
  slug: convai-com-characters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-characters-api-openapi.yml
- filename: convai-com-chat-history-api-openapi.yml
  format: yaml
  label: Convai Chat History API
  slug: convai-com-chat-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-chat-history-api-openapi.yml
- filename: convai-com-custom-llm-api-openapi.yml
  format: yaml
  label: Convai Custom LLM API
  slug: convai-com-custom-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-custom-llm-api-openapi.yml
- filename: convai-com-evaluation-api-openapi.yml
  format: yaml
  label: Convai Evaluation API
  slug: convai-com-evaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-evaluation-api-openapi.yml
- filename: convai-com-interaction-api-openapi.yml
  format: yaml
  label: Convai Interaction API
  slug: convai-com-interaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-interaction-api-openapi.yml
- filename: convai-com-knowledge-bank-api-openapi.yml
  format: yaml
  label: Convai Knowledge Bank API
  slug: convai-com-knowledge-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-knowledge-bank-api-openapi.yml
- filename: convai-com-live-api-openapi.yml
  format: yaml
  label: Convai Live API
  slug: convai-com-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-live-api-openapi.yml
- filename: convai-com-narrative-api-openapi.yml
  format: yaml
  label: Convai Narrative API
  slug: convai-com-narrative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-narrative-api-openapi.yml
- filename: convai-com-streaming-api-openapi.yml
  format: yaml
  label: Convai Streaming API
  slug: convai-com-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-streaming-api-openapi.yml
- filename: convai-com-tts-api-openapi.yml
  format: yaml
  label: Convai TTS API
  slug: convai-com-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/openapi/convai-com-tts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: convai.com
  spf: true
hosts:
- cert_expires: Sep 23 09:42:44 2026 GMT
  host: convai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 19:20:43 2026 GMT
  host: docs.convai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:24:32 2026 GMT
  host: api.convai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Convai Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Convai
provider_slug: convai-com
slug: convai-com-domain-security
source_filename: convai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: convai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:42:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.convai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:20:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.convai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:24:32 2026 GMT\n  hsts: null\ndomains:\n- domain: convai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convai-com/refs/heads/main/security/convai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Conversational AI
- Characters
- NPCs
- Virtual Worlds
- Games
- Avatars
- Speech
- TTS
- WebRTC
---
