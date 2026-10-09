---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: centrapay-payment-requests-api-openapi.yml
  format: yaml
  label: Centrapay Payment Requests API
  slug: centrapay-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrapay/refs/heads/main/openapi/centrapay-payment-requests-api-openapi.yml
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Centrapay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Centrapay secures its APIs with apiKey and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Centrapay
provider_slug: centrapay
scheme_count: 2
schemes:
- description: API Keys provide enduring access to a single Centrapay account. Roles "account-owner" and "merchant-terminal".
  docs: https://docs.centrapay.com/api/api-keys
  in: header
  name: ApiKey
  parameter: X-Api-Key
  sources:
  - openapi/centrapay-openapi.yml
  - https://docs.centrapay.com/api/auth
  type: apiKey
- description: User access tokens provide time-limited access to all Centrapay accounts for which the user is a member. Issued using OIDC code flow via auth.centrapay.com. Access Token expires after 1 hour; Refresh Token expires after 60 days or when revoked. OAuth client ids with whitelisted redirect URIs are obtained by contacting Centrapay support.
  flow: authorization_code with PKCE
  in: header
  name: UserAccessToken
  not_in_spec: true
  openIdConnectUrl: https://auth.centrapay.com/.well-known/openid-configuration
  parameter: Authorization
  sources:
  - https://docs.centrapay.com/api/auth
  token_lifetimes:
    access_token: Expires after 1 hour.
    refresh_token: Expires after 60 days or when revoked.
  type: openIdConnect
slug: centrapay-authentication
source_filename: centrapay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://docs.centrapay.com/api/auth\ndocs: https://docs.centrapay.com/api/auth\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API Keys provide enduring access to a single Centrapay account. Roles \"account-owner\" and \"merchant-terminal\".\n  docs: https://docs.centrapay.com/api/api-keys\n  sources:\n  - openapi/centrapay-openapi.yml\n  - https://docs.centrapay.com/api/auth\n- name: UserAccessToken\n  type: openIdConnect\n  in: header\n  parameter: Authorization\n  openIdConnectUrl: https://auth.centrapay.com/.well-known/openid-configuration\n  flow: authorization_code with PKCE\n  description: User access tokens provide time-limited access to all Centrapay accounts for which the user is a member. Issued using OIDC code flow via auth.centrapay.com. Access Token expires after 1 hour; Refresh Token expires\
  \ after 60 days or when revoked. OAuth client ids with whitelisted redirect URIs are obtained by contacting Centrapay support.\n  token_lifetimes:\n    access_token: Expires after 1 hour.\n    refresh_token: Expires after 60 days or when revoked.\n  not_in_spec: true\n  sources:\n  - https://docs.centrapay.com/api/auth\nheaders:\n- name: X-Centrapay-Account\n  description: Required for Org Accounts accessed with a user access token; specifies the unique identifier of the Centrapay Org Account.\nauthorization_model:\n  style: role-based permissions\n  roles: [Account Owner, Anon Consumer, Merchant Terminal, External Asset Provider, Cashier]\n  docs: https://docs.centrapay.com/api/auth#permissions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrapay/refs/heads/main/authentication/centrapay-authentication.yml
summary_line: apiKey/openIdConnect · 2 schemes
tags:
- Company
- Payments
- Digital Wallets
- Open Banking
- QR Code Payments
- Loyalty
- Gift Cards
- Fintech
---
