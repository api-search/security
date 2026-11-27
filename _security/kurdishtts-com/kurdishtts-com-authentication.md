---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kurdishtts-com-stt-api-openapi.yml
  format: yaml
  label: Kurdish TTS STT API
  slug: kurdishtts-com-stt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kurdishtts-com/openapi/kurdishtts-com-stt-api-openapi.yml
- filename: kurdishtts-com-tts-api-openapi.yml
  format: yaml
  label: Kurdish TTS TTS API
  slug: kurdishtts-com-tts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kurdishtts-com/openapi/kurdishtts-com-tts-api-openapi.yml
- filename: kurdishtts-com-voices-api-openapi.yml
  format: yaml
  label: Kurdish TTS Voices API
  slug: kurdishtts-com-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kurdishtts-com/openapi/kurdishtts-com-voices-api-openapi.yml
auth_types: []
description: Authentication uses an API key passed in the request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kurdish TTS Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kurdish TTS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kurdish TTS
provider_slug: kurdishtts-com
scheme_count: 1
schemes:
- evidence: ' -H "x-api-key: YOUR_TTS_KEY" \'
  header: x-api-key
  how_to_obtain: Create a free account at kurdishtts.com and generate a TTS key in Settings → API.
  location: header
  name: x-api-key
  type: apiKey
slug: kurdishtts-com-authentication
source_filename: kurdishtts-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.kurdishtts.com/docs/guides/kurdish-text-to-speech-api
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.kurdishtts.com/docs/guides/kurdish-text-to-speech-api\nsources:\n- https://www.kurdishtts.com/docs/guides/kurdish-text-to-speech-api\ndescription: Authentication uses an API key passed in the request header.\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: ' -H \"x-api-key: YOUR_TTS_KEY\" \\'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a free account at kurdishtts.com and generate a TTS key in Settings → API.\ndocs: https://www.kurdishtts.com/docs/guides/kurdish-text-to-speech-api\n"
source_yaml_url: https://artifacts.apis.io/kurdishtts-com/authentication/kurdishtts-com-authentication.yml
summary_line: 1 scheme
tags:
- Kurdish
- Text-to-Speech
- Speech-to-Text
- Voice Chat
- Artificial Intelligence
---
