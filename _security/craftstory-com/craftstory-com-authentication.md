---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: craftstory-com-audio-api-openapi.yml
  format: yaml
  label: CraftStory Audio API
  slug: craftstory-com-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-audio-api-openapi.yml
- filename: craftstory-com-craftstory-2-api-openapi.yml
  format: yaml
  label: CraftStory Craftstory 2 API
  slug: craftstory-com-craftstory-2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-craftstory-2-api-openapi.yml
- filename: craftstory-com-flux-3-max-api-openapi.yml
  format: yaml
  label: CraftStory Flux 3 Max API
  slug: craftstory-com-flux-3-max-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-flux-3-max-api-openapi.yml
- filename: craftstory-com-flux-3-video-api-openapi.yml
  format: yaml
  label: CraftStory Flux 3 Video API
  slug: craftstory-com-flux-3-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-flux-3-video-api-openapi.yml
- filename: craftstory-com-gemini-omni-flash-api-openapi.yml
  format: yaml
  label: CraftStory Gemini Omni Flash API
  slug: craftstory-com-gemini-omni-flash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-gemini-omni-flash-api-openapi.yml
- filename: craftstory-com-heygen-video-api-openapi.yml
  format: yaml
  label: CraftStory Heygen Video API
  slug: craftstory-com-heygen-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-heygen-video-api-openapi.yml
- filename: craftstory-com-images-api-openapi.yml
  format: yaml
  label: CraftStory Images API
  slug: craftstory-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-images-api-openapi.yml
- filename: craftstory-com-minimax-h3-api-openapi.yml
  format: yaml
  label: CraftStory Minimax H3 API
  slug: craftstory-com-minimax-h3-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-minimax-h3-api-openapi.yml
- filename: craftstory-com-minimax-h3-max-api-openapi.yml
  format: yaml
  label: CraftStory Minimax H3 Max API
  slug: craftstory-com-minimax-h3-max-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-minimax-h3-max-api-openapi.yml
- filename: craftstory-com-models-api-openapi.yml
  format: yaml
  label: CraftStory Models API
  slug: craftstory-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-models-api-openapi.yml
- filename: craftstory-com-music-api-openapi.yml
  format: yaml
  label: CraftStory Music API
  slug: craftstory-com-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-music-api-openapi.yml
- filename: craftstory-com-seedance-api-openapi.yml
  format: yaml
  label: CraftStory Seedance API
  slug: craftstory-com-seedance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-seedance-api-openapi.yml
- filename: craftstory-com-sound-effects-api-openapi.yml
  format: yaml
  label: CraftStory Sound Effects API
  slug: craftstory-com-sound-effects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-sound-effects-api-openapi.yml
- filename: craftstory-com-uploads-api-openapi.yml
  format: yaml
  label: CraftStory Uploads API
  slug: craftstory-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftstory-com/openapi/craftstory-com-uploads-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CraftStory Authentication
name_suffix: Authentication
oauth_flows: []
overview: CraftStory secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CraftStory
provider_slug: craftstory-com
scheme_count: 1
schemes:
- description: Enter 'Bearer sk-cs-...' (your API key from Account → API Access).
  docs_text: 'Authorization: Bearer sk-cs-… ; the key inherits the subscription of its owner'
  format: Bearer sk-cs-...
  in: header
  key_management: Keys are created and revoked in the CraftStory app under Account → API Access. The docs state tokens are SHA-256 hashed server-side and the plaintext is shown only once at creation; revoke and re-issue a key if you suspect a leak.
  key_prefix: sk-cs-
  name: ApiKey
  parameter: Authorization
  plan_requirement: 'A key whose owner plan does not include API access gets 401 {"detail": "Your subscription plan does not include API access."}; the pricing page says Producer adds API access.'
  sources:
  - openapi/craftstory-com-openapi.yml
  - https://api.craftstory.com/api/v1/docs/samples/curl/
  type: apiKey
slug: craftstory-com-authentication
source_filename: craftstory-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://api.craftstory.com/api/v1/docs/samples/curl/\ndocs: https://api.craftstory.com/api/v1/docs/samples/curl/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Bearer sk-cs-...'\n  key_prefix: sk-cs-\n  description: Enter 'Bearer sk-cs-...' (your API key from Account → API Access).\n  docs_text: 'Authorization: Bearer sk-cs-… ; the key inherits the subscription of its owner'\n  key_management: Keys are created and revoked in the CraftStory app under Account → API Access. The docs state tokens are SHA-256 hashed server-side and the plaintext is shown only once at creation; revoke and re-issue a key if you suspect a leak.\n  plan_requirement: 'A key whose owner plan does not include API access gets 401 {\"detail\": \"Your subscription plan does not include API access.\"}; the pricing page says Producer adds API access.'\n\
  \  sources:\n  - openapi/craftstory-com-openapi.yml\n  - https://api.craftstory.com/api/v1/docs/samples/curl/\n"
source_yaml_url: https://artifacts.apis.io/craftstory-com/authentication/craftstory-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI Video
- Video Generation
- Avatars
- Generative AI
- Lip Sync
- MCP
---
