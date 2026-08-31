---
api_key_in: []
api_specs:
- filename: x-account-activity-api-openapi.yml
  format: yaml
  label: X Account Activity API
  slug: x-account-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-account-activity-api-openapi.yml
- filename: x-account-api-openapi.yml
  format: yaml
  label: X Account API
  slug: x-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-account-api-openapi.yml
- filename: x-activity-api-openapi.yml
  format: yaml
  label: X Activity API
  slug: x-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-activity-api-openapi.yml
- filename: x-articles-api-openapi.yml
  format: yaml
  label: X Articles API
  slug: x-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-articles-api-openapi.yml
- filename: x-bots-api-openapi.yml
  format: yaml
  label: X Bots API
  slug: x-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-bots-api-openapi.yml
- filename: x-broadcasts-api-openapi.yml
  format: yaml
  label: X Broadcasts API
  slug: x-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-broadcasts-api-openapi.yml
- filename: x-chat-api-openapi.yml
  format: yaml
  label: X Chat API
  slug: x-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-chat-api-openapi.yml
- filename: x-communities-api-openapi.yml
  format: yaml
  label: X Communities API
  slug: x-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-communities-api-openapi.yml
- filename: x-community-notes-api-openapi.yml
  format: yaml
  label: X Community Notes API
  slug: x-community-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-community-notes-api-openapi.yml
- filename: x-compliance-api-openapi.yml
  format: yaml
  label: X Compliance API
  slug: x-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-compliance-api-openapi.yml
- filename: x-connections-api-openapi.yml
  format: yaml
  label: X Connections API
  slug: x-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-connections-api-openapi.yml
- filename: x-direct-messages-api-openapi.yml
  format: yaml
  label: X Direct Messages API
  slug: x-direct-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-direct-messages-api-openapi.yml
- filename: x-general-api-openapi.yml
  format: yaml
  label: X General API
  slug: x-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-general-api-openapi.yml
- filename: x-lists-api-openapi.yml
  format: yaml
  label: X Lists API
  slug: x-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-lists-api-openapi.yml
- filename: x-media-api-openapi.yml
  format: yaml
  label: X Media API
  slug: x-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-media-api-openapi.yml
- filename: x-news-api-openapi.yml
  format: yaml
  label: X News API
  slug: x-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-news-api-openapi.yml
- filename: x-posts-api-openapi.yml
  format: yaml
  label: X Posts API
  slug: x-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-posts-api-openapi.yml
- filename: x-spaces-api-openapi.yml
  format: yaml
  label: X Spaces API
  slug: x-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-spaces-api-openapi.yml
- filename: x-stream-api-openapi.yml
  format: yaml
  label: X Stream API
  slug: x-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-stream-api-openapi.yml
- filename: x-trends-api-openapi.yml
  format: yaml
  label: X Trends API
  slug: x-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-trends-api-openapi.yml
- filename: x-usage-api-openapi.yml
  format: yaml
  label: X Usage API
  slug: x-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-usage-api-openapi.yml
- filename: x-users-api-openapi.yml
  format: yaml
  label: X Users API
  slug: x-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-users-api-openapi.yml
- filename: x-webhooks-api-openapi.yml
  format: yaml
  label: X Webhooks API
  slug: x-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/openapi/x-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: 'Authentication profile for the X API v2. Three schemes are declared in X''s published contract and all three are documented as first-class methods: app-only Bearer for read-only public data, OAuth 2.0 Authorization Code with PKCE for user context (required for every write), and legacy OAuth 1.0a user context. Enterprise endpoints additionally accept Basic Auth.'
kind: authentication
layout: security
method: searched
name: X Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: X secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: X
provider_slug: x
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://api.x.com/2/oauth2/authorize
    flow: authorizationCode
    scopes: 26
    tokenUrl: https://api.x.com/2/oauth2/token
  name: OAuth2UserToken
  sources:
  - openapi/x-account-activity-api-openapi.yml
  - openapi/x-account-api-openapi.yml
  - openapi/x-activity-api-openapi.yml
  - openapi/x-articles-api-openapi.yml
  - openapi/x-broadcasts-api-openapi.yml
  - openapi/x-chat-api-openapi.yml
  - openapi/x-communities-api-openapi.yml
  - openapi/x-community-notes-api-openapi.yml
  - openapi/x-direct-messages-api-openapi.yml
  - openapi/x-lists-api-openapi.yml
  - openapi/x-media-api-openapi.yml
  - openapi/x-news-api-openapi.yml
  - openapi/x-posts-api-openapi.yml
  - openapi/x-spaces-api-openapi.yml
  - openapi/x-trends-api-openapi.yml
  - openapi/x-usage-api-openapi.yml
  - openapi/x-users-api-openapi.yml
  type: oauth2
- name: BearerToken
  scheme: bearer
  sources:
  - openapi/x-account-activity-api-openapi.yml
  - openapi/x-activity-api-openapi.yml
  - openapi/x-bots-api-openapi.yml
  - openapi/x-communities-api-openapi.yml
  - openapi/x-compliance-api-openapi.yml
  - openapi/x-connections-api-openapi.yml
  - openapi/x-lists-api-openapi.yml
  - openapi/x-media-api-openapi.yml
  - openapi/x-news-api-openapi.yml
  - openapi/x-posts-api-openapi.yml
  - openapi/x-spaces-api-openapi.yml
  - openapi/x-stream-api-openapi.yml
  - openapi/x-trends-api-openapi.yml
  - openapi/x-usage-api-openapi.yml
  - openapi/x-users-api-openapi.yml
  - openapi/x-webhooks-api-openapi.yml
  type: http
- name: UserToken
  scheme: OAuth
  sources:
  - openapi/x-account-activity-api-openapi.yml
  - openapi/x-activity-api-openapi.yml
  - openapi/x-articles-api-openapi.yml
  - openapi/x-broadcasts-api-openapi.yml
  - openapi/x-chat-api-openapi.yml
  - openapi/x-communities-api-openapi.yml
  - openapi/x-community-notes-api-openapi.yml
  - openapi/x-direct-messages-api-openapi.yml
  - openapi/x-lists-api-openapi.yml
  - openapi/x-media-api-openapi.yml
  - openapi/x-news-api-openapi.yml
  - openapi/x-posts-api-openapi.yml
  - openapi/x-trends-api-openapi.yml
  - openapi/x-users-api-openapi.yml
  - openapi/x-webhooks-api-openapi.yml
  type: http
slug: x-authentication
source_filename: x-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://docs.x.com/fundamentals/authentication/overview + openapi/_original/x-api-v2-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2UserToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.x.com/2/oauth2/authorize\n    tokenUrl: https://api.x.com/2/oauth2/token\n    scopes: 26\n  sources:\n  - openapi/x-account-activity-api-openapi.yml\n  - openapi/x-account-api-openapi.yml\n  - openapi/x-activity-api-openapi.yml\n  - openapi/x-articles-api-openapi.yml\n  - openapi/x-broadcasts-api-openapi.yml\n  - openapi/x-chat-api-openapi.yml\n  - openapi/x-communities-api-openapi.yml\n  - openapi/x-community-notes-api-openapi.yml\n  - openapi/x-direct-messages-api-openapi.yml\n  - openapi/x-lists-api-openapi.yml\n  - openapi/x-media-api-openapi.yml\n  - openapi/x-news-api-openapi.yml\n  - openapi/x-posts-api-openapi.yml\n\
  \  - openapi/x-spaces-api-openapi.yml\n  - openapi/x-trends-api-openapi.yml\n  - openapi/x-usage-api-openapi.yml\n  - openapi/x-users-api-openapi.yml\n- name: BearerToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/x-account-activity-api-openapi.yml\n  - openapi/x-activity-api-openapi.yml\n  - openapi/x-bots-api-openapi.yml\n  - openapi/x-communities-api-openapi.yml\n  - openapi/x-compliance-api-openapi.yml\n  - openapi/x-connections-api-openapi.yml\n  - openapi/x-lists-api-openapi.yml\n  - openapi/x-media-api-openapi.yml\n  - openapi/x-news-api-openapi.yml\n  - openapi/x-posts-api-openapi.yml\n  - openapi/x-spaces-api-openapi.yml\n  - openapi/x-stream-api-openapi.yml\n  - openapi/x-trends-api-openapi.yml\n  - openapi/x-usage-api-openapi.yml\n  - openapi/x-users-api-openapi.yml\n  - openapi/x-webhooks-api-openapi.yml\n- name: UserToken\n  type: http\n  scheme: OAuth\n  sources:\n  - openapi/x-account-activity-api-openapi.yml\n  - openapi/x-activity-api-openapi.yml\n  - openapi/x-articles-api-openapi.yml\n\
  \  - openapi/x-broadcasts-api-openapi.yml\n  - openapi/x-chat-api-openapi.yml\n  - openapi/x-communities-api-openapi.yml\n  - openapi/x-community-notes-api-openapi.yml\n  - openapi/x-direct-messages-api-openapi.yml\n  - openapi/x-lists-api-openapi.yml\n  - openapi/x-media-api-openapi.yml\n  - openapi/x-news-api-openapi.yml\n  - openapi/x-posts-api-openapi.yml\n  - openapi/x-trends-api-openapi.yml\n  - openapi/x-users-api-openapi.yml\n  - openapi/x-webhooks-api-openapi.yml\ndocs: https://docs.x.com/fundamentals/authentication/overview\ndescription: 'Authentication profile for the X API v2. Three schemes are declared in X''s published contract\n  and all three are documented as first-class methods: app-only Bearer for read-only public data, OAuth\n  2.0 Authorization Code with PKCE for user context (required for every write), and legacy OAuth 1.0a\n  user context. Enterprise endpoints additionally accept Basic Auth.'\ndiscovery:\n  authorization_server: https://api.x.com/.well-known/oauth-authorization-server\n\
  \  authorization_server_status: 200\n  protected_resource: https://api.x.com/.well-known/oauth-protected-resource\n  protected_resource_status: 200\n  openid_connect: false\n  dynamic_client_registration: false\n  note: X serves RFC 8414 and RFC 9728 metadata but no OpenID Connect discovery document, and it documents\n    explicitly that api.x.com/mcp does not advertise native MCP OAuth discovery and has no dynamic client\n    registration — you must bring your own registered developer app.\nmethods:\n- name: App-only Bearer token\n  scheme: BearerToken\n  type: http\n  bearer: true\n  use: Read-only access to public data; no user context. Obtained from the app Keys and tokens page in\n    the Developer Console.\n  docs: https://docs.x.com/fundamentals/authentication/oauth-2-0/application-only\n- name: OAuth 2.0 Authorization Code with PKCE\n  scheme: OAuth2UserToken\n  type: oauth2\n  use: User context with granular scopes. Required for all writes and for the xurl MCP bridge.\n  scopes:\
  \ 29\n  detail: ../scopes/x-scopes.yml\n  docs: https://docs.x.com/fundamentals/authentication/oauth-2-0/authorization-code\n- name: OAuth 1.0a user context\n  scheme: UserToken\n  type: http\n  http_scheme: OAuth\n  use: Legacy signed-request user context, still supported for v2 and required by some v1.1 endpoints.\n  docs: https://docs.x.com/fundamentals/authentication/oauth-1-0a/api-key-and-secret\n- name: Basic Auth\n  scheme: null\n  type: http\n  use: Some Enterprise (GNIP lineage) endpoints only; not part of the v2 securitySchemes.\n  source: https://docs.x.com/AGENTS.md\ncredentials:\n  issued_by: https://console.x.com\n  test_credentials: false\n  note: One credential set per app; nothing distinguishes test from production. See ../sandbox/x-sandbox.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x/refs/heads/main/authentication/x-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Social
- Social-Media
- Posts
- User
- Direct Messages
- Streaming
- Webhook
- Real-Time
- Trends
- Media
- Spaces
- Content
- Conversation
- Agents
- MCP
---
