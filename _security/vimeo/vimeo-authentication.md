---
api_key_in: []
api_specs:
- filename: api.yaml
  format: yaml
  label: Vimeo API
  slug: rest-api
  spec_type: OpenAPI
  url: https://github.com/vimeo/openapi/blob/master/api.yaml
- filename: vimeo-asyncapi.yml
  format: yaml
  label: Vimeo Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/vimeo/refs/heads/main/openapi/vimeo-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Vimeo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Vimeo secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Vimeo
provider_slug: vimeo
scheme_count: 2
schemes:
- description: OAuth 2.0 Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vimeo-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://api.vimeo.com/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.vimeo.com/oauth/access_token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.vimeo.com/oauth/authorize/client
  name: oauth2
  sources:
  - openapi/vimeo-openapi.yml
  type: oauth2
slug: vimeo-authentication
source_filename: vimeo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vimeo-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token\n  sources:\n  - openapi/vimeo-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.vimeo.com/oauth/authorize\n    tokenUrl: https://api.vimeo.com/oauth/access_token\n    scopes: 6\n  - flow: clientCredentials\n    tokenUrl: https://api.vimeo.com/oauth/authorize/client\n    scopes: 1\n  sources:\n  - openapi/vimeo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vimeo/refs/heads/main/authentication/vimeo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Video
- Streaming
- Video Hosting
- Live Streaming
- Media
- OTT
---
