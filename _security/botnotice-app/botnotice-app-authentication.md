---
anonymous_access: false
api_key_in: []
api_specs:
- filename: botnotice-app-consent-api-openapi.yml
  format: yaml
  label: BotNotice Consent API
  slug: botnotice-app-consent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-consent-api-openapi.yml
- filename: botnotice-app-content-register-api-openapi.yml
  format: yaml
  label: BotNotice Content register API
  slug: botnotice-app-content-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-content-register-api-openapi.yml
- filename: botnotice-app-free-tools-api-openapi.yml
  format: yaml
  label: BotNotice Free tools API
  slug: botnotice-app-free-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-free-tools-api-openapi.yml
- filename: botnotice-app-law-dataset-api-openapi.yml
  format: yaml
  label: BotNotice Law dataset API
  slug: botnotice-app-law-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-law-dataset-api-openapi.yml
- filename: botnotice-app-voice-api-openapi.yml
  format: yaml
  label: BotNotice Voice API
  slug: botnotice-app-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-voice-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: BotNotice Authentication
name_suffix: Authentication
oauth_flows: []
overview: BotNotice secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BotNotice
provider_slug: botnotice-app
scheme_count: 1
schemes:
- description: The site's voice token (starts with bni_), from the dashboard's Voice page. Also accepted as ?token= on voice endpoints, and as x-vapi-secret on /api/voice/event.
  name: voiceToken
  scheme: bearer
  sources:
  - openapi/botnotice-app-openapi.json
  type: http
slug: botnotice-app-authentication
source_filename: botnotice-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/botnotice-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: voiceToken\n  type: http\n  scheme: bearer\n  description: The site's voice token (starts with bni_), from the dashboard's Voice page. Also\n    accepted as ?token= on voice endpoints, and as x-vapi-secret on /api/voice/event.\n  sources:\n  - openapi/botnotice-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/botnotice-app/authentication/botnotice-app-authentication.yml
summary_line: http · 1 scheme
tags:
- AI disclosure
- chatbot compliance
- Recordkeeping
- website widget
- managed compliance
- subscription pricing
---
