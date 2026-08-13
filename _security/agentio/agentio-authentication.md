---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Agentio Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- refresh_token
overview: Agentio secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code and refresh_token flow(s).
provider_name: Agentio
provider_slug: agentio
scheme_count: 1
schemes:
- advertised:
    bearer_methods_supported:
    - header
    client_id_metadata_document_supported: true
    code_challenge_methods_supported:
    - S256
    grant_types_supported:
    - authorization_code
    - refresh_token
    response_types_supported:
    - code
    token_endpoint_auth_methods_supported:
    - none
  applies_to: https://mcp.agentio.com/mcp
  endpoints:
    authorization_endpoint: https://app.agentio.com/connector/consent
    registration_endpoint: https://api.agentio.com/o/register
    revocation_endpoint: https://api.agentio.com/o/revoke_token
    token_endpoint: https://api.agentio.com/o/token
  flows:
  - authorizationUrl: https://app.agentio.com/connector/consent
    flow: authorizationCode
    refreshUrl: https://api.agentio.com/o/token
    scopes:
      brand-connector:read: Read-only access to one brand's Agentio data via the MCP connector
    tokenUrl: https://api.agentio.com/o/token
  issuer: https://api.agentio.com/o
  name: AgentioBrandConnectorOAuth
  sources:
  - well-known/agentio-oauth-authorization-server.json
  - well-known/agentio-oauth-protected-resource.json
  type: oauth2
slug: agentio-authentication
source_filename: agentio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://api.agentio.com/.well-known/oauth-authorization-server/o\ndocs: https://www.agentio.com/connector\nnote: >-\n  Agentio publishes no OpenAPI, so this profile is not derived from securitySchemes. It is read\n  directly from the two discovery documents Agentio serves anonymously for its hosted MCP server\n  (RFC 9728 protected-resource metadata on mcp.agentio.com, RFC 8414 authorization-server\n  metadata on api.agentio.com) plus the connector documentation. Every value below is copied\n  verbatim from those documents.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorization_code\n  - refresh_token\n  bearer_methods:\n  - header\n  pkce: required (S256 is the only code_challenge_method advertised)\n  dynamic_client_registration: true\n  client_authentication: none (public clients; token_endpoint_auth_methods_supported = [\"none\"])\nschemes:\n- name: AgentioBrandConnectorOAuth\n  type: oauth2\n  applies_to:\
  \ https://mcp.agentio.com/mcp\n  sources:\n  - well-known/agentio-oauth-authorization-server.json\n  - well-known/agentio-oauth-protected-resource.json\n  issuer: https://api.agentio.com/o\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.agentio.com/connector/consent\n    tokenUrl: https://api.agentio.com/o/token\n    refreshUrl: https://api.agentio.com/o/token\n    scopes:\n      brand-connector:read: Read-only access to one brand's Agentio data via the MCP connector\n  endpoints:\n    authorization_endpoint: https://app.agentio.com/connector/consent\n    token_endpoint: https://api.agentio.com/o/token\n    registration_endpoint: https://api.agentio.com/o/register\n    revocation_endpoint: https://api.agentio.com/o/revoke_token\n  advertised:\n    response_types_supported:\n    - code\n    grant_types_supported:\n    - authorization_code\n    - refresh_token\n    code_challenge_methods_supported:\n    - S256\n    token_endpoint_auth_methods_supported:\n    - none\n\
  \    client_id_metadata_document_supported: true\n    bearer_methods_supported:\n    - header\nprotected_resources:\n- resource: https://mcp.agentio.com/mcp\n  authorization_servers:\n  - https://api.agentio.com/o\n  scopes_supported:\n  - brand-connector:read\nconsent:\n  step: >-\n    The user is sent to app.agentio.com/connector/consent in a browser, confirms the\n    connection, and picks which brand the connection is pinned to when they have more than one.\n  revocation: >-\n    Settings -> Integrations in the Agentio app lists every connected AI app; disconnecting\n    takes effect immediately and cuts that app's access. There is also an RFC 7009 revocation\n    endpoint at https://api.agentio.com/o/revoke_token.\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - url: https://api.agentio.com/.well-known/oauth-authorization-server/o\n    http_status: 200\n    content_type: application/json\n  - url: https://mcp.agentio.com/.well-known/oauth-protected-resource/mcp\n    http_status:\
  \ 200\n    content_type: application/json\n  - url: https://api.agentio.com/o/token\n    method: GET\n    http_status: 405\n    note: method-not-allowed confirms the token endpoint is live and POST-only\n  - url: https://api.agentio.com/o/register\n    method: GET\n    http_status: 405\n    note: 'returns {\"detail\": \"Method \\\"GET\\\" not allowed.\"} — the DCR endpoint is live'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentio/refs/heads/main/authentication/agentio-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Adtech
- Advertising
- Creator Economy
- Influencer Marketing
- Marketing
- Artificial Intelligence
- YouTube
- MCP
- Model Context Protocol
- Agents
- Analytics
---
