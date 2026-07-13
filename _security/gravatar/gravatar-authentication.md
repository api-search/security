---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: Gravatar Avatar API
  slug: avatar-api
  spec_type: OpenAPI
  url: https://api.gravatar.com/v3/openapi
- filename: openapi
  format: yaml
  label: Gravatar REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://api.gravatar.com/v3/openapi
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Gravatar Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Gravatar secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Gravatar
provider_slug: gravatar
scheme_count: 2
schemes:
- description: Bearer token to authenticate the request. Full profile information is only available in authenticated requests.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
- description: WordPress OAuth token to authenticate the request.
  flows:
  - authorizationUrl: https://public-api.wordpress.com/oauth2/authorize
    flow: implicit
    scopes: 0
  name: oauth
  sources:
  - openapi/openapi.json
  type: oauth2
slug: gravatar-authentication
source_filename: gravatar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Bearer token to authenticate the request. Full profile information is only available\n    in authenticated requests.\n  sources:\n  - openapi/openapi.json\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://public-api.wordpress.com/oauth2/authorize\n    scopes: 0\n  description: WordPress OAuth token to authenticate the request.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gravatar/refs/heads/main/authentication/gravatar-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Avatars
- Identity
- Profiles
- Social
- Images
- GraphQL
- REST
---
