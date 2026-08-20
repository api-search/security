---
api_key_in: []
api_specs:
- filename: hooklogic-criteo-accounts-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Accounts API
  slug: hooklogic-criteo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-accounts-api-openapi.yml
- filename: hooklogic-criteo-analytics-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Analytics API
  slug: hooklogic-criteo-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-analytics-api-openapi.yml
- filename: hooklogic-criteo-audience-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Audience API
  slug: hooklogic-criteo-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-audience-api-openapi.yml
- filename: hooklogic-criteo-balance-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Balance API
  slug: hooklogic-criteo-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-balance-api-openapi.yml
- filename: hooklogic-criteo-billing-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Billing API
  slug: hooklogic-criteo-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-billing-api-openapi.yml
- filename: hooklogic-criteo-campaign-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Campaign API
  slug: hooklogic-criteo-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-campaign-api-openapi.yml
- filename: hooklogic-criteo-catalog-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Catalog API
  slug: hooklogic-criteo-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-catalog-api-openapi.yml
- filename: hooklogic-criteo-gateway-api-openapi.yml
  format: yaml
  label: HookLogic (Criteo) Gateway API
  slug: hooklogic-criteo-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/openapi/hooklogic-criteo-gateway-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hooklogic Criteo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: HookLogic (Criteo) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: HookLogic (Criteo)
provider_slug: hooklogic-criteo
scheme_count: 1
schemes:
- applies_to: all eight Retail Media specs (Accounts, Analytics, Audience, Balance, Billing, Campaign, Catalog, Gateway)
  flows:
  - flow: clientCredentials
    rate_limit: 250 calls/min default, 40 calls/min reporting
    scope_level: application
    tokenUrl: https://api.criteo.com/oauth2/token
    use_case: server-to-server, single data owner
  - authorizationUrl: https://api.criteo.com/oauth2
    flow: authorizationCode
    pkce: true
    pkce_docs: https://developers.criteo.com/criteo-apis/docs/oauth-app-authorization-code-pkce-setup
    rate_limit: 10 calls/min per account per user, scales with consents
    refresh_token: valid 6 months; revoked if the user's role changes
    scope_level: account
    tokenUrl: https://api.criteo.com/oauth2/token
    use_case: multi-user, self-service platforms
  header: 'Authorization: Bearer <access_token>'
  name: oauth
  scopes: scopes/hooklogic-criteo-scopes.yml
  token_lifetime_seconds: 900
  type: oauth2
slug: hooklogic-criteo-authentication
source_filename: hooklogic-criteo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://developers.criteo.com/criteo-apis/docs/authentication\nsource: >-\n  openapi/hooklogic-criteo-*-openapi.yml (all eight refined specs declare the\n  same `oauth` scheme), upgraded from\n  https://developers.criteo.com/criteo-apis/docs/authentication and the\n  provider-published Agent Skill at\n  https://developers.criteo.com/.well-known/agent-skills/criteo/skill.md\nnote: >-\n  The Criteo Retail Media API (the HookLogic product line) is OAuth 2.0 only —\n  there is no API-key or basic-auth path. Every one of the eight refined\n  OpenAPI documents declares the same single `oauth` security scheme, so the\n  profile is stated once here rather than repeated per spec. Two grants are\n  supported and they differ in more than plumbing: client-credentials is\n  application-scoped and single-data-owner, authorization-code is account-scoped\n  and requires explicit advertiser consent, which is also what determines the\n  rate limit\
  \ an integration gets.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  api_key: false\n  basic: false\n  mtls: false\nschemes:\n- name: oauth\n  type: oauth2\n  applies_to: all eight Retail Media specs (Accounts, Analytics, Audience, Balance, Billing, Campaign, Catalog, Gateway)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.criteo.com/oauth2/token\n    scope_level: application\n    use_case: server-to-server, single data owner\n    rate_limit: 250 calls/min default, 40 calls/min reporting\n  - flow: authorizationCode\n    authorizationUrl: https://api.criteo.com/oauth2\n    tokenUrl: https://api.criteo.com/oauth2/token\n    scope_level: account\n    pkce: true\n    pkce_docs: https://developers.criteo.com/criteo-apis/docs/oauth-app-authorization-code-pkce-setup\n    use_case: multi-user, self-service platforms\n    rate_limit: 10 calls/min per account per user, scales with consents\n    refresh_token: valid 6 months;\
  \ revoked if the user's role changes\n  header: 'Authorization: Bearer <access_token>'\n  token_lifetime_seconds: 900\n  scopes: scopes/hooklogic-criteo-scopes.yml\nonboarding:\n  steps:\n  - Create a Criteo partner account\n  - Create an organization\n  - Create an API application and select the permission domains it needs\n  - Retrieve client credentials\n  - For authorization-code apps, generate a consent URL and have the advertiser approve it\n  docs: https://developers.criteo.com/criteo-apis/docs/connect-to-the-api\nfailure_modes:\n- status: 401\n  cause: missing or expired access token (tokens live 900 seconds)\n- status: 403\n  cause: token lacks the permission domain for the endpoint, or an account admin revoked the application's consent\nsee:\n  scopes: scopes/hooklogic-criteo-scopes.yml\n  conventions: conventions/hooklogic-criteo-conventions.yml\n  errors: errors/hooklogic-criteo-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hooklogic-criteo/refs/heads/main/authentication/hooklogic-criteo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Commerce
- Retail Media
- Advertising
- E-Commerce
- Marketing
- Retail
---
