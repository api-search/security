---
anonymous_access: false
api_key_in: []
api_specs:
- filename: icallagent-public-api-agents-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Agents API
  slug: icallagent-public-api-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-agents-api-openapi.yml
- filename: icallagent-public-api-campaigns-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Campaigns API
  slug: icallagent-public-api-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-campaigns-api-openapi.yml
- filename: icallagent-public-api-contacts-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Contacts API
  slug: icallagent-public-api-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-contacts-api-openapi.yml
- filename: icallagent-public-api-phone-numbers-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Phone Numbers API
  slug: icallagent-public-api-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-phone-numbers-api-openapi.yml
- filename: icallagent-public-api-webhooks-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Webhooks API
  slug: icallagent-public-api-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Icallagent Public Api Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: iCallAgent Public API secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: iCallAgent Public API
provider_slug: icallagent-public-api
scheme_count: 2
schemes:
- bearerFormat: ic_live_<token>
  description: 'Personal API key from Settings → API Keys. Code samples show `Authorization: Bearer <token>` — replace `<token>` with your key (include the word Bearer).'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/icallagent-public-api-openapi.json
  type: http
- description: OAuth2 access token from the consent flow third-party apps go through (see /oauth/authorize/). Interchangeable with a personal API key on every operation below — both are sent as a Bearer token in the same header.
  flows:
  - authorizationUrl: /oauth/authorize/
    flow: authorizationCode
    scopes: 3
    tokenUrl: /oauth/token/
  name: oauth2
  sources:
  - openapi/icallagent-public-api-openapi.json
  type: oauth2
slug: icallagent-public-api-authentication
source_filename: icallagent-public-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: searched\nsource: openapi/icallagent-public-api-openapi.json\ndocs: https://docs.icallagent.com/api-reference/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ic_live_<token>\n  description: 'Personal API key from Settings → API Keys. Code samples show `Authorization:\n    Bearer <token>` — replace `<token>` with your key (include the word Bearer).'\n  sources:\n  - openapi/icallagent-public-api-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize/\n    tokenUrl: /oauth/token/\n    scopes: 3\n  description: OAuth2 access token from the consent flow third-party apps go through (see /oauth/authorize/).\n    Interchangeable with a personal API key on every operation below — both are sent as a Bearer\n    token in the same header.\n  sources:\n  - openapi/icallagent-public-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/authentication/icallagent-public-api-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Voice AI
- voice ai assistant
- Conversational AI
- Voice Agents
- telephony / CPaaS
- contact center / CCaaS
- Outbound Calling
- speech (ASR/TTS)
- agent tools / MCP
---
