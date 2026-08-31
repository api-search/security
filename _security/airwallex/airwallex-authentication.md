---
api_key_in:
- header
api_specs:
- filename: airwallex-authentication-api-openapi.yml
  format: yaml
  label: Airwallex Authentication API
  slug: airwallex-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-authentication-api-openapi.yml
- filename: airwallex-balances-api-openapi.yml
  format: yaml
  label: Airwallex Balances API
  slug: airwallex-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-balances-api-openapi.yml
- filename: airwallex-beneficiaries-api-openapi.yml
  format: yaml
  label: Airwallex Beneficiaries API
  slug: airwallex-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-beneficiaries-api-openapi.yml
- filename: airwallex-customers-api-openapi.yml
  format: yaml
  label: Airwallex Customers API
  slug: airwallex-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-customers-api-openapi.yml
- filename: airwallex-payment-intents-api-openapi.yml
  format: yaml
  label: Airwallex Payment Intents API
  slug: airwallex-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-payment-intents-api-openapi.yml
- filename: airwallex-payouts-api-openapi.yml
  format: yaml
  label: Airwallex Payouts API
  slug: airwallex-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-payouts-api-openapi.yml
- filename: airwallex-refunds-api-openapi.yml
  format: yaml
  label: Airwallex Refunds API
  slug: airwallex-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-refunds-api-openapi.yml
- filename: airwallex-transfers-api-openapi.yml
  format: yaml
  label: Airwallex Transfers API
  slug: airwallex-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-transfers-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Airwallex Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Airwallex secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Airwallex
provider_slug: airwallex
scheme_count: 4
schemes:
- description: 'Bearer access token obtained via POST /api/v1/authentication/login using

    `x-client-id` and `x-api-key` request headers.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/airwallex-authentication-api-openapi.yml
  - openapi/airwallex-balances-api-openapi.yml
  - openapi/airwallex-beneficiaries-api-openapi.yml
  - openapi/airwallex-customers-api-openapi.yml
  - openapi/airwallex-payment-intents-api-openapi.yml
  - openapi/airwallex-payouts-api-openapi.yml
  - openapi/airwallex-refunds-api-openapi.yml
  - openapi/airwallex-transfers-api-openapi.yml
  type: http
- in: header
  name: ClientIdHeader
  parameter: x-client-id
  sources:
  - openapi/airwallex-authentication-api-openapi.yml
  - openapi/airwallex-balances-api-openapi.yml
  - openapi/airwallex-beneficiaries-api-openapi.yml
  - openapi/airwallex-customers-api-openapi.yml
  - openapi/airwallex-payment-intents-api-openapi.yml
  - openapi/airwallex-payouts-api-openapi.yml
  - openapi/airwallex-refunds-api-openapi.yml
  - openapi/airwallex-transfers-api-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/airwallex-authentication-api-openapi.yml
  - openapi/airwallex-balances-api-openapi.yml
  - openapi/airwallex-beneficiaries-api-openapi.yml
  - openapi/airwallex-customers-api-openapi.yml
  - openapi/airwallex-payment-intents-api-openapi.yml
  - openapi/airwallex-payouts-api-openapi.yml
  - openapi/airwallex-refunds-api-openapi.yml
  - openapi/airwallex-transfers-api-openapi.yml
  type: apiKey
- audience: third-party partner applications, the Airwallex CLI, and the hosted MCP servers
  flows:
  - consent_roles:
    - Owner
    - Admin
    - Finance Admin
    flow: authorizationCode
    scopes: 98
  name: AirwallexOAuth
  revocation: https://www.airwallex.com/app/integrations/home
  scopes_artifact: scopes/airwallex-scopes.yml
  sources:
  - https://www.airwallex.com/docs/developer-tools/partner-connections/oauth-scopes
  - https://mcp.airwallex.com/.well-known/oauth-protected-resource/mcp/
  type: oauth2
slug: airwallex-authentication
source_filename: airwallex-authentication.yml
source_heading: Authentication Profile
source_url: https://www.airwallex.com/docs/api/getting_started
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://www.airwallex.com/docs/api/getting_started\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  token_lifetime: 30 minutes\n  token_endpoint: POST /api/v1/authentication/login\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer access token obtained via POST /api/v1/authentication/login using\n\n    `x-client-id` and `x-api-key` request headers.'\n  sources:\n  - openapi/airwallex-authentication-api-openapi.yml\n  - openapi/airwallex-balances-api-openapi.yml\n  - openapi/airwallex-beneficiaries-api-openapi.yml\n  - openapi/airwallex-customers-api-openapi.yml\n  - openapi/airwallex-payment-intents-api-openapi.yml\n  - openapi/airwallex-payouts-api-openapi.yml\n  - openapi/airwallex-refunds-api-openapi.yml\n  - openapi/airwallex-transfers-api-openapi.yml\n- name: ClientIdHeader\n  type: apiKey\n  in: header\n  parameter:\
  \ x-client-id\n  sources:\n  - openapi/airwallex-authentication-api-openapi.yml\n  - openapi/airwallex-balances-api-openapi.yml\n  - openapi/airwallex-beneficiaries-api-openapi.yml\n  - openapi/airwallex-customers-api-openapi.yml\n  - openapi/airwallex-payment-intents-api-openapi.yml\n  - openapi/airwallex-payouts-api-openapi.yml\n  - openapi/airwallex-refunds-api-openapi.yml\n  - openapi/airwallex-transfers-api-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/airwallex-authentication-api-openapi.yml\n  - openapi/airwallex-balances-api-openapi.yml\n  - openapi/airwallex-beneficiaries-api-openapi.yml\n  - openapi/airwallex-customers-api-openapi.yml\n  - openapi/airwallex-payment-intents-api-openapi.yml\n  - openapi/airwallex-payouts-api-openapi.yml\n  - openapi/airwallex-refunds-api-openapi.yml\n  - openapi/airwallex-transfers-api-openapi.yml\n- name: AirwallexOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n \
  \   scopes: 98\n    consent_roles:\n    - Owner\n    - Admin\n    - Finance Admin\n  audience: third-party partner applications, the Airwallex CLI, and the hosted MCP servers\n  sources:\n  - https://www.airwallex.com/docs/developer-tools/partner-connections/oauth-scopes\n  - https://mcp.airwallex.com/.well-known/oauth-protected-resource/mcp/\n  scopes_artifact: scopes/airwallex-scopes.yml\n  revocation: https://www.airwallex.com/app/integrations/home\ndocs:\n  getting_started: https://www.airwallex.com/docs/api/getting_started\n  manage_api_keys: https://www.airwallex.com/docs/developer-tools/api/manage-api-keys\n  api_key_best_practices: https://www.airwallex.com/docs/developer-tools/api/api-key-best-practices\n  oauth_scopes: https://www.airwallex.com/docs/developer-tools/partner-connections/oauth-scopes\nnote: Upgraded from derived to searched. The three schemes below were confirmed against the provider's own Get started\n  page, and the OAuth model - which the OpenAPI in this repo\
  \ does not carry at all - was added from the partner-connections\n  scope reference and the live RFC 9728 metadata on the hosted MCP servers.\ntoken:\n  endpoint: POST https://api.airwallex.com/api/v1/authentication/login\n  sandbox_endpoint: POST https://api.sandbox.airwallex.com/api/v1/authentication/login\n  request_headers:\n  - x-client-id\n  - x-api-key\n  - 'Content-Type: application/json'\n  response_fields:\n  - token\n  - expires_at\n  lifetime: 30 minutes\n  call_header: 'Authorization: Bearer <token>'\n  rate_limit: 100 requests per minute per API key (fixed, environment-independent)\n  reuse_required: true\ndelegation:\n  header: x-on-behalf-of\n  value: connected account id\n  note: platform credentials plus this header call any endpoint for a connected account; no per-account credentials\n    are issued\nkey_management:\n  location: Account > Developer > API keys in the Airwallex web app\n  environment_separation: separate keys per environment; NO test/live key prefix\n\
  \  best_practices: https://www.airwallex.com/docs/developer-tools/api/api-key-best-practices\nenvironments:\n- name: production\n  base: https://api.airwallex.com/api/v1\n- name: sandbox\n  base: https://api.sandbox.airwallex.com/api/v1\nsources:\n- https://www.airwallex.com/docs/api/getting_started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/authentication/airwallex-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Cross-Border Payments
- Fintech
- Foreign Exchange
- Payments
- Global
- Embedded Finance
- Multi-Currency
---
