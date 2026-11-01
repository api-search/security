---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pricklymails-com-account-api-openapi.yml
  format: yaml
  label: pricklymails-com Account API
  slug: pricklymails-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-account-api-openapi.yml
- filename: pricklymails-com-agents-api-openapi.yml
  format: yaml
  label: pricklymails-com Agents API
  slug: pricklymails-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-agents-api-openapi.yml
- filename: pricklymails-com-api-keys-api-openapi.yml
  format: yaml
  label: pricklymails-com API Keys API
  slug: pricklymails-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-api-keys-api-openapi.yml
- filename: pricklymails-com-auth-api-openapi.yml
  format: yaml
  label: pricklymails-com Auth API
  slug: pricklymails-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-auth-api-openapi.yml
- filename: pricklymails-com-batches-api-openapi.yml
  format: yaml
  label: pricklymails-com Batches API
  slug: pricklymails-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-batches-api-openapi.yml
- filename: pricklymails-com-billing-api-openapi.yml
  format: yaml
  label: pricklymails-com Billing API
  slug: pricklymails-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-billing-api-openapi.yml
- filename: pricklymails-com-config-api-openapi.yml
  format: yaml
  label: pricklymails-com Config API
  slug: pricklymails-com-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-config-api-openapi.yml
- filename: pricklymails-com-jobs-api-openapi.yml
  format: yaml
  label: pricklymails-com Jobs API
  slug: pricklymails-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-jobs-api-openapi.yml
- filename: pricklymails-com-notifications-api-openapi.yml
  format: yaml
  label: pricklymails-com Notifications API
  slug: pricklymails-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-notifications-api-openapi.yml
- filename: pricklymails-com-oauth-api-openapi.yml
  format: yaml
  label: pricklymails-com OAuth API
  slug: pricklymails-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-oauth-api-openapi.yml
- filename: pricklymails-com-sessions-api-openapi.yml
  format: yaml
  label: pricklymails-com Sessions API
  slug: pricklymails-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-sessions-api-openapi.yml
- filename: pricklymails-com-stats-api-openapi.yml
  format: yaml
  label: pricklymails-com Stats API
  slug: pricklymails-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-stats-api-openapi.yml
- filename: pricklymails-com-subscription-api-openapi.yml
  format: yaml
  label: pricklymails-com Subscription API
  slug: pricklymails-com-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-subscription-api-openapi.yml
- filename: pricklymails-com-verification-api-openapi.yml
  format: yaml
  label: pricklymails-com Verification API
  slug: pricklymails-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-verification-api-openapi.yml
- filename: pricklymails-com-wallet-api-openapi.yml
  format: yaml
  label: pricklymails-com Wallet API
  slug: pricklymails-com-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-wallet-api-openapi.yml
- filename: pricklymails-com-webhooks-api-openapi.yml
  format: yaml
  label: pricklymails-com Webhooks API
  slug: pricklymails-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pricklymails-com/openapi/pricklymails-com-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Pricklymails Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: pricklymails-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: pricklymails-com
provider_slug: pricklymails-com
scheme_count: 2
schemes:
- description: Bearer API key (pm_live_... for production, pm_test_... for sandbox)
  in: header
  name: Authorization
  type: apiKey
- authorizationUrl: <not provided>
  description: OAuth 2.1 PKCE flow for AI agents
  flow: authorizationCode
  tokenUrl: <not provided>
  type: oauth2
slug: pricklymails-com-authentication
source_filename: pricklymails-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://pricklymails.com/docs/authentication\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer API key (pm_live_... for production, pm_test_... for sandbox)\n  - type: oauth2\n    flow: authorizationCode\n    description: OAuth 2.1 PKCE flow for AI agents\n    authorizationUrl: <not provided>\n    tokenUrl: <not provided>\n"
source_yaml_url: https://artifacts.apis.io/pricklymails-com/authentication/pricklymails-com-authentication.yml
summary_line: 2 schemes
tags:
- Email Verification
- API
- SaaS
- Data Validation
- EU-hosted
---
