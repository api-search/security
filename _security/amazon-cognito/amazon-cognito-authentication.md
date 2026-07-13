---
api_key_in:
- header
api_specs:
- filename: amazon-cognito-user-pools-openapi.yml
  format: yaml
  label: Amazon Cognito User Pools API
  slug: user-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/openapi/amazon-cognito-user-pools-openapi.yml
- filename: amazon-cognito-identity-pools-openapi.yml
  format: yaml
  label: Amazon Cognito Identity Pools API
  slug: identity-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/openapi/amazon-cognito-identity-pools-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Cognito Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Cognito secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Cognito
provider_slug: amazon-cognito
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-cognito-identity-pools-openapi.yml
  - openapi/amazon-cognito-user-pools-openapi.yml
  type: apiKey
slug: amazon-cognito-authentication
source_filename: amazon-cognito-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-cognito-identity-pools-openapi.yml, openapi/amazon-cognito-user-pools-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-cognito-identity-pools-openapi.yml\n  - openapi/amazon-cognito-user-pools-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/authentication/amazon-cognito-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Authentication
- Identity
- OAuth
- OIDC
- SAML
- User Management
- Federated Identity
---
