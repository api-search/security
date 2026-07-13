---
api_key_in: []
api_specs:
- filename: trainerize-openapi.yml
  format: yaml
  label: ABC Trainerize Clients API
  slug: trainerize-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-openapi.yml
- filename: trainerize-openapi.yml
  format: yaml
  label: ABC Trainerize Training Programs API
  slug: trainerize-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-openapi.yml
- filename: trainerize-openapi.yml
  format: yaml
  label: ABC Trainerize Client Data API
  slug: trainerize-client-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-openapi.yml
- filename: trainerize-openapi.yml
  format: yaml
  label: ABC Trainerize Messaging API
  slug: trainerize-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-openapi.yml
- filename: trainerize-openapi.yml
  format: yaml
  label: ABC Trainerize Webhooks API
  slug: trainerize-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Trainerize Authentication
name_suffix: Authentication
oauth_flows: []
overview: ABC Trainerize secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ABC Trainerize
provider_slug: trainerize
scheme_count: 2
schemes:
- description: API key provisioned from the ABC Trainerize account settings. API access is limited to Studio and Enterprise plans. Passed as an Authorization header credential. The exact header format is documented only in the gated ABC Trainerize help center; modeled here as an Authorization header key.
  header: Authorization
  in: header
  name: apiKey
  sources:
  - https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize
  - https://apitracker.io/a/trainerize
  type: apiKey
- description: OAuth2 connection offered for partner integrations, obtained from the Trainerize settings alongside the API key option. Grant flow and scope details are behind the gated help center and were not publicly confirmable.
  name: oauth2
  sources:
  - https://apitracker.io/a/trainerize
  type: oauth2
slug: trainerize-authentication
source_filename: trainerize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/trainerize-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  header: Authorization\n  description: >-\n    API key provisioned from the ABC Trainerize account settings. API access is\n    limited to Studio and Enterprise plans. Passed as an Authorization header\n    credential. The exact header format is documented only in the gated ABC\n    Trainerize help center; modeled here as an Authorization header key.\n  sources:\n  - https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize\n  - https://apitracker.io/a/trainerize\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth2 connection offered for partner integrations, obtained from the\n    Trainerize settings alongside the API key option. Grant flow and scope\n    details are behind the gated help center and were not publicly confirmable.\n  sources:\n\
  \  - https://apitracker.io/a/trainerize\nnotes: >-\n  Trainerize's API is partner / private, not open self-serve: credentials are\n  provisioned per business (Studio/Enterprise), and ABC Trainerize support does\n  not assist with building API calls. Auth type is confirmed (API key and OAuth2);\n  the precise header name/format and OAuth endpoints are modeled because the full\n  reference is authenticated.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/authentication/trainerize-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Fitness
- Personal Training
- Coaching
- Fitness Software
- Client Management
- SaaS
---
