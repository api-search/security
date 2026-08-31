---
api_key_in:
- header
api_specs:
- filename: nooks-accounts-api-openapi.yml
  format: yaml
  label: Nooks Accounts API
  slug: nooks-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-accounts-api-openapi.yml
- filename: nooks-calldispositions-api-openapi.yml
  format: yaml
  label: Nooks Call Dispositions API
  slug: nooks-calldispositions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-calldispositions-api-openapi.yml
- filename: nooks-calls-api-openapi.yml
  format: yaml
  label: Nooks Calls API
  slug: nooks-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-calls-api-openapi.yml
- filename: nooks-emails-api-openapi.yml
  format: yaml
  label: Nooks Emails API
  slug: nooks-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-emails-api-openapi.yml
- filename: nooks-emailtemplates-api-openapi.yml
  format: yaml
  label: Nooks Email Templates API
  slug: nooks-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-emailtemplates-api-openapi.yml
- filename: nooks-introspection-api-openapi.yml
  format: yaml
  label: Nooks Introspection API
  slug: nooks-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-introspection-api-openapi.yml
- filename: nooks-mailboxes-api-openapi.yml
  format: yaml
  label: Nooks Mailboxes API
  slug: nooks-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-mailboxes-api-openapi.yml
- filename: nooks-nooks-sequencing-api-api-openapi.yml
  format: yaml
  label: Nooks Nooks Sequencing API
  slug: nooks-nooks-sequencing-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-nooks-sequencing-api-api-openapi.yml
- filename: nooks-notes-api-openapi.yml
  format: yaml
  label: Nooks Notes API
  slug: nooks-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-notes-api-openapi.yml
- filename: nooks-prospects-api-openapi.yml
  format: yaml
  label: Nooks Prospects API
  slug: nooks-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-prospects-api-openapi.yml
- filename: nooks-sequences-api-openapi.yml
  format: yaml
  label: Nooks Sequences API
  slug: nooks-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequences-api-openapi.yml
- filename: nooks-sequencestates-api-openapi.yml
  format: yaml
  label: Nooks Sequence States API
  slug: nooks-sequencestates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequencestates-api-openapi.yml
- filename: nooks-sequencesteps-api-openapi.yml
  format: yaml
  label: Nooks Sequence Steps API
  slug: nooks-sequencesteps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequencesteps-api-openapi.yml
- filename: nooks-tasks-api-openapi.yml
  format: yaml
  label: Nooks Tasks API
  slug: nooks-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-tasks-api-openapi.yml
- filename: nooks-users-api-openapi.yml
  format: yaml
  label: Nooks Users API
  slug: nooks-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nooks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nooks secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nooks
provider_slug: nooks
scheme_count: 1
schemes:
- applied: global
  description: Bearer token sent in the `Authorization` header. Accepts either a long-lived Nooks API key (`nooks-api-...`, from Developer Settings → API Keys) or an OAuth 2.0 access token issued by https://oauth.nooks.in. The API detects which format was sent and validates accordingly.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nooks-sequencing-openapi.yml
  type: http
slug: nooks-authentication
source_filename: nooks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/nooks-sequencing-openapi.yml\ndocs: https://developer.nooks.in/\nnote: >-\n  Derived from the OpenAPI securitySchemes, then upgraded from the spec's own Authentication\n  introduction and the live RFC 8414 authorization-server metadata at\n  https://oauth.nooks.in/.well-known/oauth-authorization-server. The spec declares a single\n  `BearerAuth` http/bearer scheme, but that one header carries TWO distinct credential types —\n  a long-lived workspace API key and a short-lived user-scoped OAuth 2.0 JWT — which the derived\n  pass could not see because Nooks does not model the OAuth flow as an `oauth2` securityScheme.\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  applied: global\n  description: >-\n    Bearer token sent in the `Authorization` header. Accepts either\
  \ a long-lived Nooks API key\n    (`nooks-api-...`, from Developer Settings → API Keys) or an OAuth 2.0 access token issued by\n    https://oauth.nooks.in. The API detects which format was sent and validates accordingly.\n  sources:\n  - openapi/nooks-sequencing-openapi.yml\ncredentials:\n- kind: api-key\n  name: Nooks API key\n  transport: Authorization Bearer header\n  prefix: nooks-api-\n  lifetime: long-lived\n  scoping: workspace-scoped, full read/write within the owning workspace\n  issuance: Developer Settings → API Keys in the Nooks workspace\n  best_for: backend integrations and server-to-server automation\n- kind: oauth2-access-token\n  name: OAuth 2.0 access token\n  transport: Authorization Bearer header\n  format: JWT\n  lifetime: 1 hour\n  scoping: user-scoped, limited to consented scopes\n  refresh: refresh tokens rotate every 90 days and are invalidated on first re-use (refresh-token reuse detection)\n  best_for: third-party apps acting on behalf of a specific user\noauth2:\n\
  \  issuer: https://oauth.nooks.in\n  discovery: well-known/nooks-oauth-authorization-server.json\n  discovery_url: https://oauth.nooks.in/.well-known/oauth-authorization-server\n  authorization_endpoint: https://oauth.nooks.in/oauth/authorize\n  token_endpoint: https://oauth.nooks.in/oauth/token\n  revocation_endpoint: https://oauth.nooks.in/oauth/revoke\n  jwks_uri: https://oauth.nooks.in/.well-known/jwks.json\n  jwks_file: well-known/nooks-jwks.json\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  code_challenge_methods_supported:\n  - S256\n  pkce: required (S256)\n  scope_count: 24\n  scopes: scopes/nooks-scopes.yml\nprotected_resources:\n- resource: https://mcp.nooks.in/\n  resource_name: Nooks MCP Server\n  metadata: well-known/nooks-oauth-protected-resource.json\n  metadata_url: https://mcp.nooks.in/.well-known/oauth-protected-resource\n  spec: RFC 9728\
  \ OAuth 2.0 Protected Resource Metadata\n  authorization_servers:\n  - https://oauth.nooks.in\nerrors:\n  '401': Unauthorized — missing, malformed, or expired credential\n  '403': Forbidden — credential valid but lacks the required scope or workspace access\nx-evidence:\n- url: https://developer.nooks.in/openapi.yml\n  status: 200\n- url: https://oauth.nooks.in/.well-known/oauth-authorization-server\n  status: 200\n- url: https://oauth.nooks.in/.well-known/jwks.json\n  status: 200\n- url: https://mcp.nooks.in/.well-known/oauth-protected-resource\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/authentication/nooks-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- Sales Engagement
- Sales Dialer
- AI SDR
- Outbound Sales
- Sales Coaching
- Revenue Operations
- Sales Sequencing
- CRM Integration
- Agents
- MCP
---
