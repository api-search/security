---
api_key_in:
- header
api_specs:
- filename: napkin-openapi.yml
  format: yaml
  label: Napkin API
  slug: napkin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/napkin/refs/heads/main/openapi/napkin-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Napkin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Napkin secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Napkin
provider_slug: napkin
scheme_count: 2
schemes:
- description: 'Napkin account API token sent as `Authorization: Bearer YOUR_API_TOKEN`. Create tokens in the web app: app.napkin.ai -> Account/Team Space Settings -> Developers -> "Create new API token". Multiple tokens per account are allowed. API-token auth added in v1.0.0 (2026-01-29).'
  name: bearerAuth
  obtain: https://app.napkin.ai/signin
  scheme: bearer
  sources:
  - openapi/napkin-openapi.yml
  type: http
- description: OAuth 2.0 authorization-code flow for third-party apps acting on behalf of Napkin users. Applications must be approved by Napkin (contact api@napkin.ai) to obtain client credentials.
  flows:
  - authorizationUrl: https://api.napkin.ai/v1/oauth/authorize
    flow: authorizationCode
    revokeUrl: https://api.napkin.ai/v1/oauth/revoke
    scopes:
    - user
    - generation
    tokenUrl: https://api.napkin.ai/v1/oauth/token
  name: oauth2
  sources:
  - openapi/napkin-openapi.yml
  token_lifetimes:
    access_token: 1 hour
    authorization_code: 10 minutes
    refresh_token: 30 days
  type: oauth2
slug: napkin-authentication
source_filename: napkin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.napkin.ai/oauth-user-authentication\ndocs: https://api.napkin.ai/api/napkin-api-documentation\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Napkin account API token sent as `Authorization: Bearer YOUR_API_TOKEN`. Create tokens in\n      the web app: app.napkin.ai -> Account/Team Space Settings -> Developers -> \"Create new API\n      token\". Multiple tokens per account are allowed. API-token auth added in v1.0.0 (2026-01-29).\n    obtain: https://app.napkin.ai/signin\n    sources: [openapi/napkin-openapi.yml]\n  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 authorization-code flow for third-party apps acting on behalf of Napkin users.\n      Applications must be approved by Napkin (contact api@napkin.ai) to obtain client\
  \ credentials.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.napkin.ai/v1/oauth/authorize\n        tokenUrl: https://api.napkin.ai/v1/oauth/token\n        revokeUrl: https://api.napkin.ai/v1/oauth/revoke\n        scopes: [user, generation]\n    token_lifetimes:\n      access_token: 1 hour\n      refresh_token: 30 days\n      authorization_code: 10 minutes\n    sources: [openapi/napkin-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/napkin/refs/heads/main/authentication/napkin-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Ai
- Visualization
- Diagrams
- Infographics
- Presentations
- Content Generation
- Developer API
- Design
---
