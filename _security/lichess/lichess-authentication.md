---
api_key_in: []
api_specs:
- filename: lichess-openapi.yml
  format: yaml
  label: Lichess API
  slug: lichess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lichess/refs/heads/main/openapi/lichess-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lichess Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lichess secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lichess
provider_slug: lichess
scheme_count: 1
schemes:
- description: Read [the introduction for how to make authenticated requests](#description/authentication).
  flows:
  - authorizationUrl: https://lichess.org/oauth
    flow: authorizationCode
    scopes: 23
    tokenUrl: https://lichess.org/api/token
  name: OAuth2
  sources:
  - openapi/lichess-openapi.yml
  type: oauth2
slug: lichess-authentication
source_filename: lichess-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lichess-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lichess.org/oauth\n    tokenUrl: https://lichess.org/api/token\n    scopes: 23\n  description: Read [the introduction for how to make authenticated requests](#description/authentication).\n  sources:\n  - openapi/lichess-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lichess/refs/heads/main/authentication/lichess-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Chess
- Games
- Open Source
- Nonprofit
- Tournaments
- Puzzles
- Bots
- Streaming
- ND-JSON
- OAuth
---
