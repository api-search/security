---
api_key_in:
- header
api_specs:
- filename: teachable-admin-openapi.yml
  format: yaml
  label: Teachable Admin API
  slug: teachable-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-admin-openapi.yml
- filename: teachable-oauth-openapi.yml
  format: yaml
  label: Teachable OAuth API
  slug: teachable-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-oauth-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Teachable Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Teachable secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Teachable
provider_slug: teachable
scheme_count: 3
schemes:
- description: API key for Admin API authentication. Available on Growth plan and above.
  in: header
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/teachable-admin-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://developers.teachable.com/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://developers.teachable.com/oauth/token
  name: OAuth2
  sources:
  - openapi/teachable-oauth-openapi.yml
  type: oauth2
- description: Bearer access token for OAuth authenticated requests.
  in: header
  name: AccessToken
  parameter: Authorization
  sources:
  - openapi/teachable-oauth-openapi.yml
  type: apiKey
slug: teachable-authentication
source_filename: teachable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teachable-admin-openapi.yml, openapi/teachable-oauth-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: API key for Admin API authentication. Available on Growth plan and above.\n  sources:\n  - openapi/teachable-admin-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://developers.teachable.com/oauth/authorize\n    tokenUrl: https://developers.teachable.com/oauth/token\n    scopes: 4\n  sources:\n  - openapi/teachable-oauth-openapi.yml\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer access token for OAuth authenticated requests.\n  sources:\n  - openapi/teachable-oauth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/authentication/teachable-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Online Courses
- E-Learning
- Education
- Course Management
- Enrollments
- Coaching
- Memberships
- Transactions
---
