---
api_key_in: []
api_specs:
- filename: abound-v4-openapi.yml
  format: yaml
  label: Abound API v4
  slug: abound-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-v4-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Abound Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abound secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Abound
provider_slug: abound
scheme_count: 1
schemes:
- applied_to_operations: 55
  credential_format: appId.appSecret
  description: The bearer token is the concatenation of the Abound appId and appSecret separated by a period, e.g. appId_xxx.appSecret_yyy. A single credential selects the account; the environment is selected by base URL, not by a key prefix.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/abound-v4-openapi.yml
  total_operations: 55
  type: http
slug: abound-authentication
source_filename: abound-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/abound-v4-openapi.yml\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  note: No OAuth surface - a single bearer credential; scopes/ is therefore not applicable.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/abound-v4-openapi.yml\n  credential_format: appId.appSecret\n  description: The bearer token is the concatenation of the Abound appId and appSecret separated by a\n    period, e.g. appId_xxx.appSecret_yyy. A single credential selects the account; the environment is\n    selected by base URL, not by a key prefix.\n  applied_to_operations: 55\n  total_operations: 55\nsecondary_credentials:\n- name: access token\n  purpose: Short-lived token minted for Abound drop-in UI components.\n  operation: accessTokensCreate\n  source_operation: openapi/abound-v4-openapi.yml#accessTokensCreate\nwebhook_verification:\n  header:\
  \ Abound-Signature\n  algorithm: HMAC\n  description: An HMAC signature of the webhook payload.\n  source: openapi/abound-v4-openapi.yml#/webhooks\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/authentication/abound-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Taxes
- Tax Compliance
- Regulatory Compliance
- Financial Services
- Identity Verification
- Government
- Documents
- Webhooks
- Retired
---
