---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-signer-signing-jobs-api-openapi.yml
  format: yaml
  label: Amazon Signer Signing Jobs API
  slug: amazon-signer-signing-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-signer/openapi/amazon-signer-signing-jobs-api-openapi.yml
- filename: amazon-signer-signing-platforms-api-openapi.yml
  format: yaml
  label: Amazon Signer Signing Platforms API
  slug: amazon-signer-signing-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-signer/openapi/amazon-signer-signing-platforms-api-openapi.yml
- filename: amazon-signer-signing-profiles-api-openapi.yml
  format: yaml
  label: Amazon Signer Signing Profiles API
  slug: amazon-signer-signing-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-signer/openapi/amazon-signer-signing-profiles-api-openapi.yml
- filename: amazon-signer-tags-api-openapi.yml
  format: yaml
  label: Amazon Signer Tags API
  slug: amazon-signer-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-signer/openapi/amazon-signer-tags-api-openapi.yml
- filename: amazon-signer-revocations-api-openapi.yml
  format: yaml
  label: Amazon Signer Revocations API
  slug: amazon-signer-revocations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-signer/openapi/amazon-signer-revocations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Signer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Signer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Signer
provider_slug: amazon-signer
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-signer-revocations-api-openapi.yml
  - openapi/amazon-signer-signing-jobs-api-openapi.yml
  - openapi/amazon-signer-signing-platforms-api-openapi.yml
  - openapi/amazon-signer-signing-profiles-api-openapi.yml
  - openapi/amazon-signer-tags-api-openapi.yml
  type: apiKey
slug: amazon-signer-authentication
source_filename: amazon-signer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-signer-revocations-api-openapi.yml, openapi/amazon-signer-signing-jobs-api-openapi.yml,\n  openapi/amazon-signer-signing-platforms-api-openapi.yml, openapi/amazon-signer-signing-profiles-api-openapi.yml,\n  openapi/amazon-signer-tags-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-signer-revocations-api-openapi.yml\n  - openapi/amazon-signer-signing-jobs-api-openapi.yml\n  - openapi/amazon-signer-signing-platforms-api-openapi.yml\n  - openapi/amazon-signer-signing-profiles-api-openapi.yml\n  - openapi/amazon-signer-tags-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-signer/authentication/amazon-signer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Code Signing
- IoT
- Lambda
- Security
---
