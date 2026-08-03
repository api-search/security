---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Patlytics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Patlytics secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Patlytics
provider_slug: patlytics
scheme_count: 2
schemes:
- applies_to: https://mcp.patlytics.ai/mcp
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://mcp.patlytics.ai/authorize
    flow: authorizationCode
    refreshUrl: https://mcp.patlytics.ai/token
    scopes:
      patent:read: Read patent records, claims, portfolios and vault contents
      patent:search: Semantic patent and non-patent-literature search
    tokenUrl: https://mcp.patlytics.ai/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.patlytics.ai/
  name: PatlyticsOAuth
  registration_endpoint: https://mcp.patlytics.ai/register
  response_types_supported:
  - code
  revocation_endpoint: https://mcp.patlytics.ai/revoke
  revocation_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  sources:
  - well-known/patlytics-oauth-authorization-server.json
  - well-known/patlytics-oauth-protected-resource.json
  spec: OAuth 2.1 (RFC 6749 + RFC 7636 PKCE + RFC 7591 DCR + RFC 8414 + RFC 9728)
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
- applies_to: https://api.patlytics.ai
  description: The platform API host requires an Authorization header on every path, including the /.well-known/ surface. Unauthenticated requests return HTTP 401 with the JSON body {"detail":"Authorization header is missing"}. No public documentation, token-issuance endpoint or discovery document is published for this host.
  gated: true
  name: PatlyticsBearer
  scheme: bearer
  sources:
  - probe
  type: http
slug: patlytics-authentication
source_filename: patlytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://mcp.patlytics.ai/.well-known/oauth-authorization-server\ndocs: https://mcp.patlytics.ai/docs\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken]\n  bearer_methods: [header]\n  dynamic_client_registration: true\n  pkce_required_methods: [S256]\n  note: >-\n    Patlytics publishes no public REST OpenAPI, so this profile is searched from the live\n    RFC 8414 / RFC 9728 discovery documents on the MCP host plus the provider-published\n    connector page, not derived from a spec.\nschemes:\n- name: PatlyticsOAuth\n  type: oauth2\n  applies_to: https://mcp.patlytics.ai/mcp\n  spec: OAuth 2.1 (RFC 6749 + RFC 7636 PKCE + RFC 7591 DCR + RFC 8414 + RFC 9728)\n  issuer: https://mcp.patlytics.ai/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.patlytics.ai/authorize\n    tokenUrl: https://mcp.patlytics.ai/token\n    refreshUrl: https://mcp.patlytics.ai/token\n\
  \    scopes:\n      patent:search: Semantic patent and non-patent-literature search\n      patent:read: Read patent records, claims, portfolios and vault contents\n  registration_endpoint: https://mcp.patlytics.ai/register\n  revocation_endpoint: https://mcp.patlytics.ai/revoke\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  revocation_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  code_challenge_methods_supported: [S256]\n  sources:\n  - well-known/patlytics-oauth-authorization-server.json\n  - well-known/patlytics-oauth-protected-resource.json\n- name: PatlyticsBearer\n  type: http\n  scheme: bearer\n  applies_to: https://api.patlytics.ai\n  description: >-\n    The platform API host requires an Authorization header on every path, including the\n    /.well-known/ surface. Unauthenticated requests return HTTP 401 with the\
  \ JSON body\n    {\"detail\":\"Authorization header is missing\"}. No public documentation, token-issuance\n    endpoint or discovery document is published for this host.\n  gated: true\n  sources: [probe]\nidentity:\n  provider: >-\n    Patlytics' own identity provider (the connector page states sign-in is via \"Patlytics'\n    identity provider\"). The public status page lists an \"Auth0 User Authentication\"\n    component, indicating Auth0 backs end-user login for the customer dashboard.\n  per_user: true\n  org_scoped: true\n  note: >-\n    Each MCP client member signs in individually with their own Patlytics account and results\n    are scoped to their organization; there is no shared service-account or API-key model\n    published.\nx-evidence:\n  fetched: '2026-08-02'\n  probes:\n  - url: https://mcp.patlytics.ai/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n  - url: https://mcp.patlytics.ai/.well-known/oauth-protected-resource/mcp\n\
  \    http_status: 200\n    content_type: application/json\n  - url: https://api.patlytics.ai/\n    http_status: 401\n    content_type: application/json\n  - url: https://status.patlytics.ai/\n    http_status: 200\n    note: component list includes \"Auth0 User Authentication\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patlytics/refs/heads/main/authentication/patlytics-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Intellectual Property
- Patents
- Legal Tech
- Artificial Intelligence
- Patent Search
- Prior Art
- Model Context Protocol
- Agents
- Research
---
