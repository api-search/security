---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-iam-identity-center-aws-single-sign-on-admin-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center AWS Single Sign On Admin API
  slug: amazon-iam-identity-center-aws-single-sign-on-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-aws-single-sign-on-admin-api-openapi.yml
- filename: amazon-iam-identity-center-aws-sso-identity-store-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center AWS SSO Identity Store API
  slug: amazon-iam-identity-center-aws-sso-identity-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-aws-sso-identity-store-api-openapi.yml
- filename: amazon-iam-identity-center-application-access-scope-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center Iam Identity Center Application Access Scope API
  slug: amazon-iam-identity-center-application-access-scope-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-application-access-scope-api-openapi.yml
- filename: amazon-iam-identity-center-application-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center Iam Identity Center Application API
  slug: amazon-iam-identity-center-application-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-application-api-openapi.yml
- filename: amazon-iam-identity-center-application-assignment-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center Iam Identity Center Application Assignment API
  slug: amazon-iam-identity-center-application-assignment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-application-assignment-api-openapi.yml
- filename: amazon-iam-identity-center-application-authentication-method-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center Iam Identity Center Application Authentication Method API
  slug: amazon-iam-identity-center-application-authentication-method-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-application-authentication-method-api-openapi.yml
- filename: amazon-iam-identity-center-application-grant-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center Iam Identity Center Application Grant API
  slug: amazon-iam-identity-center-application-grant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-application-grant-api-openapi.yml
- filename: amazon-iam-identity-center-identity-store-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center Iam Identity Center Identity Store API
  slug: amazon-iam-identity-center-identity-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-identity-store-api-openapi.yml
- filename: amazon-iam-identity-center-instance-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center Iam Identity Center Instance API
  slug: amazon-iam-identity-center-instance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-instance-api-openapi.yml
- filename: amazon-iam-identity-center-operations-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center Iam Identity Center Operations API
  slug: amazon-iam-identity-center-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-operations-api-openapi.yml
- filename: amazon-iam-identity-center-region-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center Iam Identity Center Region API
  slug: amazon-iam-identity-center-region-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-region-api-openapi.yml
- filename: amazon-iam-identity-center-trusted-token-issuer-api-openapi.yml
  format: yaml
  label: Amazon IAM Identity Center Iam Identity Center Trusted Token Issuer API
  slug: amazon-iam-identity-center-trusted-token-issuer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-iam-identity-center/openapi/amazon-iam-identity-center-trusted-token-issuer-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon IAM Identity Center Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon IAM Identity Center secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-iam-identity-center-application-access-scope-api-openapi.yml
  - openapi/amazon-iam-identity-center-application-api-openapi.yml
  - openapi/amazon-iam-identity-center-application-assignment-api-openapi.yml
  - openapi/amazon-iam-identity-center-application-authentication-method-api-openapi.yml
  - openapi/amazon-iam-identity-center-application-grant-api-openapi.yml
  - openapi/amazon-iam-identity-center-aws-single-sign-on-admin-api-openapi.yml
  - openapi/amazon-iam-identity-center-aws-sso-identity-store-api-openapi.yml
  - openapi/amazon-iam-identity-center-identity-store-api-openapi.yml
  - openapi/amazon-iam-identity-center-instance-api-openapi.yml
  - openapi/amazon-iam-identity-center-operations-api-openapi.yml
  - openapi/amazon-iam-identity-center-region-api-openapi.yml
  - openapi/amazon-iam-identity-center-trusted-token-issuer-api-openapi.yml
  type: apiKey
slug: amazon-iam-identity-center-authentication
source_filename: amazon-iam-identity-center-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-iam-identity-center-application-access-scope-api-openapi.yml, openapi/amazon-iam-identity-center-application-api-openapi.yml,\n  openapi/amazon-iam-identity-center-application-assignment-api-openapi.yml, openapi/amazon-iam-identity-center-application-authentication-method-api-openapi.yml,\n  openapi/amazon-iam-identity-center-application-grant-api-openapi.yml, openapi/amazon-iam-identity-center-aws-single-sign-on-admin-api-openapi.yml,\n  openapi/amazon-iam-identity-center-aws-sso-identity-store-api-openapi.yml, openapi/amazon-iam-identity-center-identity-store-api-openapi.yml,\n  openapi/amazon-iam-identity-center-instance-api-openapi.yml, openapi/amazon-iam-identity-center-operations-api-openapi.yml,\n  openapi/amazon-iam-identity-center-region-api-openapi.yml, openapi/amazon-iam-identity-center-trusted-token-issuer-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name:\
  \ sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-iam-identity-center-application-access-scope-api-openapi.yml\n  - openapi/amazon-iam-identity-center-application-api-openapi.yml\n  - openapi/amazon-iam-identity-center-application-assignment-api-openapi.yml\n  - openapi/amazon-iam-identity-center-application-authentication-method-api-openapi.yml\n  - openapi/amazon-iam-identity-center-application-grant-api-openapi.yml\n  - openapi/amazon-iam-identity-center-aws-single-sign-on-admin-api-openapi.yml\n  - openapi/amazon-iam-identity-center-aws-sso-identity-store-api-openapi.yml\n  - openapi/amazon-iam-identity-center-identity-store-api-openapi.yml\n  - openapi/amazon-iam-identity-center-instance-api-openapi.yml\n\
  \  - openapi/amazon-iam-identity-center-operations-api-openapi.yml\n  - openapi/amazon-iam-identity-center-region-api-openapi.yml\n  - openapi/amazon-iam-identity-center-trusted-token-issuer-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-iam-identity-center/authentication/amazon-iam-identity-center-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Access Control
- Authentication
- Amazon Web Services
- Identity and Access Management
- SSO
---
