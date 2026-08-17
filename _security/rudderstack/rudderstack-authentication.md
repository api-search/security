---
api_key_in: []
api_specs:
- filename: rudderstack-event-streaming-asyncapi.yml
  format: yaml
  label: RudderStack Webhook Source API
  slug: rudderstack-webhook-source-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/asyncapi/rudderstack-event-streaming-asyncapi.yml
- filename: rudderstack-http-api-api-openapi.yml
  format: yaml
  label: RudderStack HTTP API API
  slug: rudderstack-http-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/openapi/rudderstack-http-api-api-openapi.yml
- filename: rudderstack-internal-api-api-openapi.yml
  format: yaml
  label: RudderStack Internal API API
  slug: rudderstack-internal-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/openapi/rudderstack-internal-api-api-openapi.yml
auth_types:
- http
- oauth2
description: 'RudderStack runs THREE distinct authentication regimes, one per plane. The data plane (event ingest) uses HTTP Basic with the source write key as the username and an empty password. The control plane at api.rudderstack.com uses a Bearer token — a workspace/organization Service Access Token (SAT) or, on Free and self-hosted plans, a user Personal Access Token (PAT). The hosted MCP server at mcp.rudderstack.com is an OAuth 2.0 protected resource with Dynamic Client Registration and PKCE. Conflating them is the most common integration error: a write key will not authenticate against api.rudderstack.com and a SAT will not authenticate an event POST.'
kind: authentication
layout: security
method: searched
name: Rudderstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: RudderStack secures its APIs with http and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RudderStack
provider_slug: rudderstack
scheme_count: 5
schemes:
- base: '{DATA_PLANE_URL}'
  description: 'Source write key as the HTTP Basic username with an empty password (`curl -u <source_write_key>: ...`). Scoped to a single source; it can only write events, never read or configure anything.'
  docs: https://www.rudderstack.com/docs/api/http-api/
  name: writeKeyAuth
  plane: data
  scheme: basic
  sources:
  - openapi/rudderstack-http-api-api-openapi.yml
  type: http
  used_by:
  - openapi/rudderstack-http-api-api-openapi.yml
  - openapi/rudderstack-internal-api-api-openapi.yml
  - Pixel API (write key passed as the `writeKey` query parameter on a GET)
- base: https://api.rudderstack.com
  description: Service Access Token. Issued at the organization or workspace level rather than being tied to a user, so it survives member removal and role changes. Organization-level SATs carry Admin permissions by default; workspace-level SATs are created under a configurable workspace SAT access policy. Only Admins can see the Service Access Tokens tab or create/delete tokens.
  docs: https://www.rudderstack.com/docs/access-management/service-access-tokens/
  header: 'Authorization: Bearer <SERVICE_ACCESS_TOKEN>'
  name: serviceAccessToken
  plane: control
  regional_base: https://api.eu.rudderstack.com
  scheme: bearer
  type: http
  used_by:
  - Data Catalog API
  - Tracking Plan API
  - Transformations API
  - Profiles API
  - Reverse ETL Connections API
  - Audit Logs API
  - Event Audit API
  - User Suppression API
  - Test API
  - rudder-cli (rudder-cli auth login)
- base: https://api.rudderstack.com
  description: Personal Access Token, tied to an individual user and their role. Documented as the token type for Free and self-hosted plans, and accepted by rudder-cli. Breaks when the user is removed or their permissions change — which is the stated reason SATs exist.
  docs: https://www.rudderstack.com/docs/access-management/personal-access-tokens/
  header: 'Authorization: Bearer <token>'
  name: personalAccessToken
  plane: control
  scheme: bearer
  type: http
- base: https://api.rudderstack.com
  description: OUTLIER. The Test API (/v0/testDestination/{destinationId}, /v0/testSource/{sourceId}) authenticates with HTTP Basic using an EMPTY username and the workspace Service Access Token as the PASSWORD — not the Bearer scheme every other control-plane API uses. A workspace SAT carries Read permissions by default and needs no additional resource permissions; on the legacy RBAC system the token needs at least Viewer.
  docs: https://www.rudderstack.com/docs/api/test-api/
  header: 'Authorization: Basic {Base64Encoded(:<SERVICE_ACCESS_TOKEN>)}'
  name: testApiBasic
  plane: control
  scheme: basic
  type: http
  used_by:
  - Test API
- artifacts:
  - well-known/rudderstack-mcp-oauth-authorization-server.json
  - well-known/rudderstack-mcp-oauth-protected-resource.json
  base: https://mcp.rudderstack.com
  description: OAuth 2.0 authorization_code + refresh_token with PKCE (S256) protecting the hosted MCP server. Dynamic Client Registration (RFC 7591) is advertised at /register, so an MCP client can self-register; the user then signs in with their existing RudderStack credentials and approves the integration. Discovery follows RFC 8414 and RFC 9728.
  docs: https://mcp.rudderstack.com/docs
  flows:
    authorization_code:
      authorization_url: https://mcp.rudderstack.com/authorize
      note: The authorization server metadata document declares no `scopes_supported` — see scopes/rudderstack-scopes.yml.
      registration_url: https://mcp.rudderstack.com/register
      scopes: {}
      token_url: https://mcp.rudderstack.com/token
  name: mcpOAuth
  plane: agent
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: rudderstack-authentication
source_filename: rudderstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://www.rudderstack.com/docs/access-management/service-access-tokens/,\n  https://www.rudderstack.com/docs/access-management/personal-access-tokens/,\n  https://www.rudderstack.com/docs/api/transformation-api/,\n  https://www.rudderstack.com/docs/api/http-api/,\n  https://mcp.rudderstack.com/.well-known/oauth-authorization-server, and\n  openapi/rudderstack-http-api-api-openapi.yml\ndocs: https://www.rudderstack.com/docs/access-management/\ndescription: >-\n  RudderStack runs THREE distinct authentication regimes, one per plane. The data\n  plane (event ingest) uses HTTP Basic with the source write key as the username\n  and an empty password. The control plane at api.rudderstack.com uses a Bearer\n  token — a workspace/organization Service Access Token (SAT) or, on Free and\n  self-hosted plans, a user Personal Access Token (PAT). The hosted MCP server at\n  mcp.rudderstack.com is an OAuth 2.0 protected resource\
  \ with Dynamic Client\n  Registration and PKCE. Conflating them is the most common integration error:\n  a write key will not authenticate against api.rudderstack.com and a SAT will\n  not authenticate an event POST.\nsummary:\n  types:\n    - http\n    - oauth2\n  planes: 3\nschemes:\n  - name: writeKeyAuth\n    plane: data\n    type: http\n    scheme: basic\n    base: '{DATA_PLANE_URL}'\n    description: >-\n      Source write key as the HTTP Basic username with an empty password\n      (`curl -u <source_write_key>: ...`). Scoped to a single source; it can only\n      write events, never read or configure anything.\n    used_by:\n      - openapi/rudderstack-http-api-api-openapi.yml\n      - openapi/rudderstack-internal-api-api-openapi.yml\n      - Pixel API (write key passed as the `writeKey` query parameter on a GET)\n    docs: https://www.rudderstack.com/docs/api/http-api/\n    sources:\n      - openapi/rudderstack-http-api-api-openapi.yml\n  - name: serviceAccessToken\n    plane:\
  \ control\n    type: http\n    scheme: bearer\n    base: https://api.rudderstack.com\n    regional_base: https://api.eu.rudderstack.com\n    header: 'Authorization: Bearer <SERVICE_ACCESS_TOKEN>'\n    description: >-\n      Service Access Token. Issued at the organization or workspace level rather\n      than being tied to a user, so it survives member removal and role changes.\n      Organization-level SATs carry Admin permissions by default; workspace-level\n      SATs are created under a configurable workspace SAT access policy. Only\n      Admins can see the Service Access Tokens tab or create/delete tokens.\n    docs: https://www.rudderstack.com/docs/access-management/service-access-tokens/\n    used_by:\n      - Data Catalog API\n      - Tracking Plan API\n      - Transformations API\n      - Profiles API\n      - Reverse ETL Connections API\n      - Audit Logs API\n      - Event Audit API\n      - User Suppression API\n      - Test API\n      - rudder-cli (rudder-cli auth login)\n\
  \  - name: personalAccessToken\n    plane: control\n    type: http\n    scheme: bearer\n    base: https://api.rudderstack.com\n    header: 'Authorization: Bearer <token>'\n    description: >-\n      Personal Access Token, tied to an individual user and their role. Documented\n      as the token type for Free and self-hosted plans, and accepted by rudder-cli.\n      Breaks when the user is removed or their permissions change — which is the\n      stated reason SATs exist.\n    docs: https://www.rudderstack.com/docs/access-management/personal-access-tokens/\n  - name: testApiBasic\n    plane: control\n    type: http\n    scheme: basic\n    base: https://api.rudderstack.com\n    header: 'Authorization: Basic {Base64Encoded(:<SERVICE_ACCESS_TOKEN>)}'\n    description: >-\n      OUTLIER. The Test API (/v0/testDestination/{destinationId},\n      /v0/testSource/{sourceId}) authenticates with HTTP Basic using an EMPTY\n      username and the workspace Service Access Token as the PASSWORD — not\
  \ the\n      Bearer scheme every other control-plane API uses. A workspace SAT carries\n      Read permissions by default and needs no additional resource permissions;\n      on the legacy RBAC system the token needs at least Viewer.\n    docs: https://www.rudderstack.com/docs/api/test-api/\n    used_by:\n      - Test API\n  - name: mcpOAuth\n    plane: agent\n    type: oauth2\n    base: https://mcp.rudderstack.com\n    description: >-\n      OAuth 2.0 authorization_code + refresh_token with PKCE (S256) protecting the\n      hosted MCP server. Dynamic Client Registration (RFC 7591) is advertised at\n      /register, so an MCP client can self-register; the user then signs in with\n      their existing RudderStack credentials and approves the integration.\n      Discovery follows RFC 8414 and RFC 9728.\n    flows:\n      authorization_code:\n        authorization_url: https://mcp.rudderstack.com/authorize\n        token_url: https://mcp.rudderstack.com/token\n        registration_url: https://mcp.rudderstack.com/register\n\
  \        scopes: {}\n        note: >-\n          The authorization server metadata document declares no `scopes_supported`\n          — see scopes/rudderstack-scopes.yml.\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    docs: https://mcp.rudderstack.com/docs\n    artifacts:\n      - well-known/rudderstack-mcp-oauth-authorization-server.json\n      - well-known/rudderstack-mcp-oauth-protected-resource.json\nenterprise:\n  sso:\n    supported: true\n    plans: [Enterprise]\n    providers_named: [Okta, OneLogin]\n    docs: https://www.rudderstack.com/security/\n  mfa:\n    supported: true\n    methods: [TOTP authenticator app, SMS, single-use backup codes]\n    since: '2026-08-05'\n    docs: https://www.rudderstack.com/docs/dashboard-guides/security/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/authentication/rudderstack-authentication.yml
summary_line: http/oauth2 · 5 schemes
tags:
- Customer Data Platform
- CDP
- Data Pipeline
- Open Source
- Event Streaming
- Reverse ETL
- Analytics
- Identity Resolution
---
