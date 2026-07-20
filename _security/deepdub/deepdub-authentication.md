---
api_key_in:
- header
api_specs:
- filename: deepdub-api-openapi-original.json
  format: json
  label: Deepdub Text-to-Speech API
  slug: deepdub-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepdub/refs/heads/main/openapi/deepdub-api-openapi-original.json
- filename: deepdub-managed-dub-openapi-original.json
  format: json
  label: Deepdub Managed Dubbing API
  slug: deepdub-managed-dubbing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepdub/refs/heads/main/openapi/deepdub-managed-dub-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Deepdub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deepdub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deepdub
provider_slug: deepdub
scheme_count: 1
schemes:
- description: API key passed in the x-api-key header. Keys follow the format dd-{random}{checksum} where the last 8 characters are a validation checksum; keys always start with the dd- prefix. A shared free-trial key (dd-00000000000000000000000065c9cbfe) is IP rate-limited and US-region only.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/deepdub-api-openapi-original.json
  - openapi/deepdub-managed-dub-openapi-original.json
  type: apiKey
slug: deepdub-authentication
source_filename: deepdub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource:\n- openapi/deepdub-api-openapi-original.json\n- openapi/deepdub-managed-dub-openapi-original.json\ndocs: https://docs.deepdub.ai/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: >-\n    API key passed in the x-api-key header. Keys follow the format dd-{random}{checksum} where the\n    last 8 characters are a validation checksum; keys always start with the dd- prefix. A shared\n    free-trial key (dd-00000000000000000000000065c9cbfe) is IP rate-limited and US-region only.\n  sources:\n  - openapi/deepdub-api-openapi-original.json\n  - openapi/deepdub-managed-dub-openapi-original.json\nregions:\n  us_default: https://restapi.deepdub.ai/api/v1\n  eu: https://eu-restapi.deepdub.ai/api/v1\n  note: EU region requires a production API key (not available on the free trial).\nkey_management: Contact support@deepdub.ai\
  \ or generate a key from the Deepdub dashboard. Rotate keys periodically; use separate dev/prod keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepdub/refs/heads/main/authentication/deepdub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Voice
- Text to Speech
- Dubbing
- Localization
- Speech Synthesis
- Voice Cloning
- Media
- Artificial Intelligence
- Audio
---
