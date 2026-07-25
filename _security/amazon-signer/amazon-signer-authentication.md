---
api_key_in:
- header
api_specs:
- filename: amazon-signer-revocations-signaturetimestamp-platformid-profileversionarn-jobarn-certificatehashes-api-openapi.yml
  format: yaml
  label: Amazon Signer Revocations#signatureTimestamp&platformId&profileVersionArn&jobArn&certificateHashes API
  slug: amazon-signer-revocations-signaturetimestamp-platformid-profileversionarn-jobarn-certificatehashes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/openapi/amazon-signer-revocations-signaturetimestamp-platformid-profileversionarn-jobarn-certificatehashes-api-openapi.yml
- filename: amazon-signer-signing-jobs-api-openapi.yml
  format: yaml
  label: Amazon Signer Signing Jobs API
  slug: amazon-signer-signing-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/openapi/amazon-signer-signing-jobs-api-openapi.yml
- filename: amazon-signer-signing-platforms-api-openapi.yml
  format: yaml
  label: Amazon Signer Signing Platforms API
  slug: amazon-signer-signing-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/openapi/amazon-signer-signing-platforms-api-openapi.yml
- filename: amazon-signer-signing-profiles-api-openapi.yml
  format: yaml
  label: Amazon Signer Signing Profiles API
  slug: amazon-signer-signing-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/openapi/amazon-signer-signing-profiles-api-openapi.yml
- filename: amazon-signer-tags-api-openapi.yml
  format: yaml
  label: Amazon Signer Tags API
  slug: amazon-signer-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/openapi/amazon-signer-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Signer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Signer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Signer
provider_slug: amazon-signer
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-signer.yaml
  type: apiKey
slug: amazon-signer-authentication
source_filename: amazon-signer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-signer.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-signer.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/authentication/amazon-signer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Code Signing
- IoT
- Lambda
- Security
---
