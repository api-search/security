---
api_key_in: []
api_specs:
- filename: blng-journey-api-openapi.yml
  format: yaml
  label: BLNG Journey API
  slug: blng-journey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-journey-api-openapi.yml
- filename: blng-user-api-openapi.yml
  format: yaml
  label: BLNG User API
  slug: blng-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-user-api-openapi.yml
- filename: blng-billing-api-openapi.yml
  format: yaml
  label: BLNG Billing API
  slug: blng-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/openapi/blng-billing-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Blng Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Blng secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Blng
provider_slug: blng
scheme_count: 2
schemes:
- description: Cognito authorization code flow for users
  flows:
  - authorizationUrl: https://auth.app.blng.ai/oauth2/authorize
    flow: implicit
    scopes: 4
  name: cognitoUserAuth
  sources:
  - openapi/blng-billing-api-openapi.yml
  - openapi/blng-journey-api-openapi.yml
  - openapi/blng-user-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  description: "Use your Cognito \"access_token\" or \"id_token\" obtained from AWS Cognito Hosted UI \nor CLI. Click \"Authorize\" and paste the token."
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/blng-journey-api-openapi.yml
  - openapi/blng-user-api-openapi.yml
  type: http
slug: blng-authentication
source_filename: blng-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/blng-billing-api-openapi.yml, openapi/blng-journey-api-openapi.yml, openapi/blng-user-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: cognitoUserAuth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://auth.app.blng.ai/oauth2/authorize\n    scopes: 4\n  description: Cognito authorization code flow for users\n  sources:\n  - openapi/blng-billing-api-openapi.yml\n  - openapi/blng-journey-api-openapi.yml\n  - openapi/blng-user-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: \"Use your Cognito \\\"access_token\\\" or \\\"id_token\\\" obtained from AWS Cognito\\\n    \\ Hosted UI \\nor CLI. Click \\\"Authorize\\\" and paste the token.\"\n  sources:\n  - openapi/blng-journey-api-openapi.yml\n  - openapi/blng-user-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blng/refs/heads/main/authentication/blng-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Jewelry
- Generative AI
- Design
- Creative Tools
- Rendering
- Marketing
- Retail
- 3D Models
- Image-Generation
- Workspaces
- Billing
- OpenAPI
- AWS Cognito
---
