---
api_key_in:
- header
api_specs:
- filename: rhombus-systems-openapi.json
  format: json
  label: Rhombus Public REST API
  slug: rhombus-systems-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhombus-systems/refs/heads/main/openapi/rhombus-systems-openapi.json
- filename: rhombus-systems-console-websocket-asyncapi.json
  format: json
  label: Rhombus Console WebSocket API
  slug: rhombus-systems-console-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhombus-systems/refs/heads/main/asyncapi/rhombus-systems-console-websocket-asyncapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rhombus Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rhombus Systems secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rhombus Systems
provider_slug: rhombus-systems
scheme_count: 2
schemes:
- companion_header:
    name: x-auth-scheme
    required: true
    values:
    - api-token
    - partner-api-token
  description: Rhombus API key. Requires the x-auth-scheme companion header — a key alone is not a complete credential. api-token for standard auth, partner-api-token for partner/MSP auth.
  in: header
  name: ApiKeyAuth
  parameter: x-auth-apikey
  permission_model: A key INHERITS the permissions of the user who created it. There are no key-level scopes; least privilege is achieved by creating the key from a least-privileged user or role.
  provisioning: https://console.rhombus.com/settings/api-management
  recommended_for: agents, scripts, server-to-server integrations acting as one Rhombus account
  region_bound: true
  region_note: Keys are bound to their region — a US key will not work against api2.eu.rhombussystems.com.
  self_serve: true
  shown_once: true
  sources:
  - openapi/rhombus-systems-openapi.json
  - https://www.rhombus.com/auth.md
  type: apiKey
- access_token_lifetime_sec: 3600
  client_provisioning:
    authenticated_with: an API key
    operationId: submitApplication
    path: /api/oauth/submitApplication
    related_operations:
    - getAllApplicationsForOrg
    - getApplicationByClientId
    - updateApplication
    - deleteApplication
    returns:
    - clientId
    - clientSecret
    review_required: Production apps distributed to other organizations require Rhombus review, started in the developer community.
    secret_shown_once: true
  declared_in_openapi: false
  description: '"Sign in with Rhombus" — OAuth 2.0 authorization code with PKCE, for third-party apps where Rhombus customers sign in to the developer''s product. Gives per-user consent, refresh tokens and revocation.'
  dynamic_client_registration: true
  endpoints:
    authorization: https://console.rhombus.com/oauth/authorize
    issuer: https://auth-web.rhombussystems.com/
    registration: https://auth-web.rhombussystems.com/oauth/register
    revocation: https://auth.rhombussystems.com/oauth/token/revoke
    token: https://auth.rhombussystems.com/oauth/token
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  name: OAuth2
  pkce: true
  pkce_methods:
  - S256
  recommended_for: third-party applications acting on behalf of a Rhombus user
  response_types_supported:
  - code
  sources:
  - https://www.rhombus.com/auth.md
  - https://api-docs.rhombus.community/oauth-authentication
  - https://auth.rhombussystems.com/oauth/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  token_exchange_header:
    x-auth-scheme: web2
  type: oauth2
  usage_headers:
    x-auth-access-token: ACCESS_TOKEN
    x-auth-scheme: api-oauth-token
slug: rhombus-systems-authentication
source_filename: rhombus-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.rhombus.com/auth.md\nsecondary_sources:\n- https://api-docs.rhombus.community/oauth-authentication\n- https://api2.rhombussystems.com/.well-known/oauth-protected-resource\n- https://auth.rhombussystems.com/oauth/.well-known/oauth-authorization-server\n- openapi/rhombus-systems-openapi.json\nnote: >-\n  Upgraded from derived to searched. The OpenAPI declares only ONE security scheme (ApiKeyAuth),\n  but Rhombus publishes a full second method — OAuth 2.0 authorization code with PKCE — in a\n  dedicated machine-readable auth guide and in its own agent card. The spec understates the auth\n  surface; this artifact records what the provider actually supports.\nanonymous_access: false\nanonymous_statement: 'There is no anonymous access: every API call requires one of the two credentials.'\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  methods: 2\nhosts:\n- host: api2.rhombussystems.com\n  role: resource\
  \ server (all API calls)\n- host: console.rhombus.com\n  role: interactive sign-in and OAuth authorization\n- host: auth.rhombussystems.com\n  role: OAuth token, refresh, revocation and client registration\n- host: auth-web.rhombussystems.com\n  role: declared OAuth issuer in the RFC 8414 metadata\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-auth-apikey\n  companion_header:\n    name: x-auth-scheme\n    values: [api-token, partner-api-token]\n    required: true\n  description: >-\n    Rhombus API key. Requires the x-auth-scheme companion header — a key alone is not a complete\n    credential. api-token for standard auth, partner-api-token for partner/MSP auth.\n  self_serve: true\n  provisioning: https://console.rhombus.com/settings/api-management\n  shown_once: true\n  permission_model: >-\n    A key INHERITS the permissions of the user who created it. There are no key-level scopes;\n    least privilege is achieved by creating the key from a least-privileged\
  \ user or role.\n  recommended_for: agents, scripts, server-to-server integrations acting as one Rhombus account\n  region_bound: true\n  region_note: Keys are bound to their region — a US key will not work against api2.eu.rhombussystems.com.\n  sources:\n  - openapi/rhombus-systems-openapi.json\n  - https://www.rhombus.com/auth.md\n- name: OAuth2\n  type: oauth2\n  flow: authorization_code\n  pkce: true\n  pkce_methods: [S256]\n  description: >-\n    \"Sign in with Rhombus\" — OAuth 2.0 authorization code with PKCE, for third-party apps where\n    Rhombus customers sign in to the developer's product. Gives per-user consent, refresh tokens\n    and revocation.\n  declared_in_openapi: false\n  endpoints:\n    authorization: https://console.rhombus.com/oauth/authorize\n    token: https://auth.rhombussystems.com/oauth/token\n    revocation: https://auth.rhombussystems.com/oauth/token/revoke\n    registration: https://auth-web.rhombussystems.com/oauth/register\n    issuer: https://auth-web.rhombussystems.com/\n\
  \  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, none]\n  dynamic_client_registration: true\n  usage_headers:\n    x-auth-scheme: api-oauth-token\n    x-auth-access-token: ACCESS_TOKEN\n  token_exchange_header:\n    x-auth-scheme: web2\n  access_token_lifetime_sec: 3600\n  client_provisioning:\n    operationId: submitApplication\n    path: /api/oauth/submitApplication\n    authenticated_with: an API key\n    returns: [clientId, clientSecret]\n    related_operations: [getAllApplicationsForOrg, getApplicationByClientId, updateApplication, deleteApplication]\n    secret_shown_once: true\n    review_required: >-\n      Production apps distributed to other organizations require Rhombus review, started in the\n      developer community.\n  recommended_for: third-party applications acting on behalf of a Rhombus user\n  sources:\n  - https://www.rhombus.com/auth.md\n\
  \  - https://api-docs.rhombus.community/oauth-authentication\n  - https://auth.rhombussystems.com/oauth/.well-known/oauth-authorization-server\nscopes:\n  published: false\n  scope_count: 0\n  note: >-\n    Rhombus publishes NO OAuth scope vocabulary. The RFC 8414 metadata omits scopes_supported\n    entirely and the provider's own agent card declares the oauth2 flow with an empty scopes\n    object. Authorization is therefore role-derived (the consenting user's permissions), not\n    scope-derived, and an agent cannot request or reason about least-privilege at the token\n    level. No scopes/ artifact is emitted because there is no scope surface to record.\n  role_model:\n    operations:\n    - getPermissionGroups\n    - getPartnerPermissionGroups\n    - getUsersInOrg\n    note: Permissions are managed as org permission groups (Permission Webservice, 10 operations).\ndiscovery:\n  rfc9728:\n    url: https://api2.rhombussystems.com/.well-known/oauth-protected-resource\n    status: 200\n\
  \    anonymous: true\n    resource: https://api2.rhombussystems.com\n    authorization_servers: [https://auth-web.rhombussystems.com/]\n    bearer_methods_supported: [header]\n  rfc8414:\n    url: https://auth.rhombussystems.com/oauth/.well-known/oauth-authorization-server\n    status: 200\n    anonymous: true\n  challenge:\n    status: 401\n    header: 'WWW-Authenticate: Bearer resource_metadata=\"https://api2.rhombussystems.com/.well-known/oauth-protected-resource\"'\n    note: >-\n      The entire discovery chain is reachable from ONE unauthenticated probe — a 401 on any\n      endpoint hands back the RFC 9728 URL, which names the authorization server, whose RFC 8414\n      document names every endpoint. This is a genuinely agent-friendly bootstrap.\n  openid_connect:\n    supported: false\n    probe: https://www.rhombus.com/.well-known/openid-configuration\n    status: 404\nmtls:\n  supported: true\n  note: >-\n    The Rhombus Console offers certificate-based API keys in addition to\
  \ token-based ones. The\n    published OpenAPI does not model a mutualTLS security scheme, and the AsyncAPI states\n    explicitly that certificate (mTLS) keys are NOT supported by the WebSocket service — only\n    token-based keys are.\n  source: asyncapi/rhombus-systems-console-websocket-asyncapi.json\nenterprise_sso:\n  saml2: true\n  operations: [getSAMLSettings, getSAMLSettingsV2, updateSAMLSettings, updateSAMLSettingsV2]\n  scim: true\n  scim_operations: [setupSCIMAccessForOrg, findSCIMSettingsForOrg, updateSCIMSettingsForOrg, getScimDisplayInfo, revokeSCIMAccessForOrg]\n  idps_documented: [Okta, Azure AD, Google Workspace, OneLogin]\n  documentation: https://api-docs.rhombus.community/implementations/saml-sso-provisioning\npartner_auth:\n  scheme_value: partner-api-token\n  org_scoping_header: x-auth-org\n  note: MSPs and resellers authenticate with a partner key and scope calls to a managed client org.\n  documentation: https://api-docs.rhombus.community/partner-api-calls\ngaps:\n\
  - The OpenAPI declares only ApiKeyAuth; the OAuth 2.0 method it fully documents elsewhere is absent from the contract.\n- No OAuth scope vocabulary, so no least-privilege token model.\n- No key-level scoping — an API key carries its creator's full permissions.\n- No OIDC discovery document, so no standard identity-claim surface despite OAuth support.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhombus-systems/refs/heads/main/authentication/rhombus-systems-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Physical Security
- Video Surveillance
- Access Control
- IoT Sensors
- Cloud Video Management
- Alarm Monitoring
- Computer Vision
- Building Management
- Security Cameras
- Company
---
