---
api_key_in:
- cookie
- header
api_specs:
- filename: redocly-search-api-openapi.yaml
  format: yaml
  label: Redocly Realm Search API
  slug: redocly-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-search-api-openapi.yaml
- filename: redocly-docs-mcp-openapi.yaml
  format: yaml
  label: Redocly Docs MCP Server
  slug: redocly-docs-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-docs-mcp-openapi.yaml
- filename: redocly-scout-openapi.yaml
  format: yaml
  label: Redocly Scout API
  slug: redocly-scout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-scout-openapi.yaml
- filename: redocly-scout-agent-openapi.yaml
  format: yaml
  label: Redocly Scout Agent API
  slug: redocly-scout-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-scout-agent-openapi.yaml
auth_types:
- apiKey
- http
- oauth2
description: Redocly authenticates on three different planes. Reunite/Realm organizations issue long-lived API keys used against the Redocly platform API and the Scout tool; the Docs MCP server on a Realm project uses OAuth 2.0 authorization code against per-project endpoints and validates the token's aud claim against the organization ID; and the Scout worker authenticates inbound GitHub/GitLab webhooks by signature header. Redocly's own docs project is public, so its Search API and Docs MCP server accept anonymous requests.
kind: authentication
layout: security
method: searched
name: Redocly Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Redocly secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Redocly
provider_slug: redocly
scheme_count: 5
schemes:
- flows:
  - authorizationUrl: https://{projectHost}/_mcp/oauth2/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://{projectHost}/_mcp/oauth2/token-portal
  name: OAuth2
  sources:
  - openapi/redocly-docs-mcp-openapi.yaml
  type: oauth2
- in: header
  name: GithubApiKey
  parameter: x-hub-signature-256
  sources:
  - openapi/redocly-scout-agent-openapi.yaml
  type: apiKey
- in: header
  name: GitlabApiKey
  parameter: x-gitlab-token
  sources:
  - openapi/redocly-scout-agent-openapi.yaml
  type: apiKey
- description: Default authentication scheme for interaction between browser and API.
  in: cookie
  name: UserCookie
  parameter: accessToken
  sources:
  - openapi/redocly-scout-openapi.yaml
  type: apiKey
- description: 'API key is required to access the API.

    You can get your API key from the [BlueHarvest dashboard](https://app.blueharvest.cloud).'
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/redocly-scout-openapi.yaml
  type: http
slug: redocly-authentication
source_filename: redocly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: openapi/*.yaml securitySchemes, enriched from https://redocly.com/docs/realm/reunite/organization/api-keys\n  and https://redocly.com/docs/realm/customization/mcp-server (fetched 2026-08-27)\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{projectHost}/_mcp/oauth2/auth\n    tokenUrl: https://{projectHost}/_mcp/oauth2/token-portal\n    scopes: 0\n  sources:\n  - openapi/redocly-docs-mcp-openapi.yaml\n- name: GithubApiKey\n  type: apiKey\n  in: header\n  parameter: x-hub-signature-256\n  sources:\n  - openapi/redocly-scout-agent-openapi.yaml\n- name: GitlabApiKey\n  type: apiKey\n  in: header\n  parameter: x-gitlab-token\n  sources:\n  - openapi/redocly-scout-agent-openapi.yaml\n- name: UserCookie\n  type: apiKey\n  in: cookie\n  parameter:\
  \ accessToken\n  description: Default authentication scheme for interaction between browser and API.\n  sources:\n  - openapi/redocly-scout-openapi.yaml\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: 'API key is required to access the API.\n\n    You can get your API key from the [BlueHarvest dashboard](https://app.blueharvest.cloud).'\n  sources:\n  - openapi/redocly-scout-openapi.yaml\ndocs: https://redocly.com/docs/realm/reunite/organization/api-keys\nprovider: Redocly\nproviderId: redocly\ndescription: Redocly authenticates on three different planes. Reunite/Realm organizations issue long-lived\n  API keys used against the Redocly platform API and the Scout tool; the Docs MCP server on a Realm project\n  uses OAuth 2.0 authorization code against per-project endpoints and validates the token's aud claim\n  against the organization ID; and the Scout worker authenticates inbound GitHub/GitLab webhooks by signature\n  header. Redocly's own docs project is public, so its\
  \ Search API and Docs MCP server accept anonymous\n  requests.\napi_keys:\n  docs: https://redocly.com/docs/realm/reunite/organization/api-keys\n  storage: Redocly stores API keys as one-way cryptographic hashes; the plaintext value cannot be retrieved\n    after creation.\n  expiration: Optional expiration date in UTC; a key with no expiry stays valid until manually revoked.\n  ip_restriction: Keys can be restricted to one or more allowed IP addresses on plans that include IP\n    restrictions.\n  permission_models:\n  - name: Granular permissions\n    description: Individually selected organization and project permissions; at least one must be selected.\n      Permission types are read, write and delete.\n  - name: RBAC\n    description: The key is assigned to one or more teams and inherits their roles, following the same\n      RBAC logic as users.\n  - name: Legacy full access\n    description: Read-only model shown for older unrestricted keys. New keys cannot use it; saving a legacy\n\
  \      key requires converting it to Granular or RBAC.\n  used_for:\n  - Redocly platform API\n  - Redocly Scout\noauth:\n  docs: https://redocly.com/docs/realm/customization/mcp-server\n  flow: authorization_code\n  authorization_url: https://{projectHost}/_mcp/oauth2/auth\n  token_url: https://{projectHost}/_mcp/oauth2/token-portal\n  audience_validation: The Docs MCP server compares the bearer token's aud claim to the organization ID.\n    Off by default; REDOCLY_MCP_ENFORCE_TOKEN_AUDIENCE=true rejects mismatches with 401. Tokens with no\n    aud claim skip the check.\n  dynamic_client_registration: Realm/Reef advertise dynamic client registration and Client ID Metadata\n    Document (CIMD) support for developer onboarding.\nsso:\n  docs: https://redocly.com/security\n  methods:\n  - SAML 2.0\n  - OpenID Connect\n  note: Enterprise SSO with domain verification, team mapping from IdP attributes, and project-level roles\n    and permissions.\nanonymous_surfaces:\n- surface: https://redocly.com/mcp\n\
  \  note: Docs MCP server; anonymous tools/list returned 200 on 2026-08-27 because redocly.com is a public\n    project.\n- surface: POST /_search on a public Realm project\n  note: The Search API needs no auth on public projects; protected projects use the browser session cookie\n    only — it accepts no API key or bearer token.\nnotes:\n- The ApiKey scheme in openapi/redocly-scout-openapi.yaml carries a legacy description pointing at app.blueharvest.cloud.\n  Title, contact (team@redocly.com), termsOfService and the docs location all name Redocly; the BlueHarvest\n  string is a stale reference inside one scheme description, not a different owner.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/authentication/redocly-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Artificial Intelligence
- API Catalog
- API Documentation
- Arazzo
- Developer Portal
- Governance
- Linting
- MCP
- Monitoring
- OpenAPI
---
