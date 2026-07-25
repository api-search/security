---
api_key_in: []
api_specs:
- filename: fixture-accounts-api-openapi.yml
  format: yaml
  label: Fixture Accounts API
  slug: fixture-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-accounts-api-openapi.yml
- filename: fixture-activities-api-openapi.yml
  format: yaml
  label: Fixture Activities API
  slug: fixture-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-activities-api-openapi.yml
- filename: fixture-contacts-api-openapi.yml
  format: yaml
  label: Fixture Contacts API
  slug: fixture-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-contacts-api-openapi.yml
- filename: fixture-deals-api-openapi.yml
  format: yaml
  label: Fixture Deals API
  slug: fixture-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-deals-api-openapi.yml
- filename: fixture-fixture-api-api-openapi.yml
  format: yaml
  label: Fixture Fixture API API
  slug: fixture-fixture-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-fixture-api-api-openapi.yml
- filename: fixture-leads-api-openapi.yml
  format: yaml
  label: Fixture Leads API
  slug: fixture-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-leads-api-openapi.yml
- filename: fixture-notes-api-openapi.yml
  format: yaml
  label: Fixture Notes API
  slug: fixture-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-notes-api-openapi.yml
- filename: fixture-pipelines-api-openapi.yml
  format: yaml
  label: Fixture Pipelines API
  slug: fixture-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-pipelines-api-openapi.yml
- filename: fixture-task-statuses-api-openapi.yml
  format: yaml
  label: Fixture Task Statuses API
  slug: fixture-task-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-task-statuses-api-openapi.yml
- filename: fixture-tasks-api-openapi.yml
  format: yaml
  label: Fixture Tasks API
  slug: fixture-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-tasks-api-openapi.yml
- filename: fixture-users-api-openapi.yml
  format: yaml
  label: Fixture Users API
  slug: fixture-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-users-api-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fixture Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fixture secures its APIs with http, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fixture
provider_slug: fixture
scheme_count: 3
schemes:
- bearerFormat: API key or OAuth access token
  description: Send either a Fixture API key or a Fixture OAuth access token in the Authorization header as a bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fixture-v1-openapi.json
  - https://fixture.app/docs/api-reference/overview
  type: http
- description: Workspace API keys are the service-to-service credential for external integrations. Owner-only to list, create, or revoke. Shown once at creation; scopes are chosen explicitly at creation time with no implicit full-access default. Revocation is immediate and permanent.
  docs: https://fixture.app/docs/authentication/api-keys
  header: Authorization
  in: header
  key_prefix: fx_
  name: api-key
  sources:
  - https://fixture.app/docs/authentication/api-keys
  type: apiKey
  used_by: External integrations and service jobs
  value_format: Bearer [example key]
- code_challenge_methods_supported:
  - S256
  description: Fixture OAuth is used by first-party Agent and CLI clients and by remote MCP clients. Authorization Server metadata is published at /.well-known/oauth-authorization-server on the API host, and the MCP endpoint publishes /.well-known/oauth-protected-resource. Public clients with PKCE S256; dynamic client registration is supported.
  endpoints:
    authorization: https://beta-api.fixture.app/api/oauth/authorize
    registration: https://beta-api.fixture.app/api/oauth/register
    revocation: https://beta-api.fixture.app/api/oauth/revoke
    token: https://beta-api.fixture.app/api/oauth/token
  flows:
    authorizationCode:
      authorizationUrl: https://beta-api.fixture.app/api/oauth/authorize
      refreshUrl: https://beta-api.fixture.app/api/oauth/token
      scopes:
        crm:read: Read CRM records
        crm:write: Create and update CRM records
        tasks:read: Read Tasks
        tasks:write: Create and update Tasks
        users:read: Read team Users
      tokenUrl: https://beta-api.fixture.app/api/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://beta-api.fixture.app
  name: fixture-oauth
  response_types_supported:
  - code
  sources:
  - https://beta-api.fixture.app/.well-known/oauth-authorization-server
  - https://beta-api.fixture.app/.well-known/oauth-protected-resource
  - https://fixture.app/docs/guides/agents/fixture-mcp
  token_endpoint_auth_methods_supported:
  - none
  token_format: JWT-shaped bearer (eyJ...)
  type: oauth2
  used_by: Fixture CLI, in-app Agent clients, and remote MCP clients
slug: fixture-authentication
source_filename: fixture-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://fixture.app/docs/authentication/api-keys, https://fixture.app/docs/authentication/scopes,\n  https://fixture.app/docs/api-reference/overview, https://beta-api.fixture.app/.well-known/oauth-authorization-server,\n  openapi/fixture-v1-openapi.json\ndocs: https://fixture.app/docs/authentication/api-keys\nsummary:\n  types:\n  - http\n  - apiKey\n  - oauth2\n  transport: Authorization header, bearer token only\n  session_cookies_accepted: false\n  notes: Session cookies are explicitly not accepted on /api/v1/*. Every request must carry\n    an Authorization bearer header, or the API returns 401 unauthorized.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key or OAuth access token\n  description: Send either a Fixture API key or a Fixture OAuth access token in the Authorization\n    header as a bearer token.\n  sources:\n  - openapi/fixture-v1-openapi.json\n  - https://fixture.app/docs/api-reference/overview\n\
  - name: api-key\n  type: apiKey\n  in: header\n  header: Authorization\n  value_format: Bearer [example key]\n  key_prefix: fx_\n  description: Workspace API keys are the service-to-service credential for external integrations.\n    Owner-only to list, create, or revoke. Shown once at creation; scopes are chosen explicitly\n    at creation time with no implicit full-access default. Revocation is immediate and permanent.\n  used_by: External integrations and service jobs\n  docs: https://fixture.app/docs/authentication/api-keys\n  sources:\n  - https://fixture.app/docs/authentication/api-keys\n- name: fixture-oauth\n  type: oauth2\n  description: Fixture OAuth is used by first-party Agent and CLI clients and by remote MCP\n    clients. Authorization Server metadata is published at /.well-known/oauth-authorization-server\n    on the API host, and the MCP endpoint publishes /.well-known/oauth-protected-resource.\n    Public clients with PKCE S256; dynamic client registration is supported.\n\
  \  issuer: https://beta-api.fixture.app\n  flows:\n    authorizationCode:\n      authorizationUrl: https://beta-api.fixture.app/api/oauth/authorize\n      tokenUrl: https://beta-api.fixture.app/api/oauth/token\n      refreshUrl: https://beta-api.fixture.app/api/oauth/token\n      scopes:\n        crm:read: Read CRM records\n        crm:write: Create and update CRM records\n        tasks:read: Read Tasks\n        tasks:write: Create and update Tasks\n        users:read: Read team Users\n  endpoints:\n    authorization: https://beta-api.fixture.app/api/oauth/authorize\n    token: https://beta-api.fixture.app/api/oauth/token\n    revocation: https://beta-api.fixture.app/api/oauth/revoke\n    registration: https://beta-api.fixture.app/api/oauth/register\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - none\n  code_challenge_methods_supported:\n  - S256\n  token_format: JWT-shaped bearer\
  \ (eyJ...)\n  used_by: Fixture CLI, in-app Agent clients, and remote MCP clients\n  sources:\n  - https://beta-api.fixture.app/.well-known/oauth-authorization-server\n  - https://beta-api.fixture.app/.well-known/oauth-protected-resource\n  - https://fixture.app/docs/guides/agents/fixture-mcp\nfailure_modes:\n- status: 401\n  code: unauthorized\n  when: Missing or invalid bearer token.\n- status: 403\n  code: forbidden\n  when: Valid bearer token but missing the required scope. Message names the missing scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/authentication/fixture-authentication.yml
summary_line: http/apiKey/oauth2 · 3 schemes
tags:
- Company
- CRM
- Sales
- B2B
- Artificial Intelligence
- Agents
- MCP
- Customer Relationship Management
---
