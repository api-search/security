---
api_key_in: []
api_specs:
- filename: activision-blizzard-battle-net.json
  format: json
  label: Battle.net API
  slug: battle-net
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/openapi/activision-blizzard-battle-net.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Activision Blizzard Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: activision-blizzard secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: activision-blizzard
provider_slug: activision-blizzard
scheme_count: 1
schemes:
- description: OAuth2 authentication. Create a client at develop.battle.net for client ID and secret.
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://oauth.battle.net/token
  - authorizationUrl: https://oauth.battle.net/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth.battle.net/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/activision-blizzard-battle-net.json
  type: oauth2
slug: activision-blizzard-authentication
source_filename: activision-blizzard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/activision-blizzard-battle-net.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.battle.net/token\n    scopes: 3\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.battle.net/authorize\n    tokenUrl: https://oauth.battle.net/token\n    scopes: 3\n  description: OAuth2 authentication. Create a client at develop.battle.net for client ID and\n    secret.\n  sources:\n  - openapi/activision-blizzard-battle-net.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/authentication/activision-blizzard-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fortune 1000
---
