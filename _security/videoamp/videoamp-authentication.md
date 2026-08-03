---
api_key_in: []
api_specs:
- filename: videoamp-public-api-openapi.yml
  format: yaml
  label: VideoAmp Public API
  slug: videoamp-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-public-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Videoamp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceAuthorization
overview: VideoAmp secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceAuthorization flow(s).
provider_name: VideoAmp
provider_slug: videoamp
scheme_count: 1
schemes:
- description: OAuth 2.0 / OIDC via VideoAmp's Auth0 tenant at https://login.videoamp.com. Verified from https://login.videoamp.com/.well-known/openid-configuration (HTTP 200) and https://api.videoamp.dev/.well-known/oauth-protected-resource/v1/mcp (HTTP 200, RFC 9728). Bearer tokens are presented in the Authorization header.
  flows:
  - authorizationUrl: https://login.videoamp.com/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://login.videoamp.com/oauth/token
  - flow: deviceAuthorization
    scopes: 4
    tokenUrl: https://login.videoamp.com/oauth/token
  name: videoampOAuth
  sources:
  - openapi/videoamp-public-api-openapi.yml
  type: oauth2
slug: videoamp-authentication
source_filename: videoamp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/videoamp-public-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - deviceAuthorization\nschemes:\n- name: videoampOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.videoamp.com/authorize\n    tokenUrl: https://login.videoamp.com/oauth/token\n    scopes: 4\n  - flow: deviceAuthorization\n    tokenUrl: https://login.videoamp.com/oauth/token\n    scopes: 4\n  description: OAuth 2.0 / OIDC via VideoAmp's Auth0 tenant at https://login.videoamp.com. Verified\n    from https://login.videoamp.com/.well-known/openid-configuration (HTTP 200) and https://api.videoamp.dev/.well-known/oauth-protected-resource/v1/mcp\n    (HTTP 200, RFC 9728). Bearer tokens are presented in the Authorization header.\n  sources:\n  - openapi/videoamp-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/authentication/videoamp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- media-measurement
- advertising
- adtech
- tv-currency
- audience-measurement
- media-planning
- streaming
- attribution
- data-collaboration
- mcp
- agent-native
---
