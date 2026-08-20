---
api_key_in:
- header
api_specs:
- filename: teachable-courses-api-openapi.yml
  format: yaml
  label: Teachable Courses API
  slug: teachable-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-courses-api-openapi.yml
- filename: teachable-currentuser-api-openapi.yml
  format: yaml
  label: Teachable CurrentUser API
  slug: teachable-currentuser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-currentuser-api-openapi.yml
- filename: teachable-enrollments-api-openapi.yml
  format: yaml
  label: Teachable Enrollments API
  slug: teachable-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-enrollments-api-openapi.yml
- filename: teachable-lectures-api-openapi.yml
  format: yaml
  label: Teachable Lectures API
  slug: teachable-lectures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-lectures-api-openapi.yml
- filename: teachable-pricingplans-api-openapi.yml
  format: yaml
  label: Teachable PricingPlans API
  slug: teachable-pricingplans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-pricingplans-api-openapi.yml
- filename: teachable-quizzes-api-openapi.yml
  format: yaml
  label: Teachable Quizzes API
  slug: teachable-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-quizzes-api-openapi.yml
- filename: teachable-transactions-api-openapi.yml
  format: yaml
  label: Teachable Transactions API
  slug: teachable-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-transactions-api-openapi.yml
- filename: teachable-users-api-openapi.yml
  format: yaml
  label: Teachable Users API
  slug: teachable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-users-api-openapi.yml
- filename: teachable-videos-api-openapi.yml
  format: yaml
  label: Teachable Videos API
  slug: teachable-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-videos-api-openapi.yml
- filename: teachable-webhooks-api-openapi.yml
  format: yaml
  label: Teachable Webhooks API
  slug: teachable-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-webhooks-api-openapi.yml
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
- Transaction
---
