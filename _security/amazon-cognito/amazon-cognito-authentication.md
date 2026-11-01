---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-cognito-amazon-cognito-identity-api-openapi.yml
  format: yaml
  label: Amazon Cognito Amazon Cognito Identity API
  slug: amazon-cognito-amazon-cognito-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cognito/openapi/amazon-cognito-amazon-cognito-identity-api-openapi.yml
- filename: amazon-cognito-amazon-cognito-identity-provider-api-openapi.yml
  format: yaml
  label: Amazon Cognito Amazon Cognito Identity Provider API
  slug: amazon-cognito-amazon-cognito-identity-provider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cognito/openapi/amazon-cognito-amazon-cognito-identity-provider-api-openapi.yml
- filename: amazon-cognito-managed-login-branding-api-openapi.yml
  format: yaml
  label: Amazon Cognito Cognito Managed Login Branding API
  slug: amazon-cognito-managed-login-branding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cognito/openapi/amazon-cognito-managed-login-branding-api-openapi.yml
- filename: amazon-cognito-operations-api-openapi.yml
  format: yaml
  label: Amazon Cognito Cognito Operations API
  slug: amazon-cognito-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cognito/openapi/amazon-cognito-operations-api-openapi.yml
- filename: amazon-cognito-term-api-openapi.yml
  format: yaml
  label: Amazon Cognito Cognito Term API
  slug: amazon-cognito-term-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cognito/openapi/amazon-cognito-term-api-openapi.yml
- filename: amazon-cognito-user-pool-client-secret-api-openapi.yml
  format: yaml
  label: Amazon Cognito Cognito User Pool Client Secret API
  slug: amazon-cognito-user-pool-client-secret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cognito/openapi/amazon-cognito-user-pool-client-secret-api-openapi.yml
- filename: amazon-cognito-user-pool-replica-api-openapi.yml
  format: yaml
  label: Amazon Cognito Cognito User Pool Replica API
  slug: amazon-cognito-user-pool-replica-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cognito/openapi/amazon-cognito-user-pool-replica-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/amazon-cognito/authentication/amazon-cognito-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Authentication
- Identity
- OpenID Connect
- SAML
- User Management
- Federated Identity
- Identity Federation
---
