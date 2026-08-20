---
api_specs:
- filename: modulate-velma-2-accent-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Accent Batch API
  slug: modulate-velma-2-accent-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-accent-batch-api-openapi.yml
- filename: modulate-velma-2-ai-music-detection-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Ai Music Detection Batch API
  slug: modulate-velma-2-ai-music-detection-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-ai-music-detection-batch-api-openapi.yml
- filename: modulate-velma-2-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Batch API
  slug: modulate-velma-2-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-batch-api-openapi.yml
- filename: modulate-velma-2-emotion-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Emotion Batch API
  slug: modulate-velma-2-emotion-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-emotion-batch-api-openapi.yml
- filename: modulate-velma-2-language-detection-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Language Detection Batch API
  slug: modulate-velma-2-language-detection-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-language-detection-batch-api-openapi.yml
- filename: modulate-velma-2-music-detection-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Music Detection Batch API
  slug: modulate-velma-2-music-detection-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-music-detection-batch-api-openapi.yml
- filename: modulate-velma-2-pii-phi-redaction-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Pii Phi Redaction Batch API
  slug: modulate-velma-2-pii-phi-redaction-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-pii-phi-redaction-batch-api-openapi.yml
- filename: modulate-velma-2-stt-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Stt Batch API
  slug: modulate-velma-2-stt-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-stt-batch-api-openapi.yml
- filename: modulate-velma-2-stt-batch-english-vfast-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Stt Batch English Vfast API
  slug: modulate-velma-2-stt-batch-english-vfast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-stt-batch-english-vfast-api-openapi.yml
- filename: modulate-velma-2-stt-batch-multilingual-vfast-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Stt Batch Multilingual Vfast API
  slug: modulate-velma-2-stt-batch-multilingual-vfast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-stt-batch-multilingual-vfast-api-openapi.yml
- filename: modulate-velma-2-synthetic-voice-detection-batch-api-openapi.yml
  format: yaml
  label: Modulate Velma 2 Synthetic Voice Detection Batch API
  slug: modulate-velma-2-synthetic-voice-detection-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/modulate-velma-2-synthetic-voice-detection-batch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modulate.ai
  spf: true
hosts:
- cert_expires: Sep 30 03:07:49 2026 GMT
  host: modulate.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 21:58:08 2026 GMT
  host: docs.modulate.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: platform.modulate.ai
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modulate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modulate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Modulate
provider_slug: modulate
slug: modulate-domain-security
source_filename: modulate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modulate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 03:07:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.modulate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:58:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.modulate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: modulate.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/security/modulate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Voice AI
- Speech-to-Text
- Transcription
- Deepfake Detection
- Content Moderation
- Trust and Safety
- Audio
- Machine-Learning
- PII Redaction
- Voice Intelligence
---
