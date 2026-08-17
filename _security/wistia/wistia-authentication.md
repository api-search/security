---
api_key_in: []
api_specs:
- filename: wistia-data-api-v1-openapi.yml
  format: yaml
  label: Wistia Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-data-api-v1-openapi.yml
- filename: wistia-data-api-2026-01-openapi.yml
  format: yaml
  label: Wistia Data API 2026-01
  slug: data-api-2026-01
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-data-api-2026-01-openapi.yml
- filename: wistia-data-api-modern-edge-openapi.yml
  format: yaml
  label: Wistia Data API (modern, edge)
  slug: data-api-modern-edge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-data-api-modern-edge-openapi.yml
- filename: wistia-asyncapi.yml
  format: yaml
  label: Wistia Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/asyncapi/wistia-asyncapi.yml
- filename: wistia-account-api-openapi.yml
  format: yaml
  label: Wistia Account API
  slug: wistia-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-account-api-openapi.yml
- filename: wistia-alloweddomains-api-openapi.yml
  format: yaml
  label: Wistia AllowedDomains API
  slug: wistia-alloweddomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-alloweddomains-api-openapi.yml
- filename: wistia-captions-api-openapi.yml
  format: yaml
  label: Wistia Captions API
  slug: wistia-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-captions-api-openapi.yml
- filename: wistia-channels-api-openapi.yml
  format: yaml
  label: Wistia Channels API
  slug: wistia-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-channels-api-openapi.yml
- filename: wistia-customizations-api-openapi.yml
  format: yaml
  label: Wistia Customizations API
  slug: wistia-customizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-customizations-api-openapi.yml
- filename: wistia-folders-api-openapi.yml
  format: yaml
  label: Wistia Folders API
  slug: wistia-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-folders-api-openapi.yml
- filename: wistia-medias-api-openapi.yml
  format: yaml
  label: Wistia Medias API
  slug: wistia-medias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-medias-api-openapi.yml
- filename: wistia-tags-api-openapi.yml
  format: yaml
  label: Wistia Tags API
  slug: wistia-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-tags-api-openapi.yml
- filename: wistia-tokens-api-openapi.yml
  format: yaml
  label: Wistia Tokens API
  slug: wistia-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-tokens-api-openapi.yml
- filename: wistia-webinars-api-openapi.yml
  format: yaml
  label: Wistia Webinars API
  slug: wistia-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-webinars-api-openapi.yml
auth_types:
- http
- oauth2
description: 'Wistia authenticates API and MCP traffic with bearer credentials over TLS. Two credential families exist: a long-lived account API access token created in Account Settings, and an OAuth 2.0 access token obtained on a user''s behalf. The published OpenAPI declares only the bearer scheme; the full OAuth surface — including RFC 7591 dynamic client registration, PKCE, and introspection/revocation — is declared in the live RFC 8414 / RFC 9728 discovery documents rather than in the spec, which is why an OpenAPI-only read of this provider understates its auth posture.'
kind: authentication
layout: security
method: searched
name: Wistia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wistia secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wistia
provider_slug: wistia
scheme_count: 4
schemes:
- description: 'API access token or OAuth access token sent as `Authorization: Bearer <token>`. This is the supported way to call the API and the only securityScheme declared in the published OpenAPI.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/wistia-data-api-2026-01-openapi.yml
  - openapi/wistia-data-api-modern-edge-openapi.yml
  - openapi/wistia-data-api-v1-openapi.yml
  - https://docs.wistia.com/docs/making-api-requests
  type: http
- description: HTTP Basic with the API token as the password. Historically supported and still present in the profile, but the docs name Bearer as "the supported way to access the API".
  name: basicAuth
  scheme: basic
  sources:
  - https://docs.wistia.com/docs/making-api-requests
  status: legacy
  type: http
- description: OAuth 2.0 authorization code (with PKCE S256), refresh_token, and client_credentials grants, issued by https://api.wistia.com. Discoverable anonymously via RFC 8414 and RFC 9728 metadata. Wistia's docs note OAuth2 is not enabled on all accounts by default.
  flows:
    authorizationCode:
      authorizationUrl: https://api.wistia.com/oauth/authorize
      pkce: S256
      refreshUrl: https://api.wistia.com/oauth/token
      tokenUrl: https://api.wistia.com/oauth/token
    clientCredentials:
      tokenUrl: https://api.wistia.com/oauth/token
  introspection_endpoint: https://api.wistia.com/oauth/introspect
  name: oauth2
  registration_endpoint: https://api.wistia.com/oauth/register
  revocation_endpoint: https://api.wistia.com/oauth/revoke
  scopes: ../scopes/wistia-scopes.yml
  sources:
  - well-known/wistia-oauth-authorization-server.json
  - well-known/wistia-oauth-protected-resource.json
  - https://docs.wistia.com/docs/authenticating-with-oauth2
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- description: The modern API exposes POST /expiring_token, which mints a short-lived token for sharing scenarios. Grouped by Wistia into the `sharing` MCP toolset.
  name: expiringAccessToken
  sources:
  - openapi/wistia-data-api-2026-01-openapi.yml
  type: derived-token
slug: wistia-authentication
source_filename: wistia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://docs.wistia.com/docs/making-api-requests,\n  https://docs.wistia.com/docs/authenticating-with-oauth2,\n  https://api.wistia.com/.well-known/oauth-authorization-server,\n  https://api.wistia.com/.well-known/oauth-protected-resource,\n  https://api.wistia.com/auth.md,\n  openapi/wistia-data-api-2026-01-openapi.yml\ndocs: https://docs.wistia.com/docs/making-api-requests\ndescription: >-\n  Wistia authenticates API and MCP traffic with bearer credentials over TLS. Two credential\n  families exist: a long-lived account API access token created in Account Settings, and an OAuth\n  2.0 access token obtained on a user's behalf. The published OpenAPI declares only the bearer\n  scheme; the full OAuth surface — including RFC 7591 dynamic client registration, PKCE, and\n  introspection/revocation — is declared in the live RFC 8414 / RFC 9728 discovery documents rather\n  than in the spec, which is why an OpenAPI-only read\
  \ of this provider understates its auth posture.\nsummary:\n  types:\n  - http\n  - oauth2\n  transport_required: TLS (https). The docs state plainly \"You must use SSL to access the API.\"\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API access token or OAuth access token sent as `Authorization: Bearer <token>`. This is the\n    supported way to call the API and the only securityScheme declared in the published OpenAPI.\n  sources:\n  - openapi/wistia-data-api-2026-01-openapi.yml\n  - openapi/wistia-data-api-modern-edge-openapi.yml\n  - openapi/wistia-data-api-v1-openapi.yml\n  - https://docs.wistia.com/docs/making-api-requests\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic with the API token as the password. Historically supported and still present in the\n    profile, but the docs name Bearer as \"the supported way to access the API\".\n  status: legacy\n  sources:\n  - https://docs.wistia.com/docs/making-api-requests\n\
  - name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization code (with PKCE S256), refresh_token, and client_credentials grants,\n    issued by https://api.wistia.com. Discoverable anonymously via RFC 8414 and RFC 9728 metadata.\n    Wistia's docs note OAuth2 is not enabled on all accounts by default.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://api.wistia.com/oauth/authorize\n      tokenUrl: https://api.wistia.com/oauth/token\n      refreshUrl: https://api.wistia.com/oauth/token\n      pkce: S256\n    clientCredentials:\n      tokenUrl: https://api.wistia.com/oauth/token\n  registration_endpoint: https://api.wistia.com/oauth/register\n  revocation_endpoint: https://api.wistia.com/oauth/revoke\n  introspection_endpoint: https://api.wistia.com/oauth/introspect\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  scopes: ../scopes/wistia-scopes.yml\n  sources:\n  - well-known/wistia-oauth-authorization-server.json\n\
  \  - well-known/wistia-oauth-protected-resource.json\n  - https://docs.wistia.com/docs/authenticating-with-oauth2\n- name: expiringAccessToken\n  type: derived-token\n  description: >-\n    The modern API exposes POST /expiring_token, which mints a short-lived token for sharing\n    scenarios. Grouped by Wistia into the `sharing` MCP toolset.\n  sources:\n  - openapi/wistia-data-api-2026-01-openapi.yml\nwebhook_authentication:\n  scheme: hmac\n  algorithm: HMAC-SHA256 hexdigest\n  header: X-Wistia-Signature\n  signed_payload: the raw POST body\n  secret: the `secret_key` configured on the webhook in Account Settings\n  source: https://docs.wistia.com/docs/webhooks\ntoken_management:\n  creation: https://account.wistia.com/account/api (API tab of Account Settings)\n  restriction: The API tokens page is accessible only to the Account Owner.\n  storage: >-\n    Since June 2024 tokens are stored hashed, not in plain text; a token is copyable only at the\n    moment it is created. Existing\
  \ tokens were migrated to the hashed scheme.\n  editable_permissions: true\n  source: https://docs.wistia.com/docs/wistia-deprecation-schedule\ndeprecated_methods:\n- method: query-parameter authentication\n  status: removed\n  date: '2022-07-30'\n  note: >-\n    Passing tokens or passwords in query parameters was deprecated 2022-07-30 with brownouts on\n    2022-06-30 and 2022-07-14. Bearer tokens replaced it.\n  source: https://docs.wistia.com/docs/wistia-deprecation-schedule\nagent_onboarding:\n  document: https://api.wistia.com/auth.md\n  local_copy: ../well-known/wistia-auth.md\n  note: >-\n    A machine-addressed auth runbook (\"You are an agent...\") walking discover → register →\n    authorize → use → refresh → revoke, citing RFC 7591, 7636, 7009, 8414 and 9728. Referenced from\n    the `agent_auth.skill` field of the authorization-server metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/authentication/wistia-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Video Hosting
- Video Marketing
- Video Analytics
- Lead Generation
- Webinars
- B2B Marketing
- Video Captions
- Localization
- MCP
- Media Management
---
