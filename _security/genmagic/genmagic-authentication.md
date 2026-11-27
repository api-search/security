---
anonymous_access: false
api_key_in: []
api_specs:
- filename: genmagic-agent-api-openapi.yml
  format: yaml
  label: GenMagic Agent API
  slug: genmagic-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-agent-api-openapi.yml
- filename: genmagic-audio-api-openapi.yml
  format: yaml
  label: GenMagic Audio API
  slug: genmagic-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-audio-api-openapi.yml
- filename: genmagic-benchmarks-api-openapi.yml
  format: yaml
  label: GenMagic Benchmarks API
  slug: genmagic-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-benchmarks-api-openapi.yml
- filename: genmagic-images-api-openapi.yml
  format: yaml
  label: GenMagic Images API
  slug: genmagic-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-images-api-openapi.yml
- filename: genmagic-models-api-openapi.yml
  format: yaml
  label: GenMagic Models API
  slug: genmagic-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-models-api-openapi.yml
- filename: genmagic-text-api-openapi.yml
  format: yaml
  label: GenMagic Text API
  slug: genmagic-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-text-api-openapi.yml
- filename: genmagic-usage-api-openapi.yml
  format: yaml
  label: GenMagic Usage API
  slug: genmagic-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-usage-api-openapi.yml
- filename: genmagic-videos-api-openapi.yml
  format: yaml
  label: GenMagic Videos API
  slug: genmagic-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-videos-api-openapi.yml
- filename: genmagic-chat-completions-api-openapi.yml
  format: yaml
  label: GenMagic Chat Completions API
  slug: genmagic-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genmagic/openapi/genmagic-chat-completions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GenMagic Authentication
name_suffix: Authentication
oauth_flows: []
overview: GenMagic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GenMagic
provider_slug: genmagic
scheme_count: 1
schemes:
- description: 'GenMagic API key in the form gm_live_..., sent as Authorization: Bearer <key>. Also accepted as x-api-key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/genmagic-openapi.json
  type: http
slug: genmagic-authentication
source_filename: genmagic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/genmagic-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'GenMagic API key in the form gm_live_..., sent as Authorization: Bearer <key>.\n    Also accepted as x-api-key.'\n  sources:\n  - openapi/genmagic-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/genmagic/authentication/genmagic-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Generative AI
- Media
- Subscription
---
