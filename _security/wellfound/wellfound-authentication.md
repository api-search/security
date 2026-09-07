---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Wellfound Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wellfound declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Wellfound
provider_slug: wellfound
scheme_count: 2
schemes:
- authorization_response_iss_parameter_supported: true
  code_challenge_methods_supported:
  - S256
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://wellfound.com/api/oauth/authorize
      refreshUrl: https://wellfound.com/api/oauth/token
      scopes:
        accreditation: legacy AngelList-era scope; no current public reference documents it
        applications:accept: accept an inbound application
        applications:read: read a recruiter's inbound job applications
        applications:reject: reject an inbound application
        comment: legacy AngelList-era scope; no current public reference documents it
        dealflow: legacy AngelList-era scope; no current public reference documents it
        email: read the authenticated member's email address
        invest: legacy AngelList-era scope; no current public reference documents it
        message: legacy AngelList-era scope; no current public reference documents it
      tokenUrl: https://wellfound.com/api/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: wellfound-oauth2
  issuer: https://wellfound.com
  openid_connect_discovery: https://wellfound.com/.well-known/openid-configuration
  pkce_required_for_public_clients: true
  protects:
  - https://wellfound.com/api/mcp
  registration_endpoint: https://wellfound.com/api/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://wellfound.com/api/oauth/revoke
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  type: oauth2
  x-note: The scopes list is a single flat vocabulary mixing the six legacy AngelList social / investing scopes with the three new recruiter-application scopes. api.angel.co and every /api/1/* path now return 404, so the six legacy scopes appear to outlive the REST API they were minted for. Only the three applications:* scopes appear in the protected-resource document for the live MCP server.
- code_challenge_methods_supported:
  - S256
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://reach.wellfound.com/oauth/authorize
      refreshUrl: https://reach.wellfound.com/oauth/token
      scopes:
        agents:read: read AI sourcing agents
        agents:write: create or modify AI sourcing agents
        candidates:read: read candidates
        candidates:write: create or modify candidates
        company_lists:read: read company lists
        company_lists:write: create or modify company lists
        projects:read: read sourcing projects
      tokenUrl: https://reach.wellfound.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: wellfound-reach-oauth2
  issuer: https://reach.wellfound.com
  pkce_required_for_public_clients: true
  protects:
  - https://reach.wellfound.com/mcp
  registration_endpoint: https://reach.wellfound.com/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://reach.wellfound.com/oauth/revoke
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
  x-note: token_endpoint_auth_methods_supported is ["none"] only - this server accepts PUBLIC clients exclusively and has no confidential-client path. A server-side integration cannot authenticate with a client secret here.
slug: wellfound-authentication
source_filename: wellfound-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://wellfound.com/.well-known/openid-configuration (200),\n  https://wellfound.com/.well-known/oauth-authorization-server (200),\n  https://wellfound.com/.well-known/oauth-protected-resource (200),\n  https://reach.wellfound.com/.well-known/oauth-authorization-server (200),\n  https://reach.wellfound.com/.well-known/oauth-protected-resource (200)\nnote: >-\n  Derived from nothing - every field below was read out of a discovery document Wellfound\n  actually serves. Wellfound publishes no API reference, no authentication guide and no\n  developer portal, so these five machine-readable documents are the ONLY published\n  description of how to authenticate against Wellfound, and they are complete enough to\n  drive a client without them.\n\nsummary: >-\n  Two independent OAuth 2.1-shaped authorization servers, one per product. Both are\n  authorization-code + PKCE (S256) only, both support refresh tokens, both expose RFC\
  \ 7591\n  dynamic client registration, and both protect an MCP resource advertised via RFC 9728. No\n  API-key, basic-auth, mTLS or client-credentials path was found on either.\n\nschemes:\n- id: wellfound-oauth2\n  type: oauth2\n  issuer: https://wellfound.com\n  flows:\n    authorizationCode:\n      authorizationUrl: https://wellfound.com/api/oauth/authorize\n      tokenUrl: https://wellfound.com/api/oauth/token\n      refreshUrl: https://wellfound.com/api/oauth/token\n      scopes:\n        message: legacy AngelList-era scope; no current public reference documents it\n        dealflow: legacy AngelList-era scope; no current public reference documents it\n        comment: legacy AngelList-era scope; no current public reference documents it\n        email: read the authenticated member's email address\n        invest: legacy AngelList-era scope; no current public reference documents it\n        accreditation: legacy AngelList-era scope; no current public reference documents it\n     \
  \   applications:read: read a recruiter's inbound job applications\n        applications:accept: accept an inbound application\n        applications:reject: reject an inbound application\n  revocation_endpoint: https://wellfound.com/api/oauth/revoke\n  registration_endpoint: https://wellfound.com/api/oauth/register\n  dynamic_client_registration: true\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_post\n  code_challenge_methods_supported:\n  - S256\n  pkce_required_for_public_clients: true\n  authorization_response_iss_parameter_supported: true\n  openid_connect_discovery: https://wellfound.com/.well-known/openid-configuration\n  protects:\n  - https://wellfound.com/api/mcp\n  x-note: >-\n    The scopes list is a single flat vocabulary mixing the six legacy AngelList social /\n    investing scopes with the three new recruiter-application scopes. api.angel.co\
  \ and every\n    /api/1/* path now return 404, so the six legacy scopes appear to outlive the REST API\n    they were minted for. Only the three applications:* scopes appear in the\n    protected-resource document for the live MCP server.\n- id: wellfound-reach-oauth2\n  type: oauth2\n  issuer: https://reach.wellfound.com\n  flows:\n    authorizationCode:\n      authorizationUrl: https://reach.wellfound.com/oauth/authorize\n      tokenUrl: https://reach.wellfound.com/oauth/token\n      refreshUrl: https://reach.wellfound.com/oauth/token\n      scopes:\n        projects:read: read sourcing projects\n        agents:read: read AI sourcing agents\n        agents:write: create or modify AI sourcing agents\n        candidates:read: read candidates\n        candidates:write: create or modify candidates\n        company_lists:read: read company lists\n        company_lists:write: create or modify company lists\n  revocation_endpoint: https://reach.wellfound.com/oauth/revoke\n  registration_endpoint:\
  \ https://reach.wellfound.com/oauth/register\n  dynamic_client_registration: true\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  code_challenge_methods_supported:\n  - S256\n  pkce_required_for_public_clients: true\n  protects:\n  - https://reach.wellfound.com/mcp\n  x-note: >-\n    token_endpoint_auth_methods_supported is [\"none\"] only - this server accepts PUBLIC\n    clients exclusively and has no confidential-client path. A server-side integration\n    cannot authenticate with a client secret here.\n\ntoken_presentation:\n  method: bearer\n  location: Authorization header\n  source: bearer_methods_supported [\"header\"] in both protected-resource documents\n  challenge_on_missing_token:\n    wellfound.com/api/mcp: >-\n      401 Bearer resource_metadata=\"https://wellfound.com/.well-known/oauth-protected-resource/api/mcp\",\n      error=\"invalid_token\"\n    reach.wellfound.com/mcp:\
  \ >-\n      401 Bearer error=\"invalid_token\",\n      resource_metadata=\"https://reach.wellfound.com/.well-known/oauth-protected-resource\"\n\nnot_found:\n- api_key: no API-key scheme documented or advertised on any probed surface\n- basic_auth: none found\n- mtls: no mtls_endpoint_aliases in either authorization-server document\n- client_credentials: absent from grant_types_supported on both servers - there is no\n    machine-to-machine path without a human authorization step\n- jwks_uri: neither authorization server publishes a jwks_uri, and neither exposes a\n    userinfo_endpoint, so the wellfound.com document is OIDC-discovery-shaped but not a\n    complete OpenID Provider\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellfound/refs/heads/main/authentication/wellfound-authentication.yml
summary_line: 2 schemes
tags:
- Recruiting
- Hiring
- Talent
- Human Resources
- Applicant Tracking
- Job Board
- Startups
- MCP
- agent-native
- OAuth
- AI Sourcing
---
