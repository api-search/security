---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hover Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: HOVER secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: HOVER
provider_slug: hover
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://hover.to/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://hover.to/oauth/token
    tokenUrl: https://hover.to/oauth/token
  levels:
  - user
  - org
  name: OAuth2
  org_level_note: Some endpoints, when used with org-level OAuth 2.0, require a params[current_user_email] or params[current_user_id] value or a 422 may be returned.
  token:
    access_token_note: An access token is valid for 2 hours and must be refreshed.
    access_token_ttl: 2h
    refresh_token_note: A refresh token is valid indefinitely but invalidates when it is exchanged for a new access token / refresh token combination.
  type: oauth2
slug: hover-authentication
source_filename: hover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.hover.to/docs/oauth-20-authentication\ndocs: https://developers.hover.to/docs/oauth-20-authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, refreshToken]\n  api_key_in: []\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://hover.to/oauth/authorize\n        tokenUrl: https://hover.to/oauth/token\n        refreshUrl: https://hover.to/oauth/token\n    token:\n      access_token_ttl: 2h\n      access_token_note: An access token is valid for 2 hours and must be refreshed.\n      refresh_token_note: >-\n        A refresh token is valid indefinitely but invalidates when it is\n        exchanged for a new access token / refresh token combination.\n    levels:\n      - user\n      - org\n    org_level_note: >-\n      Some endpoints, when used with org-level OAuth 2.0, require a\n      params[current_user_email] or\
  \ params[current_user_id] value or a 422 may\n      be returned.\nscopes_documented: false\nscopes_note: >-\n  Hover's public OAuth documentation does not enumerate granular scopes; access\n  is governed at the user/organization level.\nmcp_auth: https://developers.hover.to/docs/authentication-for-mcp-use\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hover/refs/heads/main/authentication/hover-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Enterprise
- Construction
- Roofing
- Insurance
- 3D Modeling
- Property Data
- Measurements
- Home Services
- Geospatial
---
