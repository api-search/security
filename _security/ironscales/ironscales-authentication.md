---
api_key_in:
- header
api_specs:
- filename: ironscales-authorization-api-openapi.yml
  format: yaml
  label: IRONSCALES Authorization API
  slug: ironscales-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-authorization-api-openapi.yml
- filename: ironscales-campaigns-api-openapi.yml
  format: yaml
  label: IRONSCALES Campaigns API
  slug: ironscales-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-campaigns-api-openapi.yml
- filename: ironscales-deepfake-api-openapi.yml
  format: yaml
  label: IRONSCALES Deepfake API
  slug: ironscales-deepfake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-deepfake-api-openapi.yml
- filename: ironscales-emails-api-openapi.yml
  format: yaml
  label: IRONSCALES Emails API
  slug: ironscales-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-emails-api-openapi.yml
- filename: ironscales-incident-api-openapi.yml
  format: yaml
  label: IRONSCALES Incident API
  slug: ironscales-incident-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-incident-api-openapi.yml
- filename: ironscales-mailboxes-api-openapi.yml
  format: yaml
  label: IRONSCALES Mailboxes API
  slug: ironscales-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-mailboxes-api-openapi.yml
- filename: ironscales-mitigation-api-openapi.yml
  format: yaml
  label: IRONSCALES Mitigation API
  slug: ironscales-mitigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-mitigation-api-openapi.yml
- filename: ironscales-sat-api-openapi.yml
  format: yaml
  label: IRONSCALES SAT API
  slug: ironscales-sat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-sat-api-openapi.yml
- filename: ironscales-settings-api-openapi.yml
  format: yaml
  label: IRONSCALES Settings API
  slug: ironscales-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/openapi/ironscales-settings-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ironscales Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: IRONSCALES secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: IRONSCALES
provider_slug: ironscales
scheme_count: 2
schemes:
- applies_to: IRONSCALES Management API
  declared_as: apikey
  in: header
  name: JWT
  note: 'The provider spec declares this scheme with `"type": "apikey"` (lowercase k), which is not a valid Swagger 2.0 securityDefinitions type — the specification requires `apiKey`. Tooling that validates strictly will reject the securityDefinitions block. Captured here and in overlays/ironscales-management-api-overlay.yaml rather than mutating the harvested original.'
  parameter: Authorization
  sources:
  - openapi/_original/ironscales-management-api-openapi.json
  - openapi/ironscales-authorization-openapi.yml
  - openapi/ironscales-campaigns-openapi.yml
  - openapi/ironscales-deepfake-openapi.yml
  - openapi/ironscales-emails-openapi.yml
  - openapi/ironscales-incident-openapi.yml
  - openapi/ironscales-mailboxes-openapi.yml
  - openapi/ironscales-mitigation-openapi.yml
  - openapi/ironscales-sat-openapi.yml
  - openapi/ironscales-settings-openapi.yml
  type: apiKey
- applies_to: IRONSCALES MCP Server (https://mcp.ironscales.com/mcp/)
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://members.ironscales.com/o/authorize/
    flow: authorizationCode
    pkce: S256
    refresh_token: true
    tokenUrl: https://members.ironscales.com/o/token/
  introspection_endpoint: https://members.ironscales.com/o/introspect/
  issuer: https://members.ironscales.com
  name: OAuth2
  registration_endpoint: https://members.ironscales.com/o/register/
  revocation_endpoint: https://members.ironscales.com/o/revoke_token/
  scopes_note: The RFC 8414 authorization-server metadata document does not advertise `scopes_supported`, and no scope reference is published in the public docs, so no scopes/ artifact is emitted rather than guess a scope vocabulary.
  scopes_published: false
  sources:
  - well-known/ironscales-oauth-authorization-server.json
  - well-known/ironscales-oauth-protected-resource.json
  token_endpoint_auth_methods:
  - client_secret_post
  type: oauth2
slug: ironscales-authentication
source_filename: ironscales-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://appapi.ironscales.com/appapi/docs/?format=openapi\ndocs: https://ironscales.com/platform/api\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  surfaces:\n  - IRONSCALES Management API (REST) — JWT bearer token in the Authorization header\n  - IRONSCALES MCP Server — OAuth 2.0 authorization code + PKCE\nschemes:\n- name: JWT\n  type: apiKey\n  in: header\n  parameter: Authorization\n  applies_to: IRONSCALES Management API\n  declared_as: apikey\n  note: >-\n    The provider spec declares this scheme with `\"type\": \"apikey\"` (lowercase k), which is not a valid\n    Swagger 2.0 securityDefinitions type — the specification requires `apiKey`. Tooling that validates\n    strictly will reject the securityDefinitions block. Captured here and in\n    overlays/ironscales-management-api-overlay.yaml rather than mutating the harvested original.\n  sources:\n  -\
  \ openapi/_original/ironscales-management-api-openapi.json\n  - openapi/ironscales-authorization-openapi.yml\n  - openapi/ironscales-campaigns-openapi.yml\n  - openapi/ironscales-deepfake-openapi.yml\n  - openapi/ironscales-emails-openapi.yml\n  - openapi/ironscales-incident-openapi.yml\n  - openapi/ironscales-mailboxes-openapi.yml\n  - openapi/ironscales-mitigation-openapi.yml\n  - openapi/ironscales-sat-openapi.yml\n  - openapi/ironscales-settings-openapi.yml\n- name: OAuth2\n  type: oauth2\n  applies_to: IRONSCALES MCP Server (https://mcp.ironscales.com/mcp/)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://members.ironscales.com/o/authorize/\n    tokenUrl: https://members.ironscales.com/o/token/\n    pkce: S256\n    refresh_token: true\n  issuer: https://members.ironscales.com\n  registration_endpoint: https://members.ironscales.com/o/register/\n  revocation_endpoint: https://members.ironscales.com/o/revoke_token/\n  introspection_endpoint: https://members.ironscales.com/o/introspect/\n\
  \  token_endpoint_auth_methods:\n  - client_secret_post\n  dynamic_client_registration: true\n  scopes_published: false\n  scopes_note: >-\n    The RFC 8414 authorization-server metadata document does not advertise `scopes_supported`, and no\n    scope reference is published in the public docs, so no scopes/ artifact is emitted rather than\n    guess a scope vocabulary.\n  sources:\n  - well-known/ironscales-oauth-authorization-server.json\n  - well-known/ironscales-oauth-protected-resource.json\ncredential_flow:\n  rest:\n    step_1: >-\n      An IRONSCALES dashboard user with an ADMIN or OWNER role generates an APP API Token under\n      Settings > Account Settings > General & Security, alongside the tenant Company ID.\n    step_2: >-\n      POST /appapi/get-token/ (operationId \"get JWT token\") exchanges the APP API token for a JWT.\n    step_3: >-\n      The JWT is presented on every subsequent call in the Authorization request header. Nearly every\n      operation is additionally\
  \ scoped by a company_id path parameter, so the token and the tenant id\n      are both required.\n    token_lifetime: not published\n  mcp:\n    step_1: >-\n      The MCP client discovers https://mcp.ironscales.com/.well-known/oauth-protected-resource from the\n      401 WWW-Authenticate challenge, which names https://members.ironscales.com/ as the authorization server.\n    step_2: >-\n      The client may self-register at the RFC 7591 registration endpoint, then runs an authorization\n      code + PKCE (S256) flow against members.ironscales.com.\n    step_3: >-\n      The resulting bearer token is sent in the Authorization header to https://mcp.ironscales.com/mcp/.\nx-evidence:\n  fetched: '2026-08-04'\n  openapi_url: https://appapi.ironscales.com/appapi/docs/?format=openapi\n  openapi_http_status: 200\n  oauth_metadata_http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironscales/refs/heads/main/authentication/ironscales-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Email Security
- Cybersecurity
- Phishing
- Anti-Phishing
- Business Email Compromise
- Account Takeover
- Threat Intelligence
- Incident Response
- Security Awareness Training
- Phishing Simulation
- Microsoft-365
- Google Workspace
- SOC Automation
- Deepfake Detection
- MCP
---
