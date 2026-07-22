---
api_specs:
- filename: velma-2-batch-openapi-original.yml
  format: yaml
  label: Velma-2 Voice Intelligence API
  slug: velma-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/velma-2-batch-openapi-original.yml
- filename: stt-batch-openapi-original.yml
  format: yaml
  label: Speech-to-Text Transcription API
  slug: stt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/stt-batch-openapi-original.yml
- filename: synthetic-voice-detection-batch-openapi-original.yml
  format: yaml
  label: Deepfake (Synthetic Voice) Detection API
  slug: deepfake-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/synthetic-voice-detection-batch-openapi-original.yml
- filename: pii-phi-redaction-batch-openapi-original.yml
  format: yaml
  label: PII/PHI Redaction API
  slug: pii-phi-redaction
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/pii-phi-redaction-batch-openapi-original.yml
- filename: emotion-batch-openapi-original.yml
  format: yaml
  label: Emotion Detection API
  slug: emotion-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/emotion-batch-openapi-original.yml
- filename: accent-batch-openapi-original.yml
  format: yaml
  label: Accent Detection API
  slug: accent-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/accent-batch-openapi-original.yml
- filename: language-detection-batch-openapi-original.yml
  format: yaml
  label: Language Detection API
  slug: language-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/language-detection-batch-openapi-original.yml
- filename: music-detection-batch-openapi-original.yml
  format: yaml
  label: Music & Speech Detection API
  slug: music-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/music-detection-batch-openapi-original.yml
- filename: ai-music-detection-batch-openapi-original.yml
  format: yaml
  label: AI Music Detection API
  slug: ai-music-detection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modulate/refs/heads/main/openapi/ai-music-detection-batch-openapi-original.yml
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
- Ai
- Voice AI
- Speech to Text
- Transcription
- Deepfake Detection
- Content Moderation
- Trust and Safety
- Audio
- Machine Learning
- PII Redaction
- Voice Intelligence
---
