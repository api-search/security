---
api_key_in: []
api_specs:
- filename: shapeways-openapi.yml
  format: yaml
  label: Shapeways API
  slug: shapeways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeways/refs/heads/main/openapi/shapeways-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Shapeways Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Shapeways secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Shapeways
provider_slug: shapeways
scheme_count: 1
schemes:
- description: OAuth 2.0. Single-account apps (the app owner's own account) use the client_credentials grant with a Client ID + Client Secret obtained from the Manage Apps dashboard. Apps acting on behalf of other Shapeways users use the authorization_code grant with a redirect_uri, then exchange the returned code for an access token; the refresh_token grant renews expired access tokens. Access tokens are bearer tokens with expires_in 3600.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.shapeways.com/oauth2/token
  - authorizationUrl: https://api.shapeways.com/oauth2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.shapeways.com/oauth2/token
  name: oauth2
  sources:
  - openapi/shapeways-openapi.yml
  type: oauth2
slug: shapeways-authentication
source_filename: shapeways-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.shapeways.com/getting-started\ndocs: https://developers.shapeways.com/getting-started\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  token_type: bearer\n  token_ttl_seconds: 3600\nschemes:\n  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0. Single-account apps (the app owner's own account) use the\n      client_credentials grant with a Client ID + Client Secret obtained from\n      the Manage Apps dashboard. Apps acting on behalf of other Shapeways users\n      use the authorization_code grant with a redirect_uri, then exchange the\n      returned code for an access token; the refresh_token grant renews expired\n      access tokens. Access tokens are bearer tokens with expires_in 3600.\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.shapeways.com/oauth2/token\n        scopes: 0\n      - flow: authorizationCode\n  \
  \      authorizationUrl: https://api.shapeways.com/oauth2/authorize\n        tokenUrl: https://api.shapeways.com/oauth2/token\n        scopes: 0\n    sources: [openapi/shapeways-openapi.yml]\napp_management: https://developers.shapeways.com/manage-apps\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shapeways/refs/heads/main/authentication/shapeways-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- 3D Printing
- Additive Manufacturing
- Manufacturing
- Prototyping
- Hardware
- Fulfillment
- eCommerce
---
