---
api_key_in:
- header
api_specs:
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Eligibility Inquiry API
  slug: eligibility-inquiry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Eligibility Summary API
  slug: eligibility-summary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Batch Eligibility API
  slug: batch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Claim Status API
  slug: claim-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Payers API
  slug: payers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Estimation API
  slug: estimation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pverify Authentication
name_suffix: Authentication
oauth_flows: []
overview: pVerify secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: pVerify
provider_slug: pverify
scheme_count: 2
schemes:
- description: OAuth2 access token returned by the /Token endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pverify-openapi.yml
  type: http
- description: Client API identifier issued by pVerify, required on all API calls.
  in: header
  name: clientApiId
  parameter: Client-API-Id
  sources:
  - openapi/pverify-openapi.yml
  type: apiKey
slug: pverify-authentication
source_filename: pverify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pverify-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 access token returned by the /Token endpoint.\n  sources:\n  - openapi/pverify-openapi.yml\n- name: clientApiId\n  type: apiKey\n  in: header\n  parameter: Client-API-Id\n  description: Client API identifier issued by pVerify, required on all API calls.\n  sources:\n  - openapi/pverify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/authentication/pverify-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Healthcare
- Insurance
- Eligibility
- Claims
- EDI
- 270/271
---
