---
api_key_in: []
api_specs:
- filename: tripleseat-openapi.yml
  format: yaml
  label: Tripleseat API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/openapi/tripleseat-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tripleseat Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Tripleseat secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Tripleseat
provider_slug: tripleseat
scheme_count: 1
schemes:
- description: OAuth 2.0. Access tokens are Bearer tokens that expire after 7200 seconds (2 hours) and are accompanied by a refresh token. OAuth 1.0 is deprecated and discontinued on July 1, 2026.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.tripleseat.com/oauth/token
  - authorizationUrl: https://api.tripleseat.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://api.tripleseat.com/oauth/token
  name: oauth2
  sources:
  - openapi/tripleseat-openapi.yml
  type: oauth2
slug: tripleseat-authentication
source_filename: tripleseat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tripleseat-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.tripleseat.com/oauth/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: https://api.tripleseat.com/oauth/authorize\n    tokenUrl: https://api.tripleseat.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0. Access tokens are Bearer tokens that expire after 7200 seconds (2\n    hours) and are accompanied by a refresh token. OAuth 1.0 is deprecated and discontinued\n    on July 1, 2026.\n  sources:\n  - openapi/tripleseat-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/authentication/tripleseat-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Restaurant
- Events
- Catering
- Leads
- Webhooks
- Sales
---
