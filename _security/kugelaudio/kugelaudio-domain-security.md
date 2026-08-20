---
api_specs:
- filename: kugelaudio-11labs-api-openapi.yml
  format: yaml
  label: KugelAudio 11labs API
  slug: kugelaudio-11labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-11labs-api-openapi.yml
- filename: kugelaudio-audio-api-openapi.yml
  format: yaml
  label: KugelAudio Audio API
  slug: kugelaudio-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-audio-api-openapi.yml
- filename: kugelaudio-billing-api-openapi.yml
  format: yaml
  label: KugelAudio billing API
  slug: kugelaudio-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-billing-api-openapi.yml
- filename: kugelaudio-dictionaries-api-openapi.yml
  format: yaml
  label: KugelAudio Dictionaries API
  slug: kugelaudio-dictionaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-dictionaries-api-openapi.yml
- filename: kugelaudio-health-api-openapi.yml
  format: yaml
  label: KugelAudio Health API
  slug: kugelaudio-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-health-api-openapi.yml
- filename: kugelaudio-license-api-openapi.yml
  format: yaml
  label: KugelAudio license API
  slug: kugelaudio-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-license-api-openapi.yml
- filename: kugelaudio-models-api-openapi.yml
  format: yaml
  label: KugelAudio Models API
  slug: kugelaudio-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-models-api-openapi.yml
- filename: kugelaudio-normalize-api-openapi.yml
  format: yaml
  label: KugelAudio Normalize API
  slug: kugelaudio-normalize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-normalize-api-openapi.yml
- filename: kugelaudio-post-overrides-api-openapi.yml
  format: yaml
  label: KugelAudio Post Overrides API
  slug: kugelaudio-post-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-post-overrides-api-openapi.yml
- filename: kugelaudio-predict-api-openapi.yml
  format: yaml
  label: KugelAudio Predict API
  slug: kugelaudio-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-predict-api-openapi.yml
- filename: kugelaudio-ready-api-openapi.yml
  format: yaml
  label: KugelAudio Ready API
  slug: kugelaudio-ready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-ready-api-openapi.yml
- filename: kugelaudio-tts-api-openapi.yml
  format: yaml
  label: KugelAudio Tts API
  slug: kugelaudio-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-tts-api-openapi.yml
- filename: kugelaudio-vapi-api-openapi.yml
  format: yaml
  label: KugelAudio Vapi API
  slug: kugelaudio-vapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-vapi-api-openapi.yml
- filename: kugelaudio-voices-api-openapi.yml
  format: yaml
  label: KugelAudio Voices API
  slug: kugelaudio-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-voices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kugelaudio.com
  spf: true
hosts:
- cert_expires: Oct 16 00:54:29 2026 GMT
  host: www.kugelaudio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 13:04:24 2026 GMT
  host: docs.kugelaudio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 00:54:29 2026 GMT
  host: api.kugelaudio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kugelaudio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KugelAudio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: KugelAudio
provider_slug: kugelaudio
slug: kugelaudio-domain-security
source_filename: kugelaudio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kugelaudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:54:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.kugelaudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 13:04:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kugelaudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:54:29 2026 GMT\n  hsts: null\ndomains:\n- domain: kugelaudio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/security/kugelaudio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Voice
- Text-to-Speech
- Speech Synthesis
- Voice AI
- Voice Cloning
- Audio
- Artificial Intelligence
- Machine-Learning
- Streaming
- Real-Time
- Conversational AI
- Europe
- Data Sovereignty
- GDPR
- Company
---
