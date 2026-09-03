---
api_key_in: []
api_specs:
- filename: tray-ai-authentication-api-openapi.yml
  format: yaml
  label: Tray.ai Authentication API
  slug: tray-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-authentication-api-openapi.yml
- filename: tray-ai-authentications-api-openapi.yml
  format: yaml
  label: Tray.ai Authentications API
  slug: tray-ai-authentications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-authentications-api-openapi.yml
- filename: tray-ai-call-connector-api-openapi.yml
  format: yaml
  label: Tray.ai Call Connector API
  slug: tray-ai-call-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-call-connector-api-openapi.yml
- filename: tray-ai-connectors-api-openapi.yml
  format: yaml
  label: Tray.ai Connectors API
  slug: tray-ai-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-connectors-api-openapi.yml
- filename: tray-ai-deployments-api-openapi.yml
  format: yaml
  label: Tray.ai Deployments API
  slug: tray-ai-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-deployments-api-openapi.yml
- filename: tray-ai-projects-api-openapi.yml
  format: yaml
  label: Tray.ai Projects API
  slug: tray-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-projects-api-openapi.yml
- filename: tray-ai-solution-instances-api-openapi.yml
  format: yaml
  label: Tray.ai Solution Instances API
  slug: tray-ai-solution-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-solution-instances-api-openapi.yml
- filename: tray-ai-solutions-api-openapi.yml
  format: yaml
  label: Tray.ai Solutions API
  slug: tray-ai-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-solutions-api-openapi.yml
- filename: tray-ai-triggers-api-openapi.yml
  format: yaml
  label: Tray.ai Triggers API
  slug: tray-ai-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-triggers-api-openapi.yml
- filename: tray-ai-users-api-openapi.yml
  format: yaml
  label: Tray.ai Users API
  slug: tray-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-users-api-openapi.yml
- filename: tray-ai-workflows-api-openapi.yml
  format: yaml
  label: Tray.ai Workflows API
  slug: tray-ai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-workflows-api-openapi.yml
- filename: tray-ai-workspaces-api-openapi.yml
  format: yaml
  label: Tray.ai Workspaces API
  slug: tray-ai-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-workspaces-api-openapi.yml
auth_types:
- http
- oauth2
description: 'Tray.ai has two authentication models on one platform, and they do not overlap. The REST Platform API and the GraphQL Embedded API take a bearer token and have NO scope surface — authority comes from the token TYPE (master vs user) and from the RBAC role attached to the API user. The MCP server is a separate, modern OAuth 2.1 surface with dynamic client registration, PKCE S256 and three real scopes. A third layer sits underneath both: the per-service AUTHENTICATIONS Tray stores on behalf of end users, which is what a connector call actually executes under.'
kind: authentication
layout: security
method: searched
name: Tray Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tray.ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tray.ai
provider_slug: tray-ai
scheme_count: 2
schemes:
- applies_to:
  - Tray.ai Platform API
  - Tray.ai Embedded API
  bearerFormat: JWT
  description: Use either a master token (obtained from Tray Embedded UI settings / API Users & Tokens) or a user token (obtained via the Embedded authorize mutation). Master tokens are required for admin operations like managing users. User tokens are required for user-scoped operations like managing solution instances.
  name: bearerAuth
  scheme: bearer
  scopes: none
  sources:
  - openapi/_original/tray-ai-platform-api-published-openapi.yaml
  - openapi/_original/tray-ai-embedded-api-published-openapi.yaml
  type: http
- applies_to:
  - Tray MCP Server
  authorization_endpoint: https://auth.tray.io/server/oauth2/authorize
  cross_ref: scopes/tray-ai-scopes.yml
  flow: authorization_code
  issuer: https://auth.tray.io
  metadata: https://api.tray.io/.well-known/oauth-authorization-server
  name: trayMcpOAuth
  pkce: S256 (required; plain not offered)
  refresh: supported
  registration_endpoint: https://auth.tray.io/server/oauth2/register
  resource_metadata: https://api.tray.io/.well-known/oauth-protected-resource/mcp
  revocation_endpoint: https://auth.tray.io/server/oauth2/revoke
  scopes:
  - mcp:list_tools
  - mcp:call_tools
  - api:full
  token_endpoint: https://auth.tray.io/server/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - none
  type: oauth2
  verified: probed
slug: tray-ai-authentication
source_filename: tray-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://tray.ai/documentation/developer/getting-started/prerequisites/master-and-user-tokens,\n  https://tray.ai/documentation/platform/enterprise-core/organisation-management/api-users-tokens,\n  https://tray.ai/documentation/platform/artificial-intelligence/agent-gateway/authentication-and-access,\n  https://api.tray.io/.well-known/oauth-authorization-server,\n  openapi/_original/tray-ai-platform-api-published-openapi.yaml,\n  openapi/_original/tray-ai-embedded-api-published-openapi.yaml\ndocs: https://tray.ai/documentation/developer/getting-started/prerequisites/master-and-user-tokens\nprovider: Tray.ai\nproviderId: tray-ai\ndescription: >-\n  Tray.ai has two authentication models on one platform, and they do not overlap. The REST Platform\n  API and the GraphQL Embedded API take a bearer token and have NO scope surface — authority comes\n  from the token TYPE (master vs user) and from the RBAC role attached to the\
  \ API user. The MCP\n  server is a separate, modern OAuth 2.1 surface with dynamic client registration, PKCE S256 and\n  three real scopes. A third layer sits underneath both: the per-service AUTHENTICATIONS Tray stores\n  on behalf of end users, which is what a connector call actually executes under.\nsummary:\n  types:\n    - http\n    - oauth2\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to: [Tray.ai Platform API, Tray.ai Embedded API]\n    description: >-\n      Use either a master token (obtained from Tray Embedded UI settings / API Users & Tokens) or a\n      user token (obtained via the Embedded authorize mutation). Master tokens are required for\n      admin operations like managing users. User tokens are required for user-scoped operations\n      like managing solution instances.\n    sources:\n      - openapi/_original/tray-ai-platform-api-published-openapi.yaml\n      - openapi/_original/tray-ai-embedded-api-published-openapi.yaml\n\
  \    scopes: none\n  - name: trayMcpOAuth\n    type: oauth2\n    applies_to: [Tray MCP Server]\n    flow: authorization_code\n    pkce: S256 (required; plain not offered)\n    issuer: https://auth.tray.io\n    authorization_endpoint: https://auth.tray.io/server/oauth2/authorize\n    token_endpoint: https://auth.tray.io/server/oauth2/token\n    registration_endpoint: https://auth.tray.io/server/oauth2/register\n    revocation_endpoint: https://auth.tray.io/server/oauth2/revoke\n    refresh: supported\n    token_endpoint_auth_methods: [client_secret_basic, none]\n    scopes: [mcp:list_tools, mcp:call_tools, api:full]\n    metadata: https://api.tray.io/.well-known/oauth-authorization-server\n    resource_metadata: https://api.tray.io/.well-known/oauth-protected-resource/mcp\n    verified: probed\n    cross_ref: scopes/tray-ai-scopes.yml\ntoken_types:\n  - name: master token\n    surface: [Platform API, Embedded API]\n    obtained_from: Tray Embedded UI settings / Organisation management >\
  \ API Users & Tokens\n    acts_as: the organization\n    required_for: creating end users, issuing user tokens, org-level administration\n    rotation: manual\n  - name: user token\n    surface: [Platform API, Embedded API]\n    obtained_from: 'Embedded `authorize` mutation (create-user-token), exchanged with a master token'\n    acts_as: one end user\n    required_for: user-scoped operations — the user's authentications and solution instances\n    guidance: >-\n      Mint server-side and hand only the user token to a browser. Never ship a master token to a\n      front end.\n  - name: RBAC API token\n    surface: [Platform API, CDK CLI, Tray Sync CLI]\n    obtained_from: API Users & Tokens (workspace or account scope)\n    acts_as: an API user with a role\n    required_for: 'tray-cdk deployments, tray-sync-cli pull/promote'\n    docs: https://tray.ai/documentation/platform/enterprise-core/organisation-management/api-users-tokens\n  - name: OAuth2 access token\n    surface: [Tray MCP Server]\n\
  \    obtained_from: https://auth.tray.io/server/oauth2/authorize\n    acts_as: the signed-in Tray user, in the workspace chosen at sign-in\n    required_for: tools/list and tools/call on api.tray.io/mcp\nend_user_authentications:\n  description: >-\n    Distinct from the tokens above. An \"authentication\" is a stored credential for a THIRD-PARTY\n    service (Salesforce, Slack, ...) that Tray holds on behalf of a user, identified by a UUID and\n    passed as `authId` on every connector call.\n  operations: [create-user-authentication, get-user-authentication, update-user-authentication, delete-user-authentication, get-full-authentication, get-service-environments]\n  graphql_operations: [get-authentications, create-authentication, delete-authentication]\n  collection_ui: 'Hosted auth dialog (popup) — see components/tray-ai-components.yml'\n  custom_oauth_apps: https://tray.ai/documentation/developer/getting-started/prerequisites/custom-oauth-apps\n  note: >-\n    Partners can white-label\
  \ these with their own OAuth apps so end users see the partner's brand on\n    the third-party consent screen, not Tray's.\nagent_gateway_layers:\n  client_authentication:\n    - method: OAuth2\n      note: Required for dynamic (user-provided) tool authentication. Tray currently names Claude Desktop as the supported OAuth2 client, with more expanding.\n    - method: API token\n      note: Static bearer; works with all MCP clients; cannot use dynamic authentication — tools must use service-account credentials.\n  tool_authentication:\n    - mode: service account\n      note: One shared credential for every execution of the tool, whoever triggered it.\n    - mode: dynamic (user-provided)\n      note: The end user authenticates with their own credentials at runtime; actions execute with their permissions and are auditable to them. Mapping is valid for 7 days.\n  access_management: >-\n    Only users explicitly added on the MCP server's Access Management tab can execute its tools —\n    workspace\
  \ membership alone is not sufficient.\n  docs: https://tray.ai/documentation/platform/artificial-intelligence/agent-gateway/authentication-and-access\nregions:\n  note: A token is region-bound. US api.tray.io / tray.io, EU api.eu1.tray.io / eu1.tray.io, APAC api.ap1.tray.io / ap1.tray.io.\ngaps:\n  - No OIDC discovery document — /.well-known/openid-configuration 404s on api.tray.io and auth.tray.io.\n  - No scopes on the REST or GraphQL surfaces; a master token is all-or-nothing.\n  - No documented token rotation or expiry policy for master and RBAC tokens.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/authentication/tray-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Automation
- Integration
- iPaaS
- AI Agents
- MCP
- Orchestration
- Workflow Automation
- Connectors
- Agent Gateway
- Embedded Integration
- Enterprise Automation
- Model Context Protocol
---
