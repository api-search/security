---
api_key_in:
- header
api_specs:
- filename: amazon-iam-identity-center-sso-admin-openapi-original.yml
  format: yaml
  label: AWS IAM Identity Center SSO Admin API
  slug: aws-sso-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/openapi/amazon-iam-identity-center-sso-admin-openapi-original.yml
- filename: amazon-iam-identity-center-identitystore-openapi-original.yml
  format: yaml
  label: AWS IAM Identity Center Identity Store API
  slug: aws-identitystore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/openapi/amazon-iam-identity-center-identitystore-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Iam Identity Center Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon IAM Identity Center secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-iam-identity-center-identitystore-openapi-original.yml
  - openapi/amazon-iam-identity-center-sso-admin-openapi-original.yml
  type: apiKey
slug: amazon-iam-identity-center-authentication
source_filename: amazon-iam-identity-center-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-iam-identity-center-identitystore-openapi-original.yml, openapi/amazon-iam-identity-center-sso-admin-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-iam-identity-center-identitystore-openapi-original.yml\n  - openapi/amazon-iam-identity-center-sso-admin-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/authentication/amazon-iam-identity-center-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
---
