---
anonymous_access: false
api_key_in: []
api_specs:
- filename: moneyhash-accounts-api-openapi.yml
  format: yaml
  label: MoneyHash Accounts API
  slug: moneyhash-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-accounts-api-openapi.yml
- filename: moneyhash-customers-api-openapi.yml
  format: yaml
  label: MoneyHash Customers API
  slug: moneyhash-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-customers-api-openapi.yml
- filename: moneyhash-direct-api-openapi.yml
  format: yaml
  label: MoneyHash Direct API
  slug: moneyhash-direct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-direct-api-openapi.yml
- filename: moneyhash-external-api-openapi.yml
  format: yaml
  label: MoneyHash External API
  slug: moneyhash-external-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-external-api-openapi.yml
- filename: moneyhash-loyalty-api-openapi.yml
  format: yaml
  label: MoneyHash Loyalty API
  slug: moneyhash-loyalty-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-loyalty-api-openapi.yml
- filename: moneyhash-payment-links-api-openapi.yml
  format: yaml
  label: MoneyHash Payment Links API
  slug: moneyhash-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-payment-links-api-openapi.yml
- filename: moneyhash-payments-api-openapi.yml
  format: yaml
  label: MoneyHash Payments API
  slug: moneyhash-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-payments-api-openapi.yml
- filename: moneyhash-payout-api-openapi.yml
  format: yaml
  label: MoneyHash Payout API
  slug: moneyhash-payout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-payout-api-openapi.yml
- filename: moneyhash-providers-api-openapi.yml
  format: yaml
  label: MoneyHash Providers API
  slug: moneyhash-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-providers-api-openapi.yml
- filename: moneyhash-reconciliations-api-openapi.yml
  format: yaml
  label: MoneyHash Reconciliations API
  slug: moneyhash-reconciliations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-reconciliations-api-openapi.yml
- filename: moneyhash-subscriptions-api-openapi.yml
  format: yaml
  label: MoneyHash Subscriptions API
  slug: moneyhash-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-subscriptions-api-openapi.yml
- filename: moneyhash-tokens-api-openapi.yml
  format: yaml
  label: MoneyHash Tokens API
  slug: moneyhash-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-tokens-api-openapi.yml
- filename: moneyhash-transactions-api-openapi.yml
  format: yaml
  label: MoneyHash Transactions API
  slug: moneyhash-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneyhash/openapi/moneyhash-transactions-api-openapi.yml
auth_types: []
description: Authentication schemes defined in MoneyHash API OpenAPI specification
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Moneyhash Authentication
name_suffix: Authentication
oauth_flows: []
overview: MoneyHash declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MoneyHash
provider_slug: moneyhash
scheme_count: 2
schemes:
- evidence: 'AccessTokenAuth": { "type": "apiKey", "in": "query", "name": "access_token" }'
  location: query
  name: AccessTokenAuth
  type: apiKey
- evidence: 'ApiKeyAuth": { "type": "apiKey", "in": "header", "name": "X-Api-Key" }'
  header: X-Api-Key
  location: header
  name: ApiKeyAuth
  type: apiKey
slug: moneyhash-authentication
source_filename: moneyhash-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.moneyhash.io/reference/v11_accounts_get_from_access_token_retrieve.md
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.moneyhash.io/reference/v11_accounts_get_from_access_token_retrieve.md\nsources:\n- https://docs.moneyhash.io/reference/v11_accounts_get_from_access_token_retrieve.md\n- https://docs.moneyhash.io/reference/v11_accounts_reset_access_token_create.md\n- https://docs.moneyhash.io/reference/v11_payments_charge_card_token_create.md\n- https://docs.moneyhash.io/reference/v11_external_payments_intents_card_token_create.md\ndescription: Authentication schemes defined in MoneyHash API OpenAPI specification\nschemes:\n- type: apiKey\n  name: AccessTokenAuth\n  evidence: 'AccessTokenAuth\": { \"type\": \"apiKey\", \"in\": \"query\", \"name\": \"access_token\" }'\n  location: query\n- type: apiKey\n  name: ApiKeyAuth\n  evidence: 'ApiKeyAuth\": { \"type\": \"apiKey\", \"in\": \"header\", \"name\": \"X-Api-Key\" }'\n  location: header\n  header: X-Api-Key\nnote: No OAuth2 flows or\
  \ other authentication methods are documented on the provided pages.\ndocs: https://docs.moneyhash.io/reference/v11_accounts_get_from_access_token_retrieve.md\n"
source_yaml_url: https://artifacts.apis.io/moneyhash/authentication/moneyhash-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Payments
- Fintech
- Orchestration
- API
---
