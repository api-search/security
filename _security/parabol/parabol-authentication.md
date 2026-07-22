---
api_key_in:
- header
api_specs:
- filename: parabol-graphql-subscriptions-asyncapi.yml
  format: yaml
  label: Parabol GraphQL API
  slug: parabol-graphql-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/parabol/refs/heads/main/asyncapi/parabol-graphql-subscriptions-asyncapi.yml
auth_types:
- http-bearer
- personal-access-token
description: ''
kind: authentication
layout: security
method: searched
name: Parabol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parabol secures its APIs with http-bearer and personal-access-token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Parabol
provider_slug: parabol
scheme_count: 1
schemes:
- bearerFormat: PAT
  create_url: https://action.parabol.co/me/profile
  header: Authorization
  in: header
  name: PersonalAccessToken
  scheme: bearer
  scoped: true
  scopes_ref: scopes/parabol-scopes.yml
  sources:
  - graphql/parabol-schema.graphql
  type: http
slug: parabol-authentication
source_filename: parabol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://raw.githubusercontent.com/ParabolInc/parabol/master/llms.txt\ndocs: https://www.parabol.co/friday-ship/introducing-the-parabol-api/\nsummary:\n  types: [http-bearer, personal-access-token]\n  api_key_in: [header]\n  token_scoped: true\n  oauth2_flows: []\n  notes: >-\n    Parabol's public GraphQL API authenticates with scoped Personal Access\n    Tokens (PATs) passed as an HTTP Bearer token in the Authorization header.\n    Tokens are least-privilege: an integration requests only the scopes it\n    needs, enforced in the schema by a @scope(name: OAuthScopeEnum!) directive\n    (252 field applications). Regular first-party sessions use a JWT for which\n    the @scope directive is a no-op. Full OAuth 2.0 authorization-code support\n    is on the published roadmap but not yet available.\nschemes:\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: PAT\n  in: header\n  header: Authorization\n \
  \ create_url: https://action.parabol.co/me/profile\n  scoped: true\n  scopes_ref: scopes/parabol-scopes.yml\n  sources: [graphql/parabol-schema.graphql]\nroadmap:\n- oauth2 authorization-code (planned, per API launch announcement)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parabol/refs/heads/main/authentication/parabol-authentication.yml
summary_line: http-bearer/personal-access-token · 1 scheme
tags:
- Company
- Developer Tools
- Agile
- Retrospectives
- Meetings
- Collaboration
- GraphQL
- Team Productivity
- Open Source
---
