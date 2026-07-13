---
api_key_in:
- header
api_specs:
- filename: aws-cognito-identity-provider-openapi.yaml
  format: yaml
  label: Amazon Cognito Identity Provider
  slug: aws-cognito-identity-provider
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/openapi/aws-cognito-identity-provider-openapi.yaml
- filename: aws-cognito-identity-openapi.yaml
  format: yaml
  label: Amazon Cognito Identity (Federated Identities)
  slug: aws-cognito-identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/openapi/aws-cognito-identity-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aws Cognito Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Cognito secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Cognito
provider_slug: aws-cognito
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/aws-cognito-identity-openapi.yaml
  - openapi/aws-cognito-identity-provider-openapi.yaml
  type: apiKey
slug: aws-cognito-authentication
source_filename: aws-cognito-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aws-cognito-identity-openapi.yaml, openapi/aws-cognito-identity-provider-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/aws-cognito-identity-openapi.yaml\n  - openapi/aws-cognito-identity-provider-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/authentication/aws-cognito-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
---
