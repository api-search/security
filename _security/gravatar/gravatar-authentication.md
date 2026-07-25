---
api_key_in: []
api_specs:
- filename: gravatar-avatars-api-openapi.yml
  format: yaml
  label: Gravatar avatars API
  slug: gravatar-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gravatar/refs/heads/main/openapi/gravatar-avatars-api-openapi.yml
- filename: gravatar-experimental-api-openapi.yml
  format: yaml
  label: Gravatar experimental API
  slug: gravatar-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gravatar/refs/heads/main/openapi/gravatar-experimental-api-openapi.yml
- filename: gravatar-profiles-api-openapi.yml
  format: yaml
  label: Gravatar profiles API
  slug: gravatar-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gravatar/refs/heads/main/openapi/gravatar-profiles-api-openapi.yml
- filename: gravatar-qr-code-api-openapi.yml
  format: yaml
  label: Gravatar qr-code API
  slug: gravatar-qr-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gravatar/refs/heads/main/openapi/gravatar-qr-code-api-openapi.yml
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
