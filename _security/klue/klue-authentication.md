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
method: searched
name: Klue Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Klue secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Klue
provider_slug: klue
scheme_count: 3
schemes:
- applies_to:
  - Klue Content API
  - Klue MCP Server
  description: A Klue API key passed as a Bearer token. Klue's own ChatGPT setup guide instructs users to select "API Key" with "Bearer" as the auth type and paste the Klue API key.
  in: header
  name: klue-content-api-key
  parameter_name: Authorization
  scheme_hint: bearer
  sources:
  - https://klue.com/blog/how-to-connect-klue-to-chatgpt
  type: apiKey
- applies_to:
  - Klue MCP Server
  - Klue integrations (Slack, Teams, CRM, SCIM)
  description: Klue runs an OAuth 2.0 authorization server on its application host, disclosed through an anonymous OpenID Connect Discovery document. Authorization code grant with refresh tokens and PKCE (S256), client_secret_basic or client_secret_post client authentication, and RFC 7591 dynamic client registration. Klue publishes no prose documentation for this surface — it is only visible through the discovery document.
  detail: scopes/klue-scopes.yml
  dynamic_client_registration:
    endpoint: https://app.klue.com/oauth/register
    probe: An anonymous POST with a deliberately invalid redirect_uri returned HTTP 400 invalid_redirect_uri, confirming the endpoint is live and validating input rather than 404ing. No client was registered.
    standard: RFC 7591
    supported: true
  flows:
  - authorizationUrl: https://app.klue.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.klue.com/oauth/token
    scopes_count: 23
    tokenUrl: https://app.klue.com/oauth/token
  method: probed
  name: klue-oauth2
  pkce:
    methods:
    - S256
    - plain
    supported: true
  sources:
  - https://app.klue.com/.well-known/openid-configuration
  - well-known/klue-openid-configuration.json
  token_management:
    introspection_endpoint: https://app.klue.com/oauth/introspect
    revocation_endpoint: https://app.klue.com/oauth/revoke
  type: oauth2
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  description: OpenID Connect provider on the same issuer. RS256 ID token signing, pairwise subject identifiers, userinfo endpoint, JWKS at /oauth/discovery/keys (verified live, returns an RSA key set).
  id_token_signing_alg_values_supported:
  - RS256
  method: probed
  name: klue-openid-connect
  openIdConnectUrl: https://app.klue.com/.well-known/openid-configuration
  sources:
  - https://app.klue.com/.well-known/openid-configuration
  subject_types_supported:
  - pairwise
  type: openIdConnect
slug: klue-authentication
source_filename: klue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://klue.com/blog/how-to-connect-klue-to-chatgpt\ndocs: https://help.app.klue.com/\ndocs_note: >-\n  help.app.klue.com is customer-only — every path below the root 302s to\n  /account/signin — so the Content API reference itself is not publicly readable.\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  oauth2_discovery: https://app.klue.com/.well-known/openid-configuration\n  scopes_published: 23\n  note: >-\n    Klue publishes no OpenAPI document publicly; the Content API OpenAPI schema is\n    distributed inside the authenticated application under\n    Apps & Integrations > Content API > \"How to use\". The apiKey profile is\n    therefore searched from Klue's public documentation rather than derived from a\n    spec. The oauth2/openIdConnect profile, added 2026-08-14, is PROBED: Klue's\n    application host serves a real OpenID Connect Discovery / RFC\
  \ 8414 document\n    anonymously at HTTP 200, which is the first machine-readable contract found on\n    Klue's public surface.\nschemes:\n- name: klue-content-api-key\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  scheme_hint: bearer\n  description: >-\n    A Klue API key passed as a Bearer token. Klue's own ChatGPT setup guide\n    instructs users to select \"API Key\" with \"Bearer\" as the auth type and paste\n    the Klue API key.\n  applies_to:\n  - Klue Content API\n  - Klue MCP Server\n  sources:\n  - https://klue.com/blog/how-to-connect-klue-to-chatgpt\n- name: klue-oauth2\n  type: oauth2\n  method: probed\n  description: >-\n    Klue runs an OAuth 2.0 authorization server on its application host, disclosed\n    through an anonymous OpenID Connect Discovery document. Authorization code\n    grant with refresh tokens and PKCE (S256), client_secret_basic or\n    client_secret_post client authentication, and RFC 7591 dynamic client\n    registration. Klue publishes\
  \ no prose documentation for this surface — it is\n    only visible through the discovery document.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.klue.com/oauth/authorize\n    tokenUrl: https://app.klue.com/oauth/token\n    refreshUrl: https://app.klue.com/oauth/token\n    scopes_count: 23\n  pkce:\n    supported: true\n    methods: [S256, plain]\n  dynamic_client_registration:\n    supported: true\n    standard: RFC 7591\n    endpoint: https://app.klue.com/oauth/register\n    probe: >-\n      An anonymous POST with a deliberately invalid redirect_uri returned HTTP 400\n      invalid_redirect_uri, confirming the endpoint is live and validating input\n      rather than 404ing. No client was registered.\n  token_management:\n    revocation_endpoint: https://app.klue.com/oauth/revoke\n    introspection_endpoint: https://app.klue.com/oauth/introspect\n  detail: scopes/klue-scopes.yml\n  applies_to:\n  - Klue MCP Server\n  - Klue integrations (Slack, Teams, CRM,\
  \ SCIM)\n  sources:\n  - https://app.klue.com/.well-known/openid-configuration\n  - well-known/klue-openid-configuration.json\n- name: klue-openid-connect\n  type: openIdConnect\n  method: probed\n  openIdConnectUrl: https://app.klue.com/.well-known/openid-configuration\n  description: >-\n    OpenID Connect provider on the same issuer. RS256 ID token signing, pairwise\n    subject identifiers, userinfo endpoint, JWKS at /oauth/discovery/keys\n    (verified live, returns an RSA key set).\n  claims_supported: [iss, sub, aud, exp, iat]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [pairwise]\n  sources:\n  - https://app.klue.com/.well-known/openid-configuration\nkey_management:\n  console_path: Apps & Integrations > Content API > Manage API Keys\n  requires_role: Admin\n  create: Create New API Key\n  named_keys: true\n  expiration:\n    supported: true\n    user_selected: true\n    vendor_recommendation: 1 year for production use\n  rotation_note: >-\n  \
  \  Keys are named and carry a user-selected expiry, so rotation is\n    self-service. Klue's guidance is to treat the key like a password.\nsso:\n  supported: true\n  protocols: [SAML 2.0]\n  identity_providers:\n  - name: Okta\n    url: https://www.okta.com/integrations/klue/\n  - name: Microsoft Entra ID\n    url: https://learn.microsoft.com/en-us/entra/identity/saas-apps/klue-tutorial\n  source: https://klue.com/product/security\naccess_control:\n  role_based_access: true\n  customized_user_permissions: true\n  source: https://klue.com/product/security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klue/refs/heads/main/authentication/klue-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Company
- SaaS
- Competitive Intelligence
- Competitive Enablement
- Sales Enablement
- Win-Loss Analysis
- Market Intelligence
- Battlecards
- Agents
- MCP
---
