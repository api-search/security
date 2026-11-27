---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hookpie-account-api-openapi.yml
  format: yaml
  label: Hookpie Account API
  slug: hookpie-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-account-api-openapi.yml
- filename: hookpie-accounts-api-openapi.yml
  format: yaml
  label: Hookpie Accounts API
  slug: hookpie-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-accounts-api-openapi.yml
- filename: hookpie-i-api-openapi.yml
  format: yaml
  label: Hookpie I API
  slug: hookpie-i-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-i-api-openapi.yml
- filename: hookpie-inboxes-api-openapi.yml
  format: yaml
  label: Hookpie Inboxes API
  slug: hookpie-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-inboxes-api-openapi.yml
- filename: hookpie-pricing-api-openapi.yml
  format: yaml
  label: Hookpie Pricing API
  slug: hookpie-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-pricing-api-openapi.yml
- filename: hookpie-usage-api-openapi.yml
  format: yaml
  label: Hookpie Usage API
  slug: hookpie-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookpie/openapi/hookpie-usage-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hookpie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hookpie secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hookpie
provider_slug: hookpie
scheme_count: 2
schemes:
- bootstrap: POST /v1/accounts (or the create_account MCP tool) returns the key once
  description: 'An API key from POST /v1/accounts (shown once). Docs: "Authenticate with Authorization: Bearer <api_key>." API keys are not scoped.'
  header: Authorization
  name: apiKey
  scheme: bearer
  sources:
  - openapi/hookpie-openapi.yml
  - https://hookpie.com/developers/
  - https://hookpie.com/.well-known/api-onboarding
  type: http
- authorizationUrl: https://hookpie.com/v1/oauth/authorize
  description: Browser OAuth with PKCE; tokens carry scopes and "work only on this site". Documented in the api-onboarding descriptor and RFC 8414 metadata, NOT declared in the OpenAPI securitySchemes.
  flow: authorization_code (PKCE S256, public client, token_endpoint_auth_methods_supported none) with refresh_token
  metadata: https://hookpie.com/.well-known/oauth-authorization-server
  name: oauth2
  scopes:
  - inbox:read
  - inbox:manage
  - account:read
  sources:
  - https://hookpie.com/.well-known/api-onboarding
  - https://hookpie.com/.well-known/oauth-authorization-server
  tokenUrl: https://hookpie.com/v1/oauth/token
  type: oauth2
slug: hookpie-authentication
source_filename: hookpie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: searched\nsource: https://hookpie.com/developers/\ndocs: https://hookpie.com/developers/\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  header: Authorization\n  description: 'An API key from POST /v1/accounts (shown once). Docs: \"Authenticate with Authorization: Bearer <api_key>.\" API keys are not scoped.'\n  bootstrap: POST /v1/accounts (or the create_account MCP tool) returns the key once\n  sources:\n  - openapi/hookpie-openapi.yml\n  - https://hookpie.com/developers/\n  - https://hookpie.com/.well-known/api-onboarding\n- name: oauth2\n  type: oauth2\n  flow: authorization_code (PKCE S256, public client, token_endpoint_auth_methods_supported none) with refresh_token\n  authorizationUrl: https://hookpie.com/v1/oauth/authorize\n  tokenUrl: https://hookpie.com/v1/oauth/token\n  metadata: https://hookpie.com/.well-known/oauth-authorization-server\n  scopes:\n  - inbox:read\n  - inbox:manage\n\
  \  - account:read\n  description: Browser OAuth with PKCE; tokens carry scopes and \"work only on this site\". Documented in the api-onboarding descriptor and RFC 8414 metadata, NOT declared in the OpenAPI securitySchemes.\n  sources:\n  - https://hookpie.com/.well-known/api-onboarding\n  - https://hookpie.com/.well-known/oauth-authorization-server\nunauthenticated:\n- operation: receiveWebhook\n  note: 'Receive path POST|PUT|PATCH|DELETE https://hookpie.com/i/{inbox_id}[/anything], no authentication, answers 202.'\n"
source_yaml_url: https://artifacts.apis.io/hookpie/authentication/hookpie-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Webhook
- AI Agents
- MCP
- Event Inbox
- Developer Tools
- Pay-as-you-go
---
