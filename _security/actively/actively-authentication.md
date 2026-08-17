---
api_key_in: []
auth_types: []
description: 'Actively AI protects its hosted MCP server (https://api.actively.ai/mcp) with OAuth 2.1 authorization-code + PKCE against a first-party authorization server at https://auth.actively.ai, which also speaks full OpenID Connect. There is no API-key surface: the only published, machine-discoverable authentication path is OAuth. No public REST API is published, so no securityScheme block exists to derive from — the profile below is read from live discovery metadata.'
kind: authentication
layout: security
method: probed
name: Actively Authentication
name_suffix: Authentication
oauth_flows: []
overview: Actively declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Actively
provider_slug: actively
scheme_count: 3
schemes:
- applies_to: https://api.actively.ai/mcp
  authorization_endpoint: https://auth.actively.ai/oauth2/authorize
  bearer_methods_supported:
  - header
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id: oauth2_authorization_code
  introspection_endpoint: https://auth.actively.ai/oauth2/introspection
  jwks_uri: https://auth.actively.ai/oauth2/jwks
  note: 'The api-host mirror of the metadata narrows this for MCP clients specifically: grant_types [authorization_code, refresh_token], token_endpoint_auth_methods ["none"] — i.e. public clients with PKCE and no client secret.'
  pkce_required_methods:
  - S256
  registration_endpoint: https://auth.actively.ai/oauth2/register
  response_modes:
  - query
  response_types:
  - code
  token_endpoint: https://auth.actively.ai/oauth2/token
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
- applies_to: https://auth.actively.ai
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id: oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://auth.actively.ai
  note: client_credentials appears in the OIDC document but NOT in the MCP-facing authorization-server mirror, so machine-to-machine tokens are not advertised for the MCP resource.
  openid_configuration: https://auth.actively.ai/.well-known/openid-configuration
  subject_types_supported:
  - public
  type: openIdConnect
  userinfo_endpoint: https://auth.actively.ai/oauth2/userinfo
- device_authorization_endpoint: https://auth.actively.ai/oauth2/device_authorization
  flow: urn:ietf:params:oauth:grant-type:device_code
  id: device_code
  note: Device authorization grant is supported, which is the flow a headless agent or CLI would use. Not documented anywhere in prose.
  type: oauth2
slug: actively-authentication
source_filename: actively-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://api.actively.ai/.well-known/oauth-protected-resource +\n  https://auth.actively.ai/.well-known/openid-configuration +\n  https://auth.actively.ai/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  Actively publishes no developer documentation host and no written auth guide.\n  This profile is derived entirely from the machine-readable discovery\n  documents the provider serves anonymously, not from prose.\ndescription: >-\n  Actively AI protects its hosted MCP server (https://api.actively.ai/mcp) with\n  OAuth 2.1 authorization-code + PKCE against a first-party authorization\n  server at https://auth.actively.ai, which also speaks full OpenID Connect.\n  There is no API-key surface: the only published, machine-discoverable\n  authentication path is OAuth. No public REST API is published, so no\n  securityScheme block exists to derive from — the profile below is read from\n  live discovery metadata.\n\
  \nschemes:\n- id: oauth2_authorization_code\n  type: oauth2\n  applies_to: https://api.actively.ai/mcp\n  flow: authorization_code\n  pkce_required_methods:\n  - S256\n  authorization_endpoint: https://auth.actively.ai/oauth2/authorize\n  token_endpoint: https://auth.actively.ai/oauth2/token\n  jwks_uri: https://auth.actively.ai/oauth2/jwks\n  registration_endpoint: https://auth.actively.ai/oauth2/register\n  introspection_endpoint: https://auth.actively.ai/oauth2/introspection\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  response_types:\n  - code\n  response_modes:\n  - query\n  bearer_methods_supported:\n  - header\n  note: >-\n    The api-host mirror of the metadata narrows this for MCP clients\n    specifically: grant_types [authorization_code, refresh_token],\n    token_endpoint_auth_methods [\"none\"] — i.e. public clients with\
  \ PKCE and\n    no client secret.\n\n- id: oidc\n  type: openIdConnect\n  applies_to: https://auth.actively.ai\n  openid_configuration: https://auth.actively.ai/.well-known/openid-configuration\n  issuer: https://auth.actively.ai\n  userinfo_endpoint: https://auth.actively.ai/oauth2/userinfo\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  note: >-\n    client_credentials appears in the OIDC document but NOT in the\n    MCP-facing authorization-server mirror, so machine-to-machine tokens are\n    not advertised for the MCP resource.\n\n- id: device_code\n  type: oauth2\n  flow: urn:ietf:params:oauth:grant-type:device_code\n  device_authorization_endpoint: https://auth.actively.ai/oauth2/device_authorization\n  note: >-\n    Device authorization grant is supported, which is the flow a headless\n    agent or CLI\
  \ would use. Not documented anywhere in prose.\n\ndynamic_client_registration:\n  supported: true\n  endpoint: https://auth.actively.ai/oauth2/register\n  spec: RFC 7591\n  client_id_metadata_document_supported: true\n  note: >-\n    An MCP client can register itself with no prior contact with Actively.\n    This is what makes the endpoint reachable from a cold start.\n\ntoken:\n  placement: header\n  scheme: Bearer\n  challenge: >-\n    Bearer error=\"invalid_token\",\n    resource_metadata=\"https://api.actively.ai/.well-known/oauth-protected-resource/mcp\"\n  challenge_note: >-\n    The 401 carries a spec-compliant RFC 9728 WWW-Authenticate challenge that\n    points the client at its own discovery document — the behaviour an MCP\n    client needs to bootstrap.\n\nidentity_provider:\n  vendor: WorkOS AuthKit\n  evidence: >-\n    app.actively.ai 307-redirects unauthenticated requests to\n    https://api.workos.com/user_management/authorize?client_id=client_01K26EZTNS1CRN2ABZ0Z37Y2MW&provider=authkit,\n\
  \    and auth.actively.ai is the branded custom domain for the same tenant.\n  note: >-\n    Recorded as an infrastructure fact, not a criticism — the authorization\n    server is served from Actively's own domain and issues Actively's tokens.\n\nnot_published:\n- api_keys: No API-key or personal-access-token surface is documented anywhere.\n- mtls: No mutual-TLS scheme advertised.\n- basic_auth: Not offered on the API surface.\n- auth_documentation: >-\n    No human-readable authentication guide, quickstart, or developer portal\n    exists. Everything here had to be probed.\n\nevidence:\n- fetched: '2026-08-13'\n  url: https://api.actively.ai/.well-known/oauth-protected-resource\n  http_status: 200\n- fetched: '2026-08-13'\n  url: https://api.actively.ai/.well-known/oauth-authorization-server\n  http_status: 200\n- fetched: '2026-08-13'\n  url: https://auth.actively.ai/.well-known/openid-configuration\n  http_status: 200\n- fetched: '2026-08-13'\n  url: https://auth.actively.ai/.well-known/oauth-authorization-server\n\
  \  http_status: 200\n- fetched: '2026-08-13'\n  url: https://api.actively.ai/mcp\n  http_status: 401\n  note: WWW-Authenticate challenge observed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actively/refs/heads/main/authentication/actively-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Ai Apps
- AI Agents
- Revenue Intelligence
- Sales
- Go To Market
- MCP
- OAuth
- Model Context Protocol
- Sales Intelligence
- Enterprise Software
---
