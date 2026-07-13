---
api_specs:
- filename: elevenlabs-text-to-speech-openapi.yml
  format: yaml
  label: ElevenLabs Text to Speech API
  slug: text-to-speech
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-text-to-speech-openapi.yml
- filename: elevenlabs-speech-to-text-openapi.yml
  format: yaml
  label: ElevenLabs Speech to Text API
  slug: speech-to-text
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-speech-to-text-openapi.yml
- filename: elevenlabs-voice-cloning-openapi.yml
  format: yaml
  label: ElevenLabs Voice Cloning API
  slug: voice-cloning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-voice-cloning-openapi.yml
- filename: elevenlabs-voices-openapi.yml
  format: yaml
  label: ElevenLabs Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-voices-openapi.yml
- filename: elevenlabs-sound-effects-openapi.yml
  format: yaml
  label: ElevenLabs Sound Effects API
  slug: sound-effects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-sound-effects-openapi.yml
- filename: elevenlabs-audio-isolation-openapi.yml
  format: yaml
  label: ElevenLabs Audio Isolation API
  slug: audio-isolation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-audio-isolation-openapi.yml
- filename: elevenlabs-dubbing-openapi.yml
  format: yaml
  label: ElevenLabs Dubbing API
  slug: dubbing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-dubbing-openapi.yml
- filename: elevenlabs-voice-changer-openapi.yml
  format: yaml
  label: ElevenLabs Voice Changer API
  slug: voice-changer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-voice-changer-openapi.yml
- filename: elevenlabs-music-openapi.yml
  format: yaml
  label: ElevenLabs Music Generation API
  slug: music
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-music-openapi.yml
- filename: elevenlabs-conversational-ai-openapi.yml
  format: yaml
  label: ElevenLabs Conversational AI API
  slug: conversational-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-conversational-ai-openapi.yml
- filename: elevenlabs-studio-openapi.yml
  format: yaml
  label: ElevenLabs Studio API
  slug: studio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/openapi/elevenlabs-studio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: elevenlabs.io
  spf: true
hosts:
- cert_expires: Sep 12 16:51:47 2026 GMT
  host: elevenlabs.io
  hsts: true
  hsts_max_age: 1800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 16:51:47 2026 GMT
  host: api.elevenlabs.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elevenlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for elevenlabs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: elevenlabs
provider_slug: elevenlabs
slug: elevenlabs-domain-security
source_filename: elevenlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elevenlabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:51:47 2026 GMT\n  hsts: true\n  hsts_max_age: 1800\n- host: api.elevenlabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:51:47 2026 GMT\n  hsts: null\ndomains:\n- domain: elevenlabs.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/security/elevenlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
