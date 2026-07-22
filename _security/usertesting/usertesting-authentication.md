---
api_key_in: []
api_specs:
- filename: usertesting-results-v2-openapi.yml
  format: yaml
  label: UserTesting Results API (v2)
  slug: usertesting-results-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-results-v2-openapi.yml
- filename: usertesting-legacy-v1-openapi.yml
  format: yaml
  label: UserTesting Legacy API (v1)
  slug: usertesting-legacy-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-legacy-v1-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Usertesting Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: UserTesting secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: UserTesting
provider_slug: usertesting
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Go to [Authorization](https://developer.usertesting.com/v1.0/docs/authentication-authorization) for information on how to generate an access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/usertesting-legacy-v1-openapi.yml
  - openapi/usertesting-results-v2-openapi.yml
  type: http
- description: Documented token flow behind bearerAuth (the OpenAPI models only the resulting bearer token). Client credentials (client_id + client_secret) are issued per registered API user by support@usertesting.com; the same token works on both Legacy (v1) and Results (v2) endpoints. Access tokens are JWTs that expire after 3600 seconds. The Okta authorization server publishes RFC 8414 / OIDC discovery metadata (saved under well-known/).
  flows:
  - flow: clientCredentials
    scopes:
      studies:read: Read access to study/test result data
    tokenUrl: https://auth.usertesting.com/oauth2/aus1p3vtd8vtm4Bxv0h8/v1/token
  name: oauth2ClientCredentials
  sources:
  - https://developer.usertesting.com/docs/authorization
  - well-known/usertesting-oauth-authorization-server.json
  type: oauth2
slug: usertesting-authentication
source_filename: usertesting-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/usertesting-legacy-v1-openapi.yml, openapi/usertesting-results-v2-openapi.yml\ndocs: https://developer.usertesting.com/docs/authorization\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Go to [Authorization](https://developer.usertesting.com/v1.0/docs/authentication-authorization)\n    for information on how to generate an access token.\n  sources:\n  - openapi/usertesting-legacy-v1-openapi.yml\n  - openapi/usertesting-results-v2-openapi.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  description: >-\n    Documented token flow behind bearerAuth (the OpenAPI models only the resulting bearer\n    token). Client credentials (client_id + client_secret) are issued per registered API user\n    by support@usertesting.com; the same token works on both Legacy (v1) and Results (v2)\n   \
  \ endpoints. Access tokens are JWTs that expire after 3600 seconds. The Okta authorization\n    server publishes RFC 8414 / OIDC discovery metadata (saved under well-known/).\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.usertesting.com/oauth2/aus1p3vtd8vtm4Bxv0h8/v1/token\n    scopes:\n      studies:read: Read access to study/test result data\n  sources:\n  - https://developer.usertesting.com/docs/authorization\n  - well-known/usertesting-oauth-authorization-server.json\nnotes:\n- 'Request header: Authorization: Bearer ACCESS_TOKEN on every API call.'\n- 'Token request: POST x-www-form-urlencoded with grant_type=client_credentials, client_id,\n  client_secret, scope=studies:read.'\n- API access is scoped to the workspaces where the registered email is a team member.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/authentication/usertesting-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- UX Research
- Usability Testing
- Human Insight
- Customer Experience
- Surveys
- Video
- Transcripts
- Experience Metrics
---
