---
api_key_in:
- header
api_specs:
- filename: talon-one-integration-api-openapi.yml
  format: yaml
  label: Talon.One Integration API
  slug: talon-one-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-integration-api-openapi.yml
- filename: talon-one-management-api-openapi.yml
  format: yaml
  label: Talon.One Management API
  slug: talon-one-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-management-api-openapi.yml
- filename: talon-one-third-party-api-openapi.yml
  format: yaml
  label: Talon.One Third-party API
  slug: talon-one-third-party-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-third-party-api-openapi.yml
- filename: talon-one-shopify-integration-api-openapi.yml
  format: yaml
  label: Talon.One Shopify Integration API
  slug: talon-one-shopify-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-shopify-integration-api-openapi.yml
- filename: talon-one-outbound-notifications-openapi.yml
  format: yaml
  label: Talon.One Outbound Notifications
  slug: talon-one-outbound-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-outbound-notifications-openapi.yml
auth_types:
- apiKey
- http
description: Every Talon.One API authenticates with a credential in the Authorization header; there is no OAuth 2.0 or OpenID Connect anywhere in the estate. Which credential you use depends on the surface, and the prefix is part of the value.
kind: authentication
layout: security
method: searched
name: Talon One Authentication
name_suffix: Authentication
oauth_flows: []
overview: Talon.One secures its APIs with apiKey and http across 8 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Talon.One
provider_slug: talon-one
scheme_count: 8
schemes:
- apis:
  - Integration API
  example_form: 'Authorization: ApiKey-v1 <key>'
  in: header
  issuance: Campaign Manager > Application > Settings > Integration API Keys > Create API Key. Name and expiration date required.
  key_types:
  - Production
  - Test (staging only, dry requests only, one per Application)
  name: Integration API key
  parameter: Authorization
  prefix: ApiKey-v1
  sources:
  - openapi/talon-one-integration-api-openapi.yml
  - https://docs.talon.one/docs/product/applications/manage-api-keys
  spec_name: api_key_v1
  type: apiKey
- apis:
  - Management API
  example_form: 'Authorization: ManagementKey-v1 <key>'
  in: header
  issuance: Campaign Manager > Account > Tools > Management API Keys > Create Key. Created by an admin, with an explicit allow-list of endpoints and a mandatory expiration date.
  name: Management API key
  parameter: Authorization
  prefix: ManagementKey-v1
  recommended: true
  scoping: Per-key endpoint allow-list chosen at creation time — the closest thing Talon.One has to scopes, but it is not an OAuth scope model and is not enumerable through the API.
  sources:
  - openapi/talon-one-management-api-openapi.yml
  - https://docs.talon.one/docs/product/account/dev-tools/manage-mapi-keys
  spec_name: management_key
  type: apiKey
- apis:
  - Management API
  example_form: 'Authorization: Bearer <token>'
  in: header
  issuance: POST /v1/sessions (createSession) with user credentials; token valid for 3 months.
  name: Management session bearer token
  note: Talon.One explicitly recommends the Management API key over this bearer token.
  parameter: Authorization
  prefix: Bearer
  recommended: false
  sources:
  - openapi/talon-one-management-api-openapi.yml
  spec_name: manager_auth
  type: apiKey
- apis:
  - Third-party API
  in: header
  issuance: Created as an Integration API key with "Third-party integration" set to Yes and the partner platform selected.
  name: Third-party API key
  parameter: Authorization
  prefix: ApiKey-v1
  sources:
  - openapi/talon-one-third-party-api-openapi.yml
  spec_name: ApiKeyAuth
  type: apiKey
- apis:
  - Third-party API
  name: Third-party HTTP Basic
  note: Alternative for partner platforms that cannot set a custom Authorization scheme.
  scheme: basic
  sources:
  - openapi/talon-one-third-party-api-openapi.yml
  spec_name: ApiKeyBasicAuth
  type: http
- apis:
  - Shopify Integration API
  in: header
  name: Shopify customer access token
  note: Shopify Customer Account API token (shcat_ prefix), issued by Shopify not Talon.One.
  parameter: Authorization
  sources:
  - openapi/talon-one-shopify-integration-api-openapi.yml
  spec_name: ShopifyCustomerAccessToken
  type: apiKey
- apis:
  - Shopify Integration API
  bearerFormat: JWT
  name: Shopify JWT
  scheme: bearer
  sources:
  - openapi/talon-one-shopify-integration-api-openapi.yml
  spec_name: ShopifyJWT
  type: http
- apis:
  - MCP server
  in: header
  issuance: Campaign Manager > Account > Tools > MCP Connections > Create Key (admin only, expiring, shown once).
  name: MCP connection key
  note: Separate key type for the MCP server; inherits the account role permissions of the creating admin.
  parameter: Authorization
  prefix: Bearer
  sources:
  - https://docs.talon.one/docs/dev/mcp
  spec_name: null
  type: apiKey
slug: talon-one-authentication
source_filename: talon-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.talon.one/docs/product/account/dev-tools/manage-mapi-keys\ndocs: https://docs.talon.one/docs/product/account/dev-tools/manage-mapi-keys\nprovider: Talon.One\nproviderId: talon-one\ndescription: Every Talon.One API authenticates with a credential in the Authorization header; there is\n  no OAuth 2.0 or OpenID Connect anywhere in the estate. Which credential you use depends on the surface,\n  and the prefix is part of the value.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: Integration API key\n  spec_name: api_key_v1\n  type: apiKey\n  in: header\n  parameter: Authorization\n  prefix: ApiKey-v1\n  example_form: 'Authorization: ApiKey-v1 <key>'\n  issuance: Campaign Manager > Application > Settings > Integration API Keys > Create API Key. Name and\n    expiration date required.\n  key_types:\n  - Production\n\
  \  - Test (staging only, dry requests only, one per Application)\n  apis:\n  - Integration API\n  sources:\n  - openapi/talon-one-integration-api-openapi.yml\n  - https://docs.talon.one/docs/product/applications/manage-api-keys\n- name: Management API key\n  spec_name: management_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  prefix: ManagementKey-v1\n  example_form: 'Authorization: ManagementKey-v1 <key>'\n  issuance: Campaign Manager > Account > Tools > Management API Keys > Create Key. Created by an admin,\n    with an explicit allow-list of endpoints and a mandatory expiration date.\n  scoping: Per-key endpoint allow-list chosen at creation time — the closest thing Talon.One has to scopes,\n    but it is not an OAuth scope model and is not enumerable through the API.\n  recommended: true\n  apis:\n  - Management API\n  sources:\n  - openapi/talon-one-management-api-openapi.yml\n  - https://docs.talon.one/docs/product/account/dev-tools/manage-mapi-keys\n- name: Management\
  \ session bearer token\n  spec_name: manager_auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  prefix: Bearer\n  example_form: 'Authorization: Bearer <token>'\n  issuance: POST /v1/sessions (createSession) with user credentials; token valid for 3 months.\n  recommended: false\n  note: Talon.One explicitly recommends the Management API key over this bearer token.\n  apis:\n  - Management API\n  sources:\n  - openapi/talon-one-management-api-openapi.yml\n- name: Third-party API key\n  spec_name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  prefix: ApiKey-v1\n  issuance: Created as an Integration API key with \"Third-party integration\" set to Yes and the partner\n    platform selected.\n  apis:\n  - Third-party API\n  sources:\n  - openapi/talon-one-third-party-api-openapi.yml\n- name: Third-party HTTP Basic\n  spec_name: ApiKeyBasicAuth\n  type: http\n  scheme: basic\n  note: Alternative for partner platforms that cannot set a custom Authorization\
  \ scheme.\n  apis:\n  - Third-party API\n  sources:\n  - openapi/talon-one-third-party-api-openapi.yml\n- name: Shopify customer access token\n  spec_name: ShopifyCustomerAccessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  note: Shopify Customer Account API token (shcat_ prefix), issued by Shopify not Talon.One.\n  apis:\n  - Shopify Integration API\n  sources:\n  - openapi/talon-one-shopify-integration-api-openapi.yml\n- name: Shopify JWT\n  spec_name: ShopifyJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  apis:\n  - Shopify Integration API\n  sources:\n  - openapi/talon-one-shopify-integration-api-openapi.yml\n- name: MCP connection key\n  spec_name: null\n  type: apiKey\n  in: header\n  parameter: Authorization\n  prefix: Bearer\n  issuance: Campaign Manager > Account > Tools > MCP Connections > Create Key (admin only, expiring, shown\n    once).\n  note: Separate key type for the MCP server; inherits the account role permissions of the creating admin.\n\
  \  apis:\n  - MCP server\n  sources:\n  - https://docs.talon.one/docs/dev/mcp\naccount_security:\n  two_factor: https://docs.talon.one/docs/product/account/account-settings/set-up-2fa\n  roles: https://docs.talon.one/docs/product/account/account-settings/manage-roles\n  audit_logs: https://docs.talon.one/docs/product/account/logs/audit-logs\n  key_expiry: All API key types require an expiration date at creation; keys move through Valid, Expires\n    Soon, Expired and Invalid states.\n  key_lifecycle_note: A key created by a user who is later disabled or deleted keeps working until it\n    expires.\noauth_scopes:\n  applicable: false\n  note: No oauth2 securityScheme exists in any published spec, so there is no scope vocabulary to derive.\n    Endpoint-level permissioning is done per Management API key at creation time.\nprevious_derivation:\n  method: derived\n  kept_for: spec-level scheme names\n  spec_schemes:\n  - api_key_v1\n  - ShopifyJWT\n  - ApiKeyBasicAuth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/authentication/talon-one-authentication.yml
summary_line: apiKey/http · 8 schemes
tags:
- Promotions
- Loyalty
- Coupons
- Incentives
- Campaigns
- Personalization
- MarTech
- Rules Engine
- Referrals
- Discounts
- E-Commerce
- Retail
---
