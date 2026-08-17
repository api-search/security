---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Bluefish Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bluefish AI secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bluefish AI
provider_slug: bluefish-ai
scheme_count: 2
schemes:
- client_id_metadata_document_supported: true
  dynamic_client_registration:
    registration_endpoint: https://auth.bluefishai.com/v1/oauth2/register
    spec: RFC 7591
    supported: true
  flows:
  - authorizationUrl: https://platform.bluefishai.com/connected-apps/authorize
    flow: authorizationCode
    refreshUrl: https://auth.bluefishai.com/v1/oauth2/token
    scopes_count: 7
    tokenUrl: https://auth.bluefishai.com/v1/oauth2/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  issuer: https://auth.bluefishai.com
  name: BluefishOAuth2
  pkce:
    plain_supported: false
    required_methods:
    - S256
  response_types:
  - code
  - code token
  sources:
  - well-known/bluefish-ai-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- end_session_endpoint: https://platform.bluefishai.com/connected-apps/authorize
  grant_types:
  - authorization_code
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://auth.bluefishai.com
  jwks_uri: https://auth.bluefishai.com/.well-known/jwks.json
  name: BluefishOIDC
  openIdConnectUrl: https://auth.bluefishai.com/.well-known/openid-configuration
  response_types:
  - code
  sources:
  - well-known/bluefish-ai-openid-configuration.json
  subject_types_supported:
  - public
  type: openIdConnect
  userinfo_endpoint: https://auth.bluefishai.com/v1/oauth2/userinfo
slug: bluefish-ai-authentication
source_filename: bluefish-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.bluefishai.com/.well-known/oauth-authorization-server\nnote: >-\n  Not derived from an OpenAPI — Bluefish publishes no spec. This profile is read\n  directly from the provider's own live OAuth 2.0 Authorization Server Metadata\n  (RFC 8414), OpenID Connect Discovery document, and the RFC 9728 protected-resource\n  metadata for the MCP endpoint. Every value below is copied from a 200 response\n  captured in well-known/. Bluefish does not document authentication anywhere on its\n  public site, so these machine-readable discovery documents are the only published\n  description of how to authenticate, and they are complete enough to implement\n  against.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  protected_resources: [https://platform.bluefishai.com/mcp]\n  public_self_service: false\n  public_self_service_note: >-\n    The authorization endpoint sits on the\
  \ authenticated customer platform at\n    /connected-apps/authorize (307s to login when anonymous), so obtaining a token\n    requires an existing Bluefish customer account. Dynamic client registration is\n    open, but consent is customer-gated.\nschemes:\n- name: BluefishOAuth2\n  type: oauth2\n  sources: [well-known/bluefish-ai-oauth-authorization-server.json]\n  issuer: https://auth.bluefishai.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.bluefishai.com/connected-apps/authorize\n    tokenUrl: https://auth.bluefishai.com/v1/oauth2/token\n    refreshUrl: https://auth.bluefishai.com/v1/oauth2/token\n    scopes_count: 7\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code, code token]\n  pkce:\n    required_methods: [S256]\n    plain_supported: false\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  dynamic_client_registration:\n    supported: true\n\
  \    registration_endpoint: https://auth.bluefishai.com/v1/oauth2/register\n    spec: RFC 7591\n  client_id_metadata_document_supported: true\n- name: BluefishOIDC\n  type: openIdConnect\n  sources: [well-known/bluefish-ai-openid-configuration.json]\n  openIdConnectUrl: https://auth.bluefishai.com/.well-known/openid-configuration\n  issuer: https://auth.bluefishai.com\n  userinfo_endpoint: https://auth.bluefishai.com/v1/oauth2/userinfo\n  end_session_endpoint: https://platform.bluefishai.com/connected-apps/authorize\n  jwks_uri: https://auth.bluefishai.com/.well-known/jwks.json\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  response_types: [code]\n  grant_types: [authorization_code]\ntoken_presentation:\n  style: bearer\n  header: Authorization\n  evidence: >-\n    POST https://platform.bluefishai.com/mcp without credentials returns 401 with\n    WWW-Authenticate: Bearer error=\"invalid_token\",\n    error_description=\"No authorization provided\"\
  .\ndivergences:\n- field: grant_types_supported\n  note: >-\n    The RFC 8414 document advertises three grants (authorization_code, refresh_token,\n    jwt-bearer) while the OIDC document advertises only authorization_code. The OIDC\n    document also lists a full_access scope the OAuth document omits, and the OAuth\n    document omits profile/email/phone. The two discovery documents are not in sync;\n    recorded as observed rather than merged silently.\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - {url: 'https://auth.bluefishai.com/.well-known/oauth-authorization-server', status: 200}\n  - {url: 'https://auth.bluefishai.com/.well-known/openid-configuration', status: 200}\n  - {url: 'https://auth.bluefishai.com/.well-known/jwks.json', status: 200}\n  - {url: 'https://platform.bluefishai.com/.well-known/oauth-protected-resource/mcp', status: 200}\n  - {url: 'https://platform.bluefishai.com/mcp', status: 401}\n  - {url: 'https://platform.bluefishai.com/connected-apps/authorize',\
  \ status: 307}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluefish-ai/refs/heads/main/authentication/bluefish-ai-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Marketing
- Artificial Intelligence
- Generative Engine Optimization
- Brand Safety
- Agentic Commerce
- Analytics
- MCP
- Agents
---
