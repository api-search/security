---
api_key_in:
- header
api_specs:
- filename: lemlist-openapi-v2.json
  format: json
  label: lemlist REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/_original/lemlist-openapi-v2.json
- filename: lemlist-campaigns-api-openapi.yml
  format: yaml
  label: lemlist Campaigns API
  slug: lemlist-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-campaigns-api-openapi.yml
- filename: lemlist-sequences-api-openapi.yml
  format: yaml
  label: lemlist Sequences API
  slug: lemlist-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-sequences-api-openapi.yml
- filename: lemlist-leads-api-openapi.yml
  format: yaml
  label: lemlist Leads API
  slug: lemlist-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-leads-api-openapi.yml
- filename: lemlist-people-database-api-openapi.yml
  format: yaml
  label: lemlist People Database API
  slug: lemlist-people-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-people-database-api-openapi.yml
- filename: lemlist-enrich-api-openapi.yml
  format: yaml
  label: lemlist Enrich API
  slug: lemlist-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-enrich-api-openapi.yml
- filename: lemlist-inbox-api-openapi.yml
  format: yaml
  label: lemlist Inbox API
  slug: lemlist-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-inbox-api-openapi.yml
- filename: lemlist-contacts-api-openapi.yml
  format: yaml
  label: lemlist Contacts API
  slug: lemlist-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-contacts-api-openapi.yml
- filename: lemlist-companies-api-openapi.yml
  format: yaml
  label: lemlist Companies API
  slug: lemlist-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-companies-api-openapi.yml
- filename: lemlist-signal-agents-api-openapi.yml
  format: yaml
  label: lemlist Signal Agents API
  slug: lemlist-signal-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-signal-agents-api-openapi.yml
- filename: lemlist-webhooks-api-openapi.yml
  format: yaml
  label: lemlist Webhooks API
  slug: lemlist-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-webhooks-api-openapi.yml
- filename: lemlist-unsubscribes-api-openapi.yml
  format: yaml
  label: lemlist Unsubscribes API
  slug: lemlist-unsubscribes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-unsubscribes-api-openapi.yml
- filename: lemlist-schedules-api-openapi.yml
  format: yaml
  label: lemlist Schedules API
  slug: lemlist-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-schedules-api-openapi.yml
- filename: lemlist-tasks-api-openapi.yml
  format: yaml
  label: lemlist Tasks API
  slug: lemlist-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-tasks-api-openapi.yml
- filename: lemlist-activities-api-openapi.yml
  format: yaml
  label: lemlist Activities API
  slug: lemlist-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-activities-api-openapi.yml
- filename: lemlist-team-api-openapi.yml
  format: yaml
  label: lemlist Team API
  slug: lemlist-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-team-api-openapi.yml
- filename: lemlist-users-api-openapi.yml
  format: yaml
  label: lemlist Users API
  slug: lemlist-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-users-api-openapi.yml
- filename: lemlist-email-accounts-api-openapi.yml
  format: yaml
  label: lemlist Email Accounts API
  slug: lemlist-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-email-accounts-api-openapi.yml
- filename: lemlist-lemwarm-api-openapi.yml
  format: yaml
  label: lemlist lemwarm API
  slug: lemlist-lemwarm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-lemwarm-api-openapi.yml
- filename: lemlist-deliverability-alerts-api-openapi.yml
  format: yaml
  label: lemlist Deliverability Alerts API
  slug: lemlist-deliverability-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-deliverability-alerts-api-openapi.yml
- filename: lemlist-fields-api-openapi.yml
  format: yaml
  label: lemlist Fields API
  slug: lemlist-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-fields-api-openapi.yml
auth_types:
- http
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Lemlist Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: lemlist secures its APIs with http, apiKey, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: lemlist
provider_slug: lemlist
scheme_count: 4
schemes:
- description: 'HTTP Basic. The login is always empty and the password is the lemlist API key — Authorization: Basic base64(":YOUR_API_KEY"). The leading colon is required.'
  key_provisioning: app.lemlist.com > Settings > Team > Integrations > Generate
  name: basicAuth
  scheme: basic
  scoping: one API key resolves to exactly one lemlist team/account
  sources:
  - openapi/_original/lemlist-openapi-v2.json
  - https://developer.lemlist.com/api-reference/getting-started/authentication
  surface: REST API (https://api.lemlist.com/api)
  type: http
- description: The same lemlist API key, passed as an X-API-Key header to the MCP endpoint instead of Basic auth.
  in: header
  name: apiKeyHeader
  parameter_name: X-API-Key
  sources:
  - https://developer.lemlist.com/mcp/setup
  surface: MCP server (https://app.lemlist.com/mcp)
  type: apiKey
- authorization_endpoint: https://app.lemlist.com/oauth/authorize
  description: OAuth 2.1 authorization-code flow with PKCE (S256) and dynamic client registration. The consent screen asks the user to pick a team, so one grant binds to one account. Access tokens last 1 hour, refresh tokens 30 days.
  flows:
  - code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
  issuer: https://app.lemlist.com
  jwks_uri: https://app.lemlist.com/.well-known/jwks.json
  name: oauth2
  registration_endpoint: https://app.lemlist.com/oauth/register
  revocation_endpoint: https://app.lemlist.com/oauth/revoke
  scopes: see scopes/lemlist-scopes.yml (14 published)
  sources:
  - https://app.lemlist.com/.well-known/oauth-authorization-server
  surface: MCP server + CLI
  token_endpoint: https://app.lemlist.com/oauth/token
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
- description: OIDC discovery is served alongside the OAuth metadata. id_token signing RS256, subject type public, userinfo at https://app.lemlist.com/oauth/userinfo.
  name: openIdConnect
  openIdConnectUrl: https://app.lemlist.com/.well-known/openid-configuration
  sources:
  - https://app.lemlist.com/.well-known/openid-configuration
  surface: MCP server + CLI
  type: openIdConnect
slug: lemlist-authentication
source_filename: lemlist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.lemlist.com/api-reference/getting-started/authentication\ndocs:\n- https://developer.lemlist.com/api-reference/getting-started/authentication\n- https://developer.lemlist.com/api-reference/getting-started/multiple-accounts\n- https://developer.lemlist.com/cli/authentication\n- https://developer.lemlist.com/mcp/setup\nprobed:\n- url: https://app.lemlist.com/.well-known/oauth-authorization-server\n  status: 200\n- url: https://app.lemlist.com/.well-known/openid-configuration\n  status: 200\n- url: https://app.lemlist.com/.well-known/oauth-protected-resource\n  status: 200\n- url: https://api.lemlist.com/.well-known/oauth-authorization-server\n  status: 200\nnote: >-\n  lemlist runs two distinct authentication models on two surfaces. The REST API at\n  api.lemlist.com is API-key only, carried as HTTP Basic with an EMPTY username and\n  the key as the password. The MCP server and the CLI additionally accept OAuth\
  \ 2.1\n  (authorization code + PKCE, with dynamic client registration), whose metadata is\n  served anonymously from lemlist's own /.well-known/ endpoints. Bearer tokens are\n  explicitly NOT accepted by the REST API — lemlist's own Agent Skill says so.\nsummary:\n  types:\n  - http\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  pkce: S256\n  dynamic_client_registration: true\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  surface: REST API (https://api.lemlist.com/api)\n  description: >-\n    HTTP Basic. The login is always empty and the password is the lemlist API key —\n    Authorization: Basic base64(\":YOUR_API_KEY\"). The leading colon is required.\n  key_provisioning: 'app.lemlist.com > Settings > Team > Integrations > Generate'\n  scoping: one API key resolves to exactly one lemlist team/account\n  sources:\n  - openapi/_original/lemlist-openapi-v2.json\n  - https://developer.lemlist.com/api-reference/getting-started/authentication\n\
  - name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  surface: MCP server (https://app.lemlist.com/mcp)\n  description: The same lemlist API key, passed as an X-API-Key header to the MCP\n    endpoint instead of Basic auth.\n  sources:\n  - https://developer.lemlist.com/mcp/setup\n- name: oauth2\n  type: oauth2\n  surface: MCP server + CLI\n  description: >-\n    OAuth 2.1 authorization-code flow with PKCE (S256) and dynamic client registration.\n    The consent screen asks the user to pick a team, so one grant binds to one account.\n    Access tokens last 1 hour, refresh tokens 30 days.\n  issuer: https://app.lemlist.com\n  authorization_endpoint: https://app.lemlist.com/oauth/authorize\n  token_endpoint: https://app.lemlist.com/oauth/token\n  revocation_endpoint: https://app.lemlist.com/oauth/revoke\n  registration_endpoint: https://app.lemlist.com/oauth/register\n  jwks_uri: https://app.lemlist.com/.well-known/jwks.json\n  flows:\n  - flow: authorizationCode\n\
  \    grant_types:\n    - authorization_code\n    - refresh_token\n    code_challenge_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  scopes: see scopes/lemlist-scopes.yml (14 published)\n  sources:\n  - https://app.lemlist.com/.well-known/oauth-authorization-server\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://app.lemlist.com/.well-known/openid-configuration\n  surface: MCP server + CLI\n  description: >-\n    OIDC discovery is served alongside the OAuth metadata. id_token signing RS256,\n    subject type public, userinfo at https://app.lemlist.com/oauth/userinfo.\n  sources:\n  - https://app.lemlist.com/.well-known/openid-configuration\nmulti_account:\n  supported: true\n  model: one credential per team; agencies store one profile per client team\n  docs: https://developer.lemlist.com/api-reference/getting-started/multiple-accounts\n  cli_support: 'lemlist auth login <profile> / lemlist auth use <profile> / --account\n\
  \    <name> / LEMLIST_PROFILE'\nerrors:\n  '401': Unauthorized — authentication is missing or invalid\n  '403': Forbidden — user is blocked\n  '400': Bad Request — includes \"Bad team\", an invalid or inaccessible team for this\n    key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/authentication/lemlist-authentication.yml
summary_line: http/apiKey/oauth2/openIdConnect · 4 schemes
tags:
- Email Outreach
- Sales Engagement
- Cold Email
- Sales Automation
- LinkedIn Outreach
- Lead Generation
- Data Enrichment
- Deliverability
- CRM
- Multichannel Messaging
- Webhook
- MCP
---
