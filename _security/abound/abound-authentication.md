---
api_key_in: []
api_specs:
- filename: abound-1099-int-api-openapi.yml
  format: yaml
  label: Abound 1099-INT API
  slug: abound-1099-int-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-1099-int-api-openapi.yml
- filename: abound-1099-k-api-openapi.yml
  format: yaml
  label: Abound 1099-K API
  slug: abound-1099-k-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-1099-k-api-openapi.yml
- filename: abound-1099-misc-api-openapi.yml
  format: yaml
  label: Abound 1099-MISC API
  slug: abound-1099-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-1099-misc-api-openapi.yml
- filename: abound-1099-nec-api-openapi.yml
  format: yaml
  label: Abound 1099-NEC API
  slug: abound-1099-nec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-1099-nec-api-openapi.yml
- filename: abound-access-tokens-api-openapi.yml
  format: yaml
  label: Abound Access Tokens API
  slug: abound-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-access-tokens-api-openapi.yml
- filename: abound-electronic-delivery-consents-api-openapi.yml
  format: yaml
  label: Abound Electronic Delivery Consents API
  slug: abound-electronic-delivery-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-electronic-delivery-consents-api-openapi.yml
- filename: abound-mailings-api-openapi.yml
  format: yaml
  label: Abound Mailings API
  slug: abound-mailings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-mailings-api-openapi.yml
- filename: abound-tax-treaties-api-openapi.yml
  format: yaml
  label: Abound Tax Treaties API
  slug: abound-tax-treaties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-tax-treaties-api-openapi.yml
- filename: abound-tin-verifications-api-openapi.yml
  format: yaml
  label: Abound TIN Verifications API
  slug: abound-tin-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-tin-verifications-api-openapi.yml
- filename: abound-users-api-openapi.yml
  format: yaml
  label: Abound Users API
  slug: abound-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-users-api-openapi.yml
- filename: abound-w-8ben-api-openapi.yml
  format: yaml
  label: Abound W-8BEN API
  slug: abound-w-8ben-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-w-8ben-api-openapi.yml
- filename: abound-w-8ben-e-api-openapi.yml
  format: yaml
  label: Abound W-8BEN-E API
  slug: abound-w-8ben-e-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-w-8ben-e-api-openapi.yml
- filename: abound-w-9-api-openapi.yml
  format: yaml
  label: Abound W-9 API
  slug: abound-w-9-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-w-9-api-openapi.yml
- filename: abound-abound-api-v4-api-openapi.yml
  format: yaml
  label: Abound Abound API V4 API
  slug: abound-abound-api-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-abound-api-v4-api-openapi.yml
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
- Financial-Services
- Identity Verification
- Government
- Documents
- Webhook
- Retired
---
