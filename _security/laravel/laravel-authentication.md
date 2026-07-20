---
api_key_in: []
api_specs:
- filename: laravel-forge-openapi.json
  format: json
  label: Laravel Forge API
  slug: forge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laravel/refs/heads/main/openapi/laravel-forge-openapi.json
- filename: laravel-cloud-openapi.json
  format: json
  label: Laravel Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laravel/refs/heads/main/openapi/laravel-cloud-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Laravel Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Laravel secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Laravel
provider_slug: laravel
scheme_count: 2
schemes:
- bearerFormat: bearer
  description: The Bearer Token generated on the Cloud UI.
  name: http
  scheme: bearer
  sources:
  - openapi/laravel-cloud-openapi.json
  - openapi/laravel-forge-openapi.json
  type: http
- flows:
  - authorizationUrl: https://forge.laravel.com/oauth/authorize
    flow: authorizationCode
    scopes: 62
    tokenUrl: https://forge.laravel.com/oauth/token
  name: oauth2
  sources:
  - openapi/laravel-forge-openapi.json
  type: oauth2
slug: laravel-authentication
source_filename: laravel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/laravel-cloud-openapi.json, openapi/laravel-forge-openapi.json\ndocs: https://forge.laravel.com/docs/api-reference/introduction, https://cloud.laravel.com/docs/api/authentication,\n  https://forge.laravel.com/docs/api, https://envoyer.io/api-documentation\nnotes: Baseline derived mechanically from both OpenAPI files, then upgraded from the provider's auth\n  documentation. Every Laravel commercial API is bearer-token authenticated. Forge additionally declares\n  a full OAuth 2.0 authorization-code flow with 62 scopes for third-party applications. Laravel account\n  sign-in itself runs through a separate OIDC identity provider at id.laravel.com, which is not the\n  resource-API auth path.\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  transport: 'Authorization: Bearer <token> header'\n  required_headers:\n  - 'Accept: application/json'\n  - 'Content-Type: application/json'\n\
  schemes:\n- name: http\n  type: http\n  scheme: bearer\n  bearerFormat: bearer\n  description: The Bearer Token generated on the Cloud UI.\n  sources:\n  - openapi/laravel-cloud-openapi.json\n  - openapi/laravel-forge-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://forge.laravel.com/oauth/authorize\n    tokenUrl: https://forge.laravel.com/oauth/token\n    scopes: 62\n  sources:\n  - openapi/laravel-forge-openapi.json\nper_api:\n- api: laravel:forge-api\n  primary: bearer token (personal API token)\n  token_management:\n    dashboard: https://forge.laravel.com/profile/api\n    docs: https://forge.laravel.com/docs/api\n    create: 'Account dashboard > API > Create token: provide a name, an optional expiration date, and\n      select the scopes to assign.'\n    expiration: optional per-token expiration date\n    scoped: true\n    revocation: Deleting a token is permanent and immediately breaks any integration using it.\n \
  \ oauth2:\n    flow: authorizationCode\n    authorization_url: https://forge.laravel.com/oauth/authorize\n    token_url: https://forge.laravel.com/oauth/token\n    scope_count: 62\n    scopes_artifact: scopes/laravel-scopes.yml\n  ci: Set FORGE_API_TOKEN in the CI environment for the Forge CLI.\n  authorization_model: Organization-scoped. Every v2 resource path is nested under /orgs/{organization},\n    and roles/permissions resources exist in the API (Roles, Teams, Permissions tags).\n- api: laravel:cloud-api\n  primary: bearer token generated in the Laravel Cloud UI\n  docs: https://cloud.laravel.com/docs/api/authentication\n  oauth2: not offered\n  scoped: not declared in the OpenAPI\n  authorization_model: Token is bound to an organization; resource paths are flat.\n- api: laravel:forge-api-legacy\n  primary: bearer API key\n  docs: https://forge.laravel.com/api-documentation\n  note: Same Authorization Bearer transport as v2; deprecated with discontinuation announced for\n    2026-07-31.\n\
  - api: laravel:envoyer-api\n  primary: bearer API key\n  docs: https://envoyer.io/api-documentation\n  scoped: coarse — all GET endpoints are readable with any token; *:create scopes govern writes.\nidentity_provider:\n  issuer: https://id.laravel.com\n  role: End-user SSO for Laravel Cloud sign-in/sign-up. Not used to authenticate resource-API calls.\n  discovery: well-known/laravel-openid-configuration.json\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  pkce: S256\n  id_token_signing: RS256\ngaps:\n- Neither API documents token rotation guidance, token introspection, or a machine-to-machine\n  client-credentials path for the resource APIs.\n- The Cloud API declares no scopes, so a Cloud token is all-or-nothing against the organization.\n- No mutualTLS or proof-of-possession option is offered on any Laravel API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laravel/refs/heads/main/authentication/laravel-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Cloud Saas
- PHP
- Developer Tools
- Platform as a Service
- Deployment
- Server Management
- Application Hosting
- Infrastructure
- Frameworks
- Monitoring
---
