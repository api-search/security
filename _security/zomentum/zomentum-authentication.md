---
api_key_in: []
api_specs:
- filename: api-docs.zomentum.com
  format: yaml
  label: Zomentum API
  slug: zomentum-api
  spec_type: Postman
  url: https://api-docs.zomentum.com
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zomentum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zomentum secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zomentum
provider_slug: zomentum
scheme_count: 2
schemes:
- description: 'Access token issued to an API User, sent as `Authorization: Bearer <token>`. Renewed with the refresh token via the Refresh Token API.'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://help.zomentum.com/support/solutions/articles/44002337023-generating-an-api-user
  type: http
- description: 'Auth0 tenant acts as Zomentum''s authorization server (confirmed on status.zomentum.com: user authentication, MFA, and Management API). Access and refresh tokens presented to the API are Auth0-issued bearer tokens.'
  name: Auth0
  sources:
  - https://status.zomentum.com
  type: oauth2
slug: zomentum-authentication
source_filename: zomentum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://help.zomentum.com/support/solutions/articles/44002337023-generating-an-api-user\ndocs: https://api-docs.zomentum.com\nnotes: >-\n  Zomentum's REST API uses Bearer token authentication. An administrator creates\n  an \"API User\" in the dashboard Settings (with scoped permissions) and generates\n  an access token and a refresh token; the access token is sent as an\n  Authorization: Bearer <token> header and renewed via the Refresh Token API.\n  The status page lists an Auth0 authorization server (user authentication, MFA,\n  Management API) as the identity provider behind these tokens. API access is\n  available on the Growth plan tier.\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_provider: Auth0\n  token_lifecycle:\n  - access_token\n  - refresh_token\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Access token issued to an API User, sent as `Authorization:\
  \ Bearer <token>`.\n    Renewed with the refresh token via the Refresh Token API.\n  sources:\n  - https://help.zomentum.com/support/solutions/articles/44002337023-generating-an-api-user\n- name: Auth0\n  type: oauth2\n  description: >-\n    Auth0 tenant acts as Zomentum's authorization server (confirmed on\n    status.zomentum.com: user authentication, MFA, and Management API). Access\n    and refresh tokens presented to the API are Auth0-issued bearer tokens.\n  sources:\n  - https://status.zomentum.com\nprovisioning:\n  api_user: dashboard Settings -> API User (scoped permissions)\n  plan_required: Growth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zomentum/refs/heads/main/authentication/zomentum-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Enterprise
- MSP
- CRM
- Sales
- Proposals
- Payments
- Revenue Platform
- PSA Integration
---
