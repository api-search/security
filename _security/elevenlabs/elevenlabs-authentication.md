---
api_key_in:
- header
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
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Elevenlabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: elevenlabs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: elevenlabs
provider_slug: elevenlabs
scheme_count: 1
schemes:
- description: ElevenLabs API key passed in the xi-api-key header for authentication.
  in: header
  name: apiKeyAuth
  parameter: xi-api-key
  sources:
  - openapi/elevenlabs-audio-isolation-openapi.yml
  - openapi/elevenlabs-conversational-ai-openapi.yml
  - openapi/elevenlabs-dubbing-openapi.yml
  - openapi/elevenlabs-music-openapi.yml
  - openapi/elevenlabs-sound-effects-openapi.yml
  - openapi/elevenlabs-speech-to-text-openapi.yml
  - openapi/elevenlabs-studio-openapi.yml
  - openapi/elevenlabs-text-to-speech-openapi.yml
  - openapi/elevenlabs-voice-changer-openapi.yml
  - openapi/elevenlabs-voice-cloning-openapi.yml
  - openapi/elevenlabs-voices-openapi.yml
  type: apiKey
slug: elevenlabs-authentication
source_filename: elevenlabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elevenlabs-audio-isolation-openapi.yml, openapi/elevenlabs-conversational-ai-openapi.yml,\n  openapi/elevenlabs-dubbing-openapi.yml, openapi/elevenlabs-music-openapi.yml, openapi/elevenlabs-sound-effects-openapi.yml,\n  openapi/elevenlabs-speech-to-text-openapi.yml, openapi/elevenlabs-studio-openapi.yml, openapi/elevenlabs-text-to-speech-openapi.yml,\n  openapi/elevenlabs-voice-changer-openapi.yml, openapi/elevenlabs-voice-cloning-openapi.yml,\n  openapi/elevenlabs-voices-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: xi-api-key\n  description: ElevenLabs API key passed in the xi-api-key header for authentication.\n  sources:\n  - openapi/elevenlabs-audio-isolation-openapi.yml\n  - openapi/elevenlabs-conversational-ai-openapi.yml\n  - openapi/elevenlabs-dubbing-openapi.yml\n  - openapi/elevenlabs-music-openapi.yml\n  - openapi/elevenlabs-sound-effects-openapi.yml\n\
  \  - openapi/elevenlabs-speech-to-text-openapi.yml\n  - openapi/elevenlabs-studio-openapi.yml\n  - openapi/elevenlabs-text-to-speech-openapi.yml\n  - openapi/elevenlabs-voice-changer-openapi.yml\n  - openapi/elevenlabs-voice-cloning-openapi.yml\n  - openapi/elevenlabs-voices-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/authentication/elevenlabs-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
