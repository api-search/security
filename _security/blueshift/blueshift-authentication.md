---
api_key_in: []
api_specs:
- filename: blueshift-openapi.yml
  format: yaml
  label: Blueshift REST API
  slug: blueshift-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshift/refs/heads/main/openapi/blueshift-openapi.yml
auth_types:
- http
- oauth2
description: Blueshift runs two entirely separate authentication regimes. The REST API uses HTTP Basic with an API key as the username and an EMPTY password — no bearer tokens, no OAuth — and splits its surface across two key classes with different blast radii. The MCP server, by contrast, is a full OAuth 2.0 authorization-code deployment with PKCE, dynamic client registration and scoped access. An integrator reading only the API reference would not know the OAuth surface exists; it is documented in the help centre, not the developer portal.
kind: authentication
layout: security
method: searched
name: Blueshift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blueshift secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Blueshift
provider_slug: blueshift
scheme_count: 3
schemes:
- applies_to: Customer profiles, catalogs, campaigns, segments, custom user lists, templates, shared assets, promotions, external fetches, reports — 71 of the 81 published operations.
  credential: User API key (USER_API_KEY)
  name: user_api_auth
  note: 'Visible only to admin users in the Blueshift app. This is the high-privilege key: it can read and delete customer PII and mutate live campaigns.'
  password: empty
  scheme: basic
  sources:
  - openapi/blueshift-openapi.yml
  - https://developer.blueshift.com/reference/authorization-1
  surface: REST API
  type: http
  username: the API key
  who_can_generate: Admin users only
- applies_to: Event ingestion and supported live-content endpoints — 10 of the 81 published operations.
  credential: Event API key (EVENT_API_KEY)
  name: event_api_auth
  note: Deliberately low-privilege and visible to every role, because it is the key that ships in server-side event collectors. Using it against a User-API endpoint returns 401.
  password: empty
  scheme: basic
  sources:
  - openapi/blueshift-openapi.yml
  - https://developer.blueshift.com/reference/authorization-1
  surface: REST API
  type: http
  username: the API key
  who_can_generate: Any user role
- applies_to: https://app.getblueshift.com/mcp and https://app.eu.getblueshift.com/mcp
  dynamic_client_registration: https://app.getblueshift.com/oauth/register
  flows:
    authorization_code:
      authorization_url: https://app.getblueshift.com/oauth/authorize
      scopes: scopes/blueshift-scopes.yml
      token_url: https://app.getblueshift.com/oauth/token
    client_credentials:
      token_url: https://app.getblueshift.com/oauth/token
    refresh_token:
      token_url: https://app.getblueshift.com/oauth/token
  name: blueshift_mcp_oauth
  note: Discovered by probe, not from the API reference. The 401 challenge on tools/list carries a correct RFC 9728 resource_metadata pointer, so a compliant MCP client can bootstrap the whole flow with no configuration beyond the server URL.
  pkce: S256
  sources:
  - well-known/blueshift-app-oauth-authorization-server.json
  - well-known/blueshift-app-oauth-protected-resource.json
  - https://help.blueshift.com/hc/en-us/articles/49713147943187-The-Blueshift-MCP-Server-Beta
  surface: MCP server
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: blueshift-authentication
source_filename: blueshift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://developer.blueshift.com/reference/authorization-1 and\n  https://developer.blueshift.com/docs/generate-api-keys, reconciled against the\n  securitySchemes in openapi/blueshift-openapi.yml and the RFC 8414 /\n  RFC 9728 documents probed at well-known/.\ndescription: >-\n  Blueshift runs two entirely separate authentication regimes. The REST API uses\n  HTTP Basic with an API key as the username and an EMPTY password — no bearer\n  tokens, no OAuth — and splits its surface across two key classes with\n  different blast radii. The MCP server, by contrast, is a full OAuth 2.0\n  authorization-code deployment with PKCE, dynamic client registration and\n  scoped access. An integrator reading only the API reference would not know the\n  OAuth surface exists; it is documented in the help centre, not the developer\n  portal.\n\nsummary:\n  types:\n    - http\n    - oauth2\n  rest_scheme: HTTP Basic (API key as username,\
  \ empty password)\n  mcp_scheme: OAuth 2.0 authorization code with PKCE\n  bearer_supported: false\n  mtls: false\n  openid_connect: false\n\nschemes:\n  - name: user_api_auth\n    type: http\n    scheme: basic\n    surface: REST API\n    applies_to: >-\n      Customer profiles, catalogs, campaigns, segments, custom user lists,\n      templates, shared assets, promotions, external fetches, reports — 71 of\n      the 81 published operations.\n    credential: User API key (USER_API_KEY)\n    username: the API key\n    password: empty\n    who_can_generate: Admin users only\n    sources:\n      - openapi/blueshift-openapi.yml\n      - https://developer.blueshift.com/reference/authorization-1\n    note: >-\n      Visible only to admin users in the Blueshift app. This is the\n      high-privilege key: it can read and delete customer PII and mutate live\n      campaigns.\n\n  - name: event_api_auth\n    type: http\n    scheme: basic\n    surface: REST API\n    applies_to: >-\n      Event ingestion\
  \ and supported live-content endpoints — 10 of the 81\n      published operations.\n    credential: Event API key (EVENT_API_KEY)\n    username: the API key\n    password: empty\n    who_can_generate: Any user role\n    sources:\n      - openapi/blueshift-openapi.yml\n      - https://developer.blueshift.com/reference/authorization-1\n    note: >-\n      Deliberately low-privilege and visible to every role, because it is the\n      key that ships in server-side event collectors. Using it against a\n      User-API endpoint returns 401.\n\n  - name: blueshift_mcp_oauth\n    type: oauth2\n    surface: MCP server\n    applies_to: https://app.getblueshift.com/mcp and https://app.eu.getblueshift.com/mcp\n    flows:\n      authorization_code:\n        authorization_url: https://app.getblueshift.com/oauth/authorize\n        token_url: https://app.getblueshift.com/oauth/token\n        scopes: scopes/blueshift-scopes.yml\n      client_credentials:\n        token_url: https://app.getblueshift.com/oauth/token\n\
  \      refresh_token:\n        token_url: https://app.getblueshift.com/oauth/token\n    pkce: S256\n    dynamic_client_registration: https://app.getblueshift.com/oauth/register\n    token_endpoint_auth_methods:\n      - none\n      - client_secret_basic\n      - client_secret_post\n    sources:\n      - well-known/blueshift-app-oauth-authorization-server.json\n      - well-known/blueshift-app-oauth-protected-resource.json\n      - https://help.blueshift.com/hc/en-us/articles/49713147943187-The-Blueshift-MCP-Server-Beta\n    note: >-\n      Discovered by probe, not from the API reference. The 401 challenge on\n      tools/list carries a correct RFC 9728 resource_metadata pointer, so a\n      compliant MCP client can bootstrap the whole flow with no configuration\n      beyond the server URL.\n\nkey_management:\n  where: Blueshift app > Account Settings > API keys tab\n  docs: https://developer.blueshift.com/docs/generate-api-keys\n  rotation: >-\n    Documented as an operator responsibility\
  \ — \"rotate keys periodically and\n    revoke compromised keys immediately\". No published rotation API, no key\n    expiry, and no scoping or restriction of a User API key below full admin\n    reach.\n  guidance: >-\n    Blueshift's own docs warn against committing keys to source control,\n    embedding them in client-side code, or sharing them outside trusted systems.\n\nregions:\n  - region: US and rest of world\n    rest_base_url: https://api.getblueshift.com\n    mcp_url: https://app.getblueshift.com/mcp\n  - region: EU\n    rest_base_url: https://api.eu.getblueshift.com\n    mcp_url: https://app.eu.getblueshift.com/mcp\n\nregions_note: >-\n  The base URL must match the region the account is provisioned in or requests\n  fail. This is a common first-integration failure and is called out in the\n  authorization docs.\n\ngaps:\n  - >-\n    Only two key classes exist for the whole REST API, and the User API key is\n    all-or-nothing. There are no restricted or scoped REST keys, so\
  \ any\n    integration that needs to read a campaign report also holds the credential\n    that can delete customer records.\n  - >-\n    The REST API has no OAuth and no bearer-token option, so there is no\n    delegated or per-user authorization path for server-side integrations —\n    only the MCP server offers that.\n  - >-\n    Basic auth with an empty password means the credential travels in an\n    unsalted Base64 header on every request; there is no request signing and no\n    replay protection.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueshift/refs/heads/main/authentication/blueshift-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Customer Data Platform
- Customer Engagement
- Marketing Automation
- Cross-Channel Messaging
- Email
- SMS
- Push Notifications
- Segmentation
- Personalization
- Product Recommendations
- Event Tracking
- Product Catalog
- MarTech
- MCP
- agent-native
---
