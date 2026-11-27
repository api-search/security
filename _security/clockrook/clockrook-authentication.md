---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clockrook-account-api-openapi.yml
  format: yaml
  label: Clockrook Account API
  slug: clockrook-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-account-api-openapi.yml
- filename: clockrook-accounts-api-openapi.yml
  format: yaml
  label: Clockrook Accounts API
  slug: clockrook-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-accounts-api-openapi.yml
- filename: clockrook-jobs-api-openapi.yml
  format: yaml
  label: Clockrook Jobs API
  slug: clockrook-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-jobs-api-openapi.yml
- filename: clockrook-pricing-api-openapi.yml
  format: yaml
  label: Clockrook Pricing API
  slug: clockrook-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-pricing-api-openapi.yml
- filename: clockrook-usage-api-openapi.yml
  format: yaml
  label: Clockrook Usage API
  slug: clockrook-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockrook/openapi/clockrook-usage-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clockrook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clockrook secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clockrook
provider_slug: clockrook
scheme_count: 2
schemes:
- description: 'An API key from POST /v1/accounts (shown once). Developers page - "Authenticate with Authorization: Bearer <api_key>". API keys are not scoped.'
  header: Authorization
  name: apiKey
  scheme: bearer
  sources:
  - openapi/clockrook-openapi.yml
  - https://clockrook.com/developers/
  type: http
- authorizationUrl: https://clockrook.com/v1/oauth/authorize
  description: OAuth (browser PKCE) documented in the onboarding descriptor and RFC 8414 metadata; not declared in the OpenAPI securitySchemes. "OAuth tokens carry these scopes and work only on this site."
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  metadata: https://clockrook.com/.well-known/oauth-authorization-server
  name: oauth2
  pkce: S256
  registrationUrl: https://clockrook.com/v1/oauth/register
  revocationUrl: https://clockrook.com/v1/oauth/revoke
  scopes:
  - jobs:read
  - jobs:manage
  - account:read
  sources:
  - https://clockrook.com/.well-known/api-onboarding
  - https://clockrook.com/.well-known/oauth-authorization-server
  tokenUrl: https://clockrook.com/v1/oauth/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: clockrook-authentication
source_filename: clockrook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: searched\nsource: https://clockrook.com/.well-known/api-onboarding\ndocs: https://clockrook.com/developers/\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  header: Authorization\n  description: 'An API key from POST /v1/accounts (shown once). Developers page - \"Authenticate with Authorization: Bearer <api_key>\". API keys are not scoped.'\n  sources:\n  - openapi/clockrook-openapi.yml\n  - https://clockrook.com/developers/\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  authorizationUrl: https://clockrook.com/v1/oauth/authorize\n  tokenUrl: https://clockrook.com/v1/oauth/token\n  revocationUrl: https://clockrook.com/v1/oauth/revoke\n  registrationUrl: https://clockrook.com/v1/oauth/register\n  metadata: https://clockrook.com/.well-known/oauth-authorization-server\n  token_endpoint_auth_methods: [none]\n  grant_types: [authorization_code, refresh_token]\n  scopes:\
  \ [jobs:read, jobs:manage, account:read]\n  description: 'OAuth (browser PKCE) documented in the onboarding descriptor and RFC 8414 metadata; not declared in the OpenAPI securitySchemes. \"OAuth tokens carry these scopes and work only on this site.\"'\n  sources:\n  - https://clockrook.com/.well-known/api-onboarding\n  - https://clockrook.com/.well-known/oauth-authorization-server\nnote: The OpenAPI declares only the bearer API key; the OAuth scheme comes from the provider's published discovery documents (fetched 200).\n"
source_yaml_url: https://artifacts.apis.io/clockrook/authentication/clockrook-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Scheduling
- Cron
- Job
- AI Agents
- Webhook
- Uptime Monitoring
- MCP
---
