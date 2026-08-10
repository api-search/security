---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Everstream Analytics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Everstream Analytics secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Everstream Analytics
provider_slug: everstream-analytics
scheme_count: 3
schemes:
- applies_to: Everstream customer application (app.us1.apps.everstream.ai, us1/eu1.apps.everstream.ai)
  audience: https://maglev-prod/api
  authorization_endpoint: https://riskpulse-prod.us.auth0.com/authorize
  device_authorization_endpoint: https://riskpulse-prod.us.auth0.com/oauth/device/code
  evidence: GET https://app.us1.apps.everstream.ai/ returns HTTP 302 to https://riskpulse-prod.us.auth0.com/authorize?audience=https%3A%2F%2Fmaglev-prod%2Fapi&scope=openid+profile+email+offline_access&response_type=code&code_challenge_method=S256 (probed 2026-08-04).
  flow: authorizationCode
  issuer: https://riskpulse-prod.us.auth0.com/
  jwks_uri: https://riskpulse-prod.us.auth0.com/.well-known/jwks.json
  mfa: true
  mfa_endpoint: https://riskpulse-prod.us.auth0.com/mfa/challenge
  name: everstream-platform-oidc
  openIdConnectUrl: https://riskpulse-prod.us.auth0.com/.well-known/openid-configuration
  pkce: S256
  provider: Auth0
  revocation_endpoint: https://riskpulse-prod.us.auth0.com/oauth/revoke
  scopes_observed:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - well-known/everstream-analytics-auth0-openid-configuration.json
  token_endpoint: https://riskpulse-prod.us.auth0.com/oauth/token
  type: openIdConnect
  userinfo_endpoint: https://riskpulse-prod.us.auth0.com/userinfo
- applies_to: us1.apps.everstream.ai (legacy application login)
  evidence: GET https://us1.apps.everstream.ai/ returns HTTP 200 at /auth/?next=%2F with an HTML login form titled "Login | Everstream" (probed 2026-08-04).
  linked_from: https://www.everstream.ai/login-page/
  login_url: https://us1.apps.everstream.ai/auth/
  name: everstream-legacy-app-login
  scheme: form-login
  type: http
- applies_to: m365-mcp.everstream.ai (Microsoft 365 MCP relay — internal productivity tooling, NOT the Everstream platform API)
  authorization_endpoint: https://m365-mcp.everstream.ai/authorize
  dynamic_client_registration: false
  evidence: POST https://m365-mcp.everstream.ai/mcp with a tools/list JSON-RPC body returns HTTP 401 {"error":"invalid_token","error_description":"Missing or malformed Authorization header"} (probed 2026-08-04).
  flow: authorizationCode
  issuer: https://m365-mcp.everstream.ai
  name: m365-mcp-oauth2
  pkce: S256
  protected_resource: https://m365-mcp.everstream.ai/mcp
  scopes_note: scopes_supported are Microsoft Graph scopes, not Everstream data scopes
  sources:
  - well-known/everstream-analytics-m365-mcp-oauth-authorization-server.json
  - well-known/everstream-analytics-m365-mcp-oauth-protected-resource.json
  token_endpoint: https://m365-mcp.everstream.ai/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: everstream-analytics-authentication
source_filename: everstream-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live probes of app.us1.apps.everstream.ai, us1.apps.everstream.ai and the\n  Auth0 tenant riskpulse-prod.us.auth0.com\ndocs: null\nnotes: 'Everstream Analytics publishes no OpenAPI, so no securityScheme could be derived.\n  This profile is assembled entirely from observed, unauthenticated HTTP behaviour of\n  the production application estate plus the identity provider''s own public discovery\n  document. The platform API''s own authentication scheme (the credential a customer\n  presents to the Reveal/Explore API) is documented only behind customer login and is\n  NOT recorded here — recording it would be a guess.'\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  spec_derived: false\nschemes:\n- name: everstream-platform-oidc\n  type: openIdConnect\n  applies_to: Everstream customer application (app.us1.apps.everstream.ai, us1/eu1.apps.everstream.ai)\n  provider:\
  \ Auth0\n  openIdConnectUrl: https://riskpulse-prod.us.auth0.com/.well-known/openid-configuration\n  issuer: https://riskpulse-prod.us.auth0.com/\n  authorization_endpoint: https://riskpulse-prod.us.auth0.com/authorize\n  token_endpoint: https://riskpulse-prod.us.auth0.com/oauth/token\n  jwks_uri: https://riskpulse-prod.us.auth0.com/.well-known/jwks.json\n  userinfo_endpoint: https://riskpulse-prod.us.auth0.com/userinfo\n  revocation_endpoint: https://riskpulse-prod.us.auth0.com/oauth/revoke\n  device_authorization_endpoint: https://riskpulse-prod.us.auth0.com/oauth/device/code\n  flow: authorizationCode\n  pkce: S256\n  audience: https://maglev-prod/api\n  scopes_observed:\n  - openid\n  - profile\n  - email\n  - offline_access\n  mfa: true\n  mfa_endpoint: https://riskpulse-prod.us.auth0.com/mfa/challenge\n  sources:\n  - well-known/everstream-analytics-auth0-openid-configuration.json\n  evidence: 'GET https://app.us1.apps.everstream.ai/ returns HTTP 302 to\n    https://riskpulse-prod.us.auth0.com/authorize?audience=https%3A%2F%2Fmaglev-prod%2Fapi&scope=openid+profile+email+offline_access&response_type=code&code_challenge_method=S256\n\
  \    (probed 2026-08-04).'\n- name: everstream-legacy-app-login\n  type: http\n  scheme: form-login\n  applies_to: us1.apps.everstream.ai (legacy application login)\n  login_url: https://us1.apps.everstream.ai/auth/\n  linked_from: https://www.everstream.ai/login-page/\n  evidence: 'GET https://us1.apps.everstream.ai/ returns HTTP 200 at /auth/?next=%2F\n    with an HTML login form titled \"Login | Everstream\" (probed 2026-08-04).'\n- name: m365-mcp-oauth2\n  type: oauth2\n  applies_to: m365-mcp.everstream.ai (Microsoft 365 MCP relay — internal productivity\n    tooling, NOT the Everstream platform API)\n  issuer: https://m365-mcp.everstream.ai\n  authorization_endpoint: https://m365-mcp.everstream.ai/authorize\n  token_endpoint: https://m365-mcp.everstream.ai/token\n  flow: authorizationCode\n  pkce: S256\n  dynamic_client_registration: false\n  token_endpoint_auth_methods_supported:\n  - none\n  protected_resource: https://m365-mcp.everstream.ai/mcp\n  scopes_note: scopes_supported\
  \ are Microsoft Graph scopes, not Everstream data scopes\n  sources:\n  - well-known/everstream-analytics-m365-mcp-oauth-authorization-server.json\n  - well-known/everstream-analytics-m365-mcp-oauth-protected-resource.json\n  evidence: 'POST https://m365-mcp.everstream.ai/mcp with a tools/list JSON-RPC body\n    returns HTTP 401 {\"error\":\"invalid_token\",\"error_description\":\"Missing or malformed\n    Authorization header\"} (probed 2026-08-04).'\ngaps:\n- No public authentication reference page for the platform API. The Insights-to-Action\n  page advertises API connectivity, webhooks and SFTP but names no credential type,\n  header, token endpoint or key-issuance flow.\n- No developer portal, no self-service credential issuance, no public API key management.\nx-evidence:\n  fetched: '2026-08-04'\n  hosts:\n  - https://app.us1.apps.everstream.ai\n  - https://us1.apps.everstream.ai\n  - https://m365-mcp.everstream.ai\n  - https://riskpulse-prod.us.auth0.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everstream-analytics/refs/heads/main/authentication/everstream-analytics-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Company
- Supply Chain
- Supply Chain Risk
- Risk Management
- Logistics
- Analytics
- Weather Intelligence
- Procurement
- Compliance
- Artificial Intelligence
---
