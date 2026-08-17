---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Voiceops Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: VoiceOps secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: VoiceOps
provider_slug: voiceops
scheme_count: 3
schemes:
- applies_to: https://mcp.voiceops.com/mcp
  description: The remote MCP server requires an Authorization header carrying a VoiceOps API key. Omitting it returns JSON-RPC error -32000 "Missing Authorization header"; a syntactically valid but unknown bearer token returns -32000 "Invalid or unknown API key". The key format, issuance flow and rotation policy are not published.
  in: header
  name: mcpApiKey
  parameter_name: Authorization
  sources:
  - probe
  type: apiKey
- applies_to: https://app.voiceops.com
  description: End-user sign-in for the VoiceOps application is an OpenID Connect provider hosted on the VoiceOps subdomain clerk.voiceops.com (CNAME to frontend-api.clerk.services). This is the application login, not an API authorization surface for third-party developers.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://clerk.voiceops.com
  jwks_uri: https://clerk.voiceops.com/.well-known/jwks.json
  name: clerkOpenIdConnect
  openIdConnectUrl: https://clerk.voiceops.com/.well-known/openid-configuration
  sources:
  - well-known/voiceops-openid-configuration.json
  type: openIdConnect
- applies_to: https://app.voiceops.com
  description: RFC 8414 authorization-server metadata is served for the VoiceOps issuer. See scopes/voiceops-scopes.yml — the scope vocabulary is Clerk's standard scoped-access vocabulary, not a VoiceOps business-capability scope catalog.
  flows:
  - authorizationUrl: https://clerk.voiceops.com/oauth/authorize
    flow: authorizationCode
    introspectionUrl: https://clerk.voiceops.com/oauth/token_info
    pkce:
    - S256
    refresh_supported: true
    revocationUrl: https://clerk.voiceops.com/oauth/token/revoke
    scope_count: 6
    tokenUrl: https://clerk.voiceops.com/oauth/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
    - none
    userinfoUrl: https://clerk.voiceops.com/oauth/userinfo
  name: clerkOAuth2
  sources:
  - well-known/voiceops-oauth-authorization-server.json
  type: oauth2
slug: voiceops-authentication
source_filename: voiceops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  live probes of https://mcp.voiceops.com/mcp,\n  https://clerk.voiceops.com/.well-known/openid-configuration and\n  https://clerk.voiceops.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  VoiceOps publishes no authentication documentation. There is no developer\n  portal, no API reference, and no OpenAPI from which securitySchemes could be\n  derived, so this profile is assembled entirely from observed behaviour of the\n  live hosts.\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: mcpApiKey\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    applies_to: https://mcp.voiceops.com/mcp\n    sources: [probe]\n    description: >-\n      The remote MCP server requires an Authorization header carrying a VoiceOps\n      API key. Omitting it returns JSON-RPC error -32000 \"Missing Authorization\n    \
  \  header\"; a syntactically valid but unknown bearer token returns -32000\n      \"Invalid or unknown API key\". The key format, issuance flow and rotation\n      policy are not published.\n  - name: clerkOpenIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://clerk.voiceops.com/.well-known/openid-configuration\n    applies_to: https://app.voiceops.com\n    sources: [well-known/voiceops-openid-configuration.json]\n    description: >-\n      End-user sign-in for the VoiceOps application is an OpenID Connect\n      provider hosted on the VoiceOps subdomain clerk.voiceops.com (CNAME to\n      frontend-api.clerk.services). This is the application login, not an API\n      authorization surface for third-party developers.\n    issuer: https://clerk.voiceops.com\n    id_token_signing_alg_values_supported: [RS256]\n    jwks_uri: https://clerk.voiceops.com/.well-known/jwks.json\n  - name: clerkOAuth2\n    type: oauth2\n    applies_to: https://app.voiceops.com\n    sources: [well-known/voiceops-oauth-authorization-server.json]\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://clerk.voiceops.com/oauth/authorize\n        tokenUrl: https://clerk.voiceops.com/oauth/token\n        revocationUrl: https://clerk.voiceops.com/oauth/token/revoke\n        introspectionUrl: https://clerk.voiceops.com/oauth/token_info\n        userinfoUrl: https://clerk.voiceops.com/oauth/userinfo\n        refresh_supported: true\n        pkce: [S256]\n        token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n        scope_count: 6\n    description: >-\n      RFC 8414 authorization-server metadata is served for the VoiceOps issuer.\n      See scopes/voiceops-scopes.yml — the scope vocabulary is Clerk's standard\n      scoped-access vocabulary, not a VoiceOps business-capability scope\n      catalog.\ngaps:\n  - No documented way for a developer to obtain an API key.\n  - No published token lifetime, rotation, or revocation guidance for the MCP API key.\n  - The MCP server does not\
  \ advertise /.well-known/oauth-protected-resource, so an\n    MCP client cannot discover its authorization server automatically.\n  - api.voiceops.com returns HTTP 404 with a JSON envelope on every anonymous path\n    probed, and never issues a 401 challenge, so its authentication model could not\n    be observed at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voiceops/refs/heads/main/authentication/voiceops-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Ai Apps
- Conversation Intelligence
- Call Centers
- Sales Coaching
- Customer Experience
- Artificial Intelligence
- Speech Analytics
- Model Context Protocol
- Agents
---
